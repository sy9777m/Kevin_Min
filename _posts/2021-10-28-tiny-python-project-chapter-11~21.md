---
toc: true
layout: post
description: Tiny Python Project Chapter 11 ~ 21 for Find-A.
categories: [markdown]
title: Tiny Python Project chapter 11 ~ 21
---
# Tiny Python Project Chapter 11 ~ 21

## Chapter 11. 맥주병 노래: 함수 작성 및 테스트

![image-20211028091059547](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028091059547.png)

![image-20211028091113621](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028091113621.png)

![image-20211028091118411](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028091118411.png)

![image-20211028091450877](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028091450877.png)

![image-20211028104605929](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028104605929.png)

![image-20211028104616076](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028104616076.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@e5040579c2cf>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Bottles of beer song',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-n',
                        '--num',
                        help='How many bottles',
                        metavar='number',
                        type=int,
                        default=10)

    args = parser.parse_args()

    if (args.num < 0):
        parser.error(f'--num "{args.num}" must be greater than 0')

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    num = args.num

    # for i in range(num, 0, -1):
    #     print(verse(i))

    print('\n\n'.join(map(verse, range(num, 0, -1))))
        
def verse(bottle):
    sing_verse = ''
    if (bottle == 1):
        sing_verse = '\n'.join([f'{bottle} bottle of beer on the wall,', f'{bottle} bottle of beer,', 'Take one down, pass it around,', 'No more bottles of beer on the wall!'])
    
    elif (bottle == 2):
        sing_verse = '\n'.join([f'{bottle} bottles of beer on the wall,', f'{bottle} bottles of beer,', 'Take one down, pass it around,', f'{bottle - 1} bottle of beer on the wall!'])
        
    else:
        sing_verse = '\n'.join([f'{bottle} bottles of beer on the wall,', f'{bottle} bottles of beer,', 'Take one down, pass it around,', f'{bottle - 1} bottles of beer on the wall!'])
        

    return sing_verse

def test_verse():
    """Test verse"""

    last_verse = verse(1)
    assert last_verse == '\n'.join([
        '1 bottle of beer on the wall,', '1 bottle of beer,', 'Take one down, pass it around,', 'No more bottles of beer on the wall!'
    ])

    two_bottles = verse(2)
    assert two_bottles == '\n'.join([
        '2 bottles of beer on the wall,', '2 bottles of beer,', 'Take one down, pass it around,', '1 bottle of beer on the wall!'
    ])

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211028110723435](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028110723435.png)

![image-20211028110728946](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028110728946.png)

![image-20211028110735521](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028110735521.png)

## Chapter 12. 협박 편지: 텍스트를 무작위로 대문자화하기

![image-20211028111110183](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028111110183.png)

![image-20211028111119362](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028111119362.png)

![image-20211028111126792](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028111126792.png)

![image-20211028111750799](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028111750799.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@bc67f35f04dd>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import random
import os

# --------------------------------------------------
def get_args():
    """Ransom Note"""

    parser = argparse.ArgumentParser(
        description='Ransom Note',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
    metavar='text',
                        help='Input text or file')

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='int',
                        type=int,
                        default=None)

    args = parser.parse_args()

    if os.path.isfile(args.text):
        args.text = open(args.text).read().rstrip()

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    random.seed(args.seed)
    original_t = args.text
    t = ''.join([choose(original_t[i]) for i in range(len(original_t))])
    print(t)

def choose(char):
    return random.choice([char.lower(), char.upper()])

def test_choose():
    state = random.getstate()
    random.seed(1)
    assert choose('a') == 'a'
    assert choose('b') == 'b'
    assert choose('c') == 'c'
    assert choose('d') == 'd'
    random.setstate(state)

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211028112436771](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028112436771.png)

![image-20211028112519886](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028112519886.png)

## Chapter 13. 12일간의 크리스마스: 알고리즘 디자인

![image-20211028112633192](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028112633192.png)

![image-20211028112642264](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028112642264.png)

![image-20211028113012514](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028113012514.png)

![image-20211028113019770](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028113019770.png)

![image-20211028114129950](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028114129950.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@117e0abe372c>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import os
import sys


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Twelve Days of christmas',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-n',
                        '--num',
                        help='Number of days to sing',
                        metavar='days',
                        type=int,
                        default=12)

    parser.add_argument('-o',
                        '--outfile',
                        help='Outfile',
                        metavar='FILE',
                        type=argparse.FileType('wt'),
                        default=sys.stdout)

    args = parser.parse_args()

    if not(1 <= args.num <= 12):
        parser.error(f'--num "{args.num}" must be between 1 and 12')
        
    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    num = args.num
    
    print('\n\n'.join([verse(day) for day in range(1, num + 1)]), end='', file=args.outfile)

def verse(day):
    ordinal = ['first', 'second', 'third', 'fourth', 'fifth', 'sixth', 'seventh', 'eighth', 'ninth', 'tenth', 'eleventh', 'twelfth']

    present = ['twelve drummers drumming', 'eleven pipers piping', 'ten lords a leaping', 'nine ladies dancing', 'eight maids a milking', 'seven swans a swimming', 'six geese a laying', 'five gold rings', 'four calling birds', 'three French hens', 'two turtle doves', 'a partridge in a pear tree']

    present_sent = ''

    for i in reversed(range(1, day + 1)):
        if (day > 1 and i == 1):
            present_sent += f'And {present[-1 * i]}.'
        
        elif (day == 1):
            present_sent += f'{present[-1 * i].capitalize()}.'
        
        else:
            present_sent += f'{present[-1 * i][0].upper()}{present[-1 * i][1:]},\n'

    return '\n'.join([f'On the {ordinal[day - 1]} day of Christmas,', 'My true love gave to me,', present_sent])

def test_verse():
    assert verse(1) == '\n'.join(['On the first day of Christmas,', 'My true love gave to me,', 'A partridge in a pear tree.'])
    assert verse(2) == '\n'.join(['On the second day of Christmas,', 'My true love gave to me,', 'A partridge in a pear tree.'])

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211028134238381](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028134238381.png)

![image-20211028134245241](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028134245241.png)

![image-20211028134315766](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028134315766.png)

![image-20211028134324646](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028134324646.png)

![image-20211028134340037](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028134340037.png)

## Chapter 14. 운율 생성기: 정규 표현식을 사용해서 운율 맞추기

![image-20211028135454852](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028135454852.png)

![image-20211028135506371](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028135506371.png)

![image-20211028141608445](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028141608445.png)

![image-20211028141602464](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028141602464.png)

![image-20211028141702902](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028141702902.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@c05ebd5110ee>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import re
import string as s

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Make rhyming "word"',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('word',
                        metavar='word',
                        help='A word to rhyme')

    return parser.parse_args()


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    word = args.word

    w_list = list('bcdfghjklmnpqrstvwxyz') + (
        'bl br ch cl cr dr fl fr gl gr pl pr sc '
        'sh sk sl sm sn sp st sw th tr tw thw wh wr '
        'sch scr shr sph spl spr squ str thr').split()

    w_list = sorted(w_list)

    start, rest = stemmer(word)

    if rest == '':
        print(f'Cannot rhyme "{start}"')
    else:
        print('\n'.join([f'{w}{rest}' for w in w_list]))

def stemmer(word):
    consonants = ''.join([c for c in s.ascii_lowercase if c not in 'aeiou'])
    pattern = f'([{consonants}]+)?([aeiou])(.*)'

    match = re.match(pattern, word.lower())

    if match:
        start = match.group(1) or ''
        aeiou = match.group(2) or ''
        rest = match.group(3) or ''
        return (start, aeiou + rest)

    else:
        return (word, '')

def test_stemmer():
    assert stemmer('') == ('', '')
    assert stemmer('cake') == ('c', 'ake')
    assert stemmer('chair') == ('ch', 'air')
    assert stemmer('APPLE') == ('', 'apple')
    assert stemmer('RDNZL') == ('rdnzl', '')
    assert stemmer('123') == ('123', '')
# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211028171658450](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028171658450.png)

![image-20211028171720475](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028171720475.png)

![image-20211028171749321](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028171749321.png)

![image-20211028171759009](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028171759009.png)

## Chapter 15. 켄터키 수도사: 정규 표현식 더 배워보기

![image-20211028235724282](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028235724282.png)

![image-20211028235728792](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028235728792.png)

![image-20211028235736730](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028235736730.png)

![image-20211028235742184](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028235742184.png)

![image-20211028235857880](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211028235857880.png)

![image-20211029000005376](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000005376.png)

![image-20211029000057073](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000057073.png)

![image-20211029000105580](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000105580.png)

![image-20211029000118664](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000118664.png)

![image-20211029000132586](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000132586.png)

![image-20211029000138399](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000138399.png)

![image-20211029000151272](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000151272.png)

![image-20211029000222752](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000222752.png)

![image-20211029000228575](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000228575.png)

![image-20211029000330568](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000330568.png)

![image-20211029000619591](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000619591.png)

![image-20211029000643386](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000643386.png)

![image-20211029000705435](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029000705435.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@c6ec56f874a6>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import os
import re

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Southern fry text',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
                        metavar='text',
                        help='Input text or file')

    args = parser.parse_args()

    if os.path.isfile(args.text):
        args.text = open(args.text).read().rstrip()

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    text = args.text
    
    for w in re.split(r'(\W+)', text):
        print(fry(w), end='')

def fry(text):
    word = text.lower()
    if word == 'you':
        return text[0] + "'all"

    match = re.search(r'(.+)ing$', text)
    if match:
        first = match.group(1) or ''
    else:
        return text

    if re.search(r'[aeiouy]', first.lower()):
        return first + "in'"
    else:
        return text

def test_fry():
    assert fry('you') == "y'all"
    assert fry('You') == "Y'all"
    assert fry('fishing') == "fishin'"
    assert fry('Aching') == "Achin'"
    assert fry('swing') == "swing"

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029025220915](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029025220915.png)

## Chapter 16. 믹서기: 무작위로 단어의 중간 부분 재정렬하기

![image-20211029025341877](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029025341877.png)

![image-20211029025351361](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029025351361.png)

![image-20211029025359920](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029025359920.png)

![image-20211029025736393](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029025736393.png)

![image-20211029025745219](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029025745219.png)

![image-20211029030039936](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029030039936.png)

![image-20211029030052811](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029030052811.png)

````python
#!/usr/bin/env python3
"""
Author : runner <runner@ab92a6669e44>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import os
import re
import random

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Scramble the letters of words',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
                        metavar='text',
                        help='Input text or fileoptional arguments:')

    parser.add_argument('-s',
                        '--seed',
                        help='Randome seed',
                        metavar='seed',
                        type=int,
                        default=None)

    args = parser.parse_args()
    if os.path.isfile(args.text):
        args.text = open(args.text).read()

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    random.seed(args.seed)
    text = args.text

    splitter = re.compile("([a-zA-Z](?:[a-zA-Z']*[a-zA-Z])?)")

    for w in splitter.split(text):
        if re.match(r"\w", w):
            print(scramble(w), end='')
        else:
            print(w, end='')

def scramble(word):
    if len(word) > 3:
        list_word = list(word[1:-1])
        random.shuffle(list_word)
        return ''.join([word[0], *list_word, word[-1]])
    else:
        return word

def test_scramble():
    state = random.getstate()
    random.seed(1)
    assert scramble('a') == 'a'
    assert scramble('ab') == 'ab'
    assert scramble('abc') == 'abc'
    assert scramble('abcd') == 'acbd'
    assert scramble('abcde') == 'acbde'
    assert scramble('abcdef') == 'aecbdf'
    assert scramble("abcde'f") == "abcd'ef"
    random.setstate(state)


# --------------------------------------------------
if __name__ == '__main__':
    main()

````

![image-20211029031630704](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031630704.png)

![image-20211029031649057](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031649057.png)

![image-20211029031658673](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031658673.png)

## Chapter 17. 매드립: 정규 표현식 사용하기

![image-20211029031832993](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031832993.png)

![image-20211029031838697](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031838697.png)

![image-20211029031951913](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031951913.png)

![image-20211029031940751](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029031940751.png)

![image-20211029032358927](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032358927.png)

![image-20211029032427222](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032427222.png)

![image-20211029032518238](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032518238.png)

![image-20211029032603026](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032603026.png)

![image-20211029032617678](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032617678.png)

![image-20211029032707879](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032707879.png)

![image-20211029032823913](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029032823913.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@ab92a6669e44>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import re
import sys

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Mad Libs',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('file',
                        metavar='FILE',
                        help='Input file',
                        type=argparse.FileType('rt'))

    parser.add_argument('-i',
                        '--inputs',
                        help='Inputs (for testing)',
                        metavar='input',
                        type=str,
                        nargs='*',)

    return parser.parse_args()


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    inputs = args.inputs
    text = args.file.read().rstrip()
    splitter = re.compile(r"(<([^<>]+)>)")
    blanks = re.findall(splitter, text)

    if not blanks:
        sys.exit(f'"{args.file.name}" has no placeholders.')

    tmpl = 'Give me {} {}'

    for placeholder, name in blanks:
        article = 'an' if name.lower()[0] in 'aeiou' else 'a'
        answer = inputs.pop(0) if inputs else input(tmpl.format(article, name))
        text = re.sub(f"{placeholder}", answer, text, count=1)
        
    print(text)


# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029043147498](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029043147498.png)

![image-20211029043200995](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029043200995.png)

## Chapter 18. 게마트리아: 아스키값을 사용한 텍스트 수치화

![image-20211029044046784](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029044046784.png)

![image-20211029044059191](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029044059191.png)

![image-20211029044039899](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029044039899.png)

![image-20211029044120790](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029044120790.png)

![image-20211029044205266](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029044205266.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@2cf8b1eba529>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import os
import re

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Gematria',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
                        metavar='text',
                        help='Input text or file')

    args = parser.parse_args()
    if os.path.isfile(args.text):
        args.text = open(args.text).read()

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    text = args.text
    
    for line in text.splitlines():
        print(' '.join(map(word2num, line.split())))

def word2num(word):
    text = re.sub(r'[^A-Za-z0-9]', '', word)
    num = str(sum(map(ord, re.findall(r'[A-Za-z0-9]', text))))
    return num

def test_word2num():
    assert word2num("a") == "97"
    assert word2num("abc") == "294"
    assert word2num("ab'c") == "294"
    assert word2num("4a-b'c,") == "346"

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029050326175](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029050326175.png)

## Chapter 19. 오늘의 운동: CSV 파일 사용하기와 텍스트 테이블 만들기

![image-20211029050755895](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029050755895.png)

![image-20211029050904470](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029050904470.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@68d96a2911e0>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import csv
from tabulate import tabulate
import io
import re
import random

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Create Workout Of (the) Day (WOD)',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-f',
                        '--file',
                        help='CSV input file of exercises',
                        metavar='FILE',
                        type=argparse.FileType('rt'),
                        default='inputs/exercises.csv')

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='seed',
                        type=int,
                        default=None)

    parser.add_argument('-n',
                        '--num',
                        help='Number of exercises',
                        metavar='exercises',
                        type=int,
                        default=4)

    parser.add_argument('-e',
                        '--easy',
                        help='Halve the reps',
                        action='store_true')

    args = parser.parse_args()

    if args.num < 1:
        parser.error(f'--num "{args.num}" must be greater than 0')

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    random.seed(args.seed)
    wod = []
    exercises = read_csv(args.file)

    for ex, low, high in random.sample(exercises, k=args.num):
        rep = random.randint(low, high)
        if args.easy:
            rep = int(rep / 2)
        wod.append((ex, rep))
    
    print(tabulate(wod, headers=('Exercise', 'Reps')))

def read_csv(fh):
    exercises = []
    for row in csv.DictReader(fh, delimiter=','):
        low, high = map(int, row['reps'].split('-'))
        exercises.append((row['exercise'], low, high))

    return exercises
def test_read_csv():
    text = io.StringIO('exercise,reps\nBurpees,20-50\nSitups,40-100')
    assert read_csv(text) == [('Burpees', 20, 50), ('Situps', 40, 100)]


# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029072039151](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029072039151.png)

## Chapter 20. 패스워드 강도: 안전하고 기억하기 쉬운 패스워드 생성하기

![image-20211029074224073](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029074224073.png)

![image-20211029074231364](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029074231364.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@8e6e030411c6>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import re
import random
import argparse
import string


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Rock the Casbah',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('file',
                        metavar='FILE',
                        help='Input file(s)',
                        nargs='+',
                        type=argparse.FileType('rt'))

    parser.add_argument('-n',
                        '--num',
                        help='Number of passwords to generate',
                        metavar='num_passwords',
                        type=int,
                        default=3)

    parser.add_argument('-w',
                        '--num_words',
                        help='Number of words to use for password',
                        metavar='num_words',
                        type=int,
                        default=4)

    parser.add_argument('-m',
                        '--min_word_len',
                        help='Minimum word length',
                        metavar='minimum',
                        type=int,
                        default=3)

    parser.add_argument('-x',
                        '--max_word_len',
                        help='Maximum word length',
                        metavar='maximum',
                        type=int,
                        default=6)

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='seed',
                        type=int,
                        default=None)

    parser.add_argument('-l',
    '--l33t',
    help='Obfuscate letters',
    action='store_true')

    return parser.parse_args()


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    random.seed(args.seed)
    words = set()

    def word_len(word):
        return args.min_word_len <= len(word) <= args.max_word_len

    for fh in args.file:
        for line in fh:
            for word in filter(word_len, map(clean, line.lower().split())):
                words.add(word.capitalize())
    
    words = sorted(words)
    passwords = [''.join(random.sample(words, args.num_words)) for _ in range(args.num)]

    if args.l33t:
        passwords = map(l33t, passwords)

    print('\n'.join(passwords))

def l33t(word):
    word = ransom(word)
    l33t_dict = str.maketrans({'a': '@', 'A': '4', 'O': '0', 't': '+', 'E': '3', 'I': '1', 'S': '5'})

    return word.translate(l33t_dict) + random.choice(string.punctuation)

def test_l33t():
    state = random.getstate()
    random.seed(1)
    assert l33t('Money') == 'moNeY{'
    assert l33t('Dollars') == 'D0ll4r5`'
    random.setstate(state)

def ransom(word):
    new_word = ''
    for w in word.lower():
        if random.choice([True, False]):
            new_word += w
        else:
            new_word += w.upper()
    return new_word

def test_ransom():
    state = random.getstate()
    random.seed(1)
    assert ransom('Money') == 'moNeY'
    assert ransom('Dollars') == 'DOLlaRs'
    random.setstate(state)

def clean(word):
    word = re.sub(r'[^a-zA-Z]', '', word)
    return word

def test_clean():
    assert clean('') == ''
    assert clean('states,') == 'states'
    assert clean("Don't") == 'Dont'

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029082305559](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029082305559.png)

![image-20211029082318959](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029082318959.png)

## Chapter 21. 틱택토 게임: 상태 확인하기

![image-20211029084154653](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029084154653.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@ded74145e45a>
Date   : 2021-10-28
Purpose: Rock the Casbah
"""

import argparse
import re

# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Rock the Casbah',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-b',
                        '--board',
                        help='',
                        metavar='board',
                        type=str,
                        default='.' * 9)

    parser.add_argument('-p',
                        '--player',
                        help='',
                        metavar='player',
                        type=str,
                        choices=['X', 'O'],
                        default=None)

    parser.add_argument('-c',
                        '--cell',
                        help='',
                        metavar='cell',
                        type=int,
                        choices=[i for i in range(1, 10)],
                        default=None)

    args = parser.parse_args()

    if (args.player == None and args.cell != None) or (args.cell == None and args.player != None):
        parser.error('Must provide both --player and --cell')

    if not re.search(r'^[.XO]{9}$', args.board):
        parser.error(f'--board "{args.board}" must be 9 characters of ., X, O')

    if args.player and args.cell and args.board[args.cell - 1] in 'XO':
        parser.error(f'--cell "{args.cell}" already taken')

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    board = args.board
    cell = args.cell
    player = args.player

    if None not in (player, cell):
        board = ''.join([player if (cell - 1) == i else c for i, c in enumerate(board)])

    result = find_winner(board)
    if result == None:
        result = 'No winner.'
    else:
        result += ' has won!'
    
    print(format_board(board) + f'\n{result}')

def format_board(board):
    board = ''.join([c if c in 'XO' else str(i + 1) for i, c in enumerate(board)])

    board = f"""-------------
| {board[0]} | {board[1]} | {board[2]} |
-------------
| {board[3]} | {board[4]} | {board[5]} |
-------------
| {board[6]} | {board[7]} | {board[8]} |
-------------"""

    return board

def find_winner(board):
    wins = [('PPP......'), ('...PPP...'), ('......PPP'), ('P..P..P..'),
            ('.P..P..P.'), ('..P..P..P'), ('P...P...P'), ('..P.P.P..')]

    for p in 'XO':
        other_player = 'O' if p == 'X' else 'X'
        for b in wins:
            win_board = b.replace('P', p)
            comp_board = board.replace(other_player, '.')
            count = 0
            for i, c in enumerate(win_board):
                if comp_board[i] != '.' and comp_board[i] == c:
                    count += 1
                if count == 3:
                    return p

    return None

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029153031020](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153031020.png)

## Chapter 22. 돌아온 틱택토 게임: 타입 힌트를 사용한 대화형 버전

![image-20211029153120042](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153120042.png)

![image-20211029153244622](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153244622.png)

![image-20211029153544734](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153544734.png)

![image-20211029153552623](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153552623.png)

![image-20211029153616572](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153616572.png)

![image-20211029153633936](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153633936.png)

![image-20211029153648410](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153648410.png)

![image-20211029153658883](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153658883.png)

![image-20211029153733124](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153733124.png)

![image-20211029153744777](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153744777.png)

![image-20211029153757951](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153757951.png)

![image-20211029153810373](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029153810373.png)

![image-20211029154117355](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029154117355.png)

![image-20211029154139143](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029154139143.png)

![image-20211029154212666](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029154212666.png)

![image-20211029154223367](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029154223367.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@1a4e6e4cffcf>
Date   : 2021-10-29
Purpose: Rock the Casbah
"""

import re
from typing import List, NamedTuple, Optional

# --------------------------------------------------
def main():
    """Make a jazz noise here"""
    state = State()

    while not state.quit:
        print("\033[H\033[J")
        print(format_board(state.board))
        if state.error:
            print(state.error)
            state = state._replace(error=None)
        val = input(f'Player {state.player}, what is your move? [q to quit] ')

        if val == 'q':
            state = state._replace(quit=True)
            print('You lose, loser!')
            break
        elif state.draw:
            print("All right, we'll call it a draw.")
            break
        elif not re.search(r'^[1-9]$', val):
            state = state._replace(error=f'Invaild cell "{val}", please use 1-9')
            continue
        else:
            val = int(val)
        
        if state.board[int(val) - 1] in 'XO':
            state = state._replace(error=f'Cell "{val}" already taken.')
            continue
        
        state = state._replace(board=[state.player if i == (val - 1) else c for i, c in enumerate(state.board)])

        winner = find_winner(''.join(state.board))
        next_player = 'O' if state.player == 'X' else 'X'

        if winner:
            print(format_board(''.join(state.board)))
            print(f'{state.player} has won!')
            state = state._replace(quit=True)
            continue
        elif not winner and '.' not in state.board:
            state = state._replace(draw=True)
        else:
            state = state._replace(player=next_player)

def format_board(board):
    board = ''.join([c if c in 'XO' else str(i + 1) for i, c in enumerate(board)])

    board = f"""-------------
| {board[0]} | {board[1]} | {board[2]} |
-------------
| {board[3]} | {board[4]} | {board[5]} |
-------------
| {board[6]} | {board[7]} | {board[8]} |
-------------"""

    return board

def find_winner(board):
    wins = [('PPP......'), ('...PPP...'), ('......PPP'), ('P..P..P..'),
            ('.P..P..P.'), ('..P..P..P'), ('P...P...P'), ('..P.P.P..')]

    for p in 'XO':
        other_player = 'O' if p == 'X' else 'X'
        for b in wins:
            win_board = b.replace('P', p)
            comp_board = board.replace(other_player, '.')
            count = 0
            for i, c in enumerate(win_board):
                if comp_board[i] != '.' and comp_board[i] == c:
                    count += 1
                if count == 3:
                    return p

    return None

class State(NamedTuple):
    board: List[str] = list('.' * 9)
    player: str = 'X'
    quit: bool = False
    draw: bool = False
    error: Optional[str] = None
    winner: Optional[str] = None

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211029163151406](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163151406.png)

![image-20211029163156607](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163156607.png)

## 마치며

![image-20211029163213333](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163213333.png)

![image-20211029163234981](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163234981.png)

![image-20211029163238679](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163238679.png)

## argparse 사용하기

![image-20211029163319915](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163319915.png)

![image-20211029163445766](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163445766.png)

![image-20211029163506441](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163506441.png)

![image-20211029163520121](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163520121.png)

![image-20211029163528026](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163528026.png)

![image-20211029163536997](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163536997.png)

![image-20211029163544972](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163544972.png)

![image-20211029163555473](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163555473.png)

![image-20211029163609312](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163609312.png)

![image-20211029163625125](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163625125.png)

![image-20211029163634566](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163634566.png)

![image-20211029163650214](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163650214.png)

![image-20211029163715105](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163715105.png)

![image-20211029163722238](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163722238.png)

![image-20211029163732310](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163732310.png)

![image-20211029163746868](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163746868.png)

![image-20211029163758256](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163758256.png)

![image-20211029163803990](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163803990.png)

![image-20211029163812708](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163812708.png)

![image-20211029163840606](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163840606.png)

![image-20211029163851368](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163851368.png)

![image-20211029163855731](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163855731.png)

![image-20211029163901835](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163901835.png)

![image-20211029163913872](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163913872.png)

![image-20211029163924193](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163924193.png)

![image-20211029163933408](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163933408.png)

![image-20211029163941919](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163941919.png)

![image-20211029163953506](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029163953506.png)

![image-20211029164006276](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164006276.png)

![image-20211029164024751](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164024751.png)

![image-20211029164037222](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164037222.png)

![image-20211029164052871](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164052871.png)

![image-20211029164101271](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164101271.png)

![image-20211029164131483](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164131483.png)

![image-20211029164136555](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164136555.png)

![image-20211029164145798](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164145798.png)

![image-20211029164150616](/Kevin_Min/images/2021-10-28-tiny-python-project-chapter-11~21/image-20211029164150616.png)

