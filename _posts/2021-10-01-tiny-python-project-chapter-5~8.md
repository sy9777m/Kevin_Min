---
toc: true
layout: post
description: Tiny Python Project Chapter 5 ~ 8 for Find-A.
categories: [markdown]
title: Tiny Python Project chapter 5 ~ 8
---
# Tiny Python Project Chapter 5 ~ 8

## Chapter 5

![image-20211001233148710](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233148710.png)

![image-20211001233209804](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233209804.png)

![image-20211001233219993](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233219993.png)

![image-20211001233250181](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233250181.png)

![image-20211001233300367](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233300367.png)

![image-20211001233326520](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233326520.png)

![image-20211001233427568](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233427568.png)

![image-20211001233646494](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233646494.png)

![image-20211001233630917](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233630917.png)

![image-20211001233747120](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233747120.png)

![image-20211001233752815](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233752815.png)

![image-20211001233805801](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233805801.png)

![image-20211001233821350](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233821350.png)

![image-20211001233830874](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001233830874.png)

![image-20211001234035570](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001234035570.png)

![image-20211001234055468](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001234055468.png)

![image-20211001234152805](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001234152805.png)

![image-20211001234202552](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211001234202552.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@9762e84df2b1>
Date   : 2021-10-01
Purpose: Rock the Casbah
"""

import argparse
import os
import sys

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Rock the Casbah',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
                        metavar='text',
                        type=str,
                        help='Input string or file')

    parser.add_argument('-o',
                        '--outfile',
                        help='Output filename',
                        metavar='str',
                        type=str,
                        default='')

    args = parser.parse_args()

    if os.path.isfile(args.text):
        args.text = open(args.text).read().rstrip()

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    text_arg = args.text
    filename_arg = args.outfile

    out_fh = open(filename_arg, 'wt') if filename_arg else sys.stdout
    out_fh.write(text_arg.upper() + '\n')
    out_fh.close()



# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211002001109223](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001109223.png)

![image-20211002001143460](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001143460.png)

![image-20211002001224039](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001224039.png)

![image-20211002001230174](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001230174.png)

![image-20211002001240260](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001240260.png)

![image-20211002001248275](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001248275.png)

# Chapter 6

![image-20211002001500256](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002001500256.png)

![image-20211002002046258](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002002046258.png)

![image-20211002002135867](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002002135867.png)

![image-20211002002202839](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002002202839.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@9762e84df2b1>
Date   : 2021-10-01
Purpose: Rock the Casbah
"""

import argparse
import sys


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Rock the Casbah',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('file',
                        metavar='FILE',
                        nargs='*',
                        type=argparse.FileType('rt'),
                        default=[sys.stdin],
                        help='Input file(s)')

    return parser.parse_args()


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()

    totalLineCounts, totalWordsCounts, totalByteCounts = 0, 0, 0

    for fh in args.file:
        lineCounts, wordsCounts, byteCounts = 0, 0, 0

        for l in fh:      
            lineCounts += 1;
            wordsCounts += len(l.split())
            byteCounts += len(l)
        
        totalLineCounts += lineCounts
        totalWordsCounts += wordsCounts
        totalByteCounts += byteCounts

        print(f'{lineCounts:8}{wordsCounts:8}{byteCounts:8} {fh.name}')
    
    if len(args.file) > 1:
        print(f'{totalLineCounts:8}{totalWordsCounts:8}{totalByteCounts:8} total')
        


# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211002004150107](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002004150107.png)

![image-20211002004205286](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002004205286.png)

# Chapter 7

![image-20211002004318306](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002004318306.png)

![image-20211002004347239](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002004347239.png)

![image-20211002005659600](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002005659600.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@f139ec3a85b3>
Date   : 2021-10-01
Purpose: Rock the Casbah
"""

import argparse


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Rock the Casbah',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('letter',
                        metavar='letter',
                        nargs='+',
                        help='Letter(s)',)

    parser.add_argument('-f',
                        '--file',
                        help='Input file',
                        metavar='FILE',
                        type=argparse.FileType('rt'),
                        default='gashlycrumb.txt')

    return parser.parse_args()


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()

    sentenceDict = {v[0]: v for v in args.file}

    for letter in args.letter:
        if (letter.upper() not in sentenceDict.keys()):
            print('I do not know \"{}\".'.format(letter))
            continue
        print(sentenceDict[letter.upper()], end='')


# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211002010825155](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002010825155.png)

![image-20211002010836838](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002010836838.png)

![image-20211002010853523](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002010853523.png)

![image-20211002010900102](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002010900102.png)

# Chapter 8

![image-20211002011200723](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002011200723.png)

![image-20211002011208396](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002011208396.png)

![image-20211002011214020](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002011214020.png)

![image-20211002011743894](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002011743894.png)

![image-20211002012031902](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002012031902.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@c71caa78d29f>
Date   : 2021-10-01
Purpose: Rock the Casbah
"""

import argparse
import os


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Apples and bananas',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
                        metavar='text',
                        help='Input text or file')

    parser.add_argument('-v',
                        '--vowel',
                        help='The vowel to substitute',
                        metavar='vowel',
                        type=str,
                        default='a',
                        choices=['a', 'e', 'i', 'o', 'u'])

    args = parser.parse_args()
    if os.path.isfile(args.text):
        args.text = open(args.text).read().rstrip()

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    text_arg = args.text
    vowel_arg = args.vowel

    if text_arg.isupper():
        vowel_dict = {v: vowel_arg.upper() for v in ['a', 'e', 'i', 'o', 'u', 'A', 'E', 'I', 'O', 'U']}
    else:
        vowel_dict = {v: vowel_arg.lower() for v in ['a', 'e', 'i', 'o', 'u', 'A', 'E', 'I', 'O', 'U']}
    new = ''
    new = text_arg.translate(str.maketrans(vowel_dict))

    print(new)



# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211002013348976](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002013348976.png)

![image-20211002013427566](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002013427566.png)

![image-20211002013442012](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002013442012.png)

![image-20211002013456408](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002013456408.png)

![image-20211002013515338](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002013515338.png)

![image-20211002013521244](/Kevin_Min/images/2021-10-01-tiny-python-project-chapter-5~8/image-20211002013521244.png)

