---
toc: true
layout: post
description: Tiny Python Project Chapter 9 ~ 10 for Find-A.
categories: [markdown]
title: Tiny Python Project chapter 9 ~ 10
---
# Tiny Python Project Chapter 9 ~ 10

## Chapter 9. 저주의 전화: 단어목록에서 무작위 험담 만들기

![image-20211006195135195](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195135195.png)

![image-20211006195142583](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195142583.png)

![image-20211006195526288](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195526288.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@9c4e508fd6f6>
Date   : 2021-10-06
Purpose: Rock the Casbah
"""

import argparse


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Heap abuse',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-a',
                        '--adjectives',
                        help='Number of adjectives',
                        metavar='adjectives',
                        type=int,
                        default=2)

    parser.add_argument('-n',
                        '--number',
                        help='Number of insults',
                        metavar='insults',
                        type=int,
                        default=3)

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='seed',
                        type=int,
                        default=None)

    return parser.parse_args()


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211006195554974](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195554974.png)

![image-20211006195618918](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195618918.png)

![image-20211006195628839](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195628839.png)

![image-20211006195904804](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006195904804.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@9c4e508fd6f6>
Date   : 2021-10-06
Purpose: Rock the Casbah
"""

import argparse
import random


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Heap abuse',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-a',
                        '--adjectives',
                        help='Number of adjectives',
                        metavar='adjectives',
                        type=int,
                        default=2)

    parser.add_argument('-n',
                        '--number',
                        help='Number of insults',
                        metavar='insults',
                        type=int,
                        default=3)

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='seed',
                        type=int,
                        default=None)

    args = parser.parse_args()

    if args.adjectives < 1:
        parser.error(f'--adjectives "{args.adjectives}" must be > 0')
    
    if args.insults < 1:
        parser.error(f'--number "{args.insults}" must be > 0')

    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211006200901482](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006200901482.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@9c4e508fd6f6>
Date   : 2021-10-06
Purpose: Rock the Casbah
"""

import argparse
import random


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Heap abuse',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('-a',
                        '--adjectives',
                        help='Number of adjectives',
                        metavar='adjectives',
                        type=int,
                        default=2)

    parser.add_argument('-n',
                        '--number',
                        help='Number of insults',
                        metavar='insults',
                        type=int,
                        default=3)

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='seed',
                        type=int,
                        default=None)

    args = parser.parse_args()

    if args.adjectives < 1:
        parser.error(f'--adjectives "{args.adjectives}" must be > 0')
    elif args.number < 1:
        parser.error(f'--number "{args.number}" must be > 0')
    
    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    random.seed(args.seed)

    adjectives = 'bankrupt base caterwauling corrupt cullionly detestable dishonest false filthsome filthy foolish foul gross heedless indistinguishable infected insatiate irksome lascivious lecherous loathsome lubbery old peevish rascaly rotten ruinous scurilous scurvy slanderous sodden-witted thin-faced toad-spotted unmannered vile wall-eyed'.split()

    nouns = 'Judas Satan ape ass barbermonger beggar block boy braggart butt carbuncle coward coxcomb cur dandy degenerate fiend fishmonger fool gull harpy jack jolthead knave liar lunatic maw milksop minion ratcatcher recreant rogue scold slave swine traitor varlet villain worm'.split()

    num_adjs = args.adjectives
    repeat_num = args.number

    for i in range(repeat_num):
        selected_adjs = random.sample(adjectives, num_adjs)
        selected_noun = random.choice(nouns)
        print('You ' + ', '.join(selected_adjs) + ' {}!'.format(selected_noun))

# --------------------------------------------------
if __name__ == '__main__':
    main()

```

![image-20211006202153543](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202153543.png)

![image-20211006202206263](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202206263.png)

![image-20211006202222975](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202222975.png)

![image-20211006202300289](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202300289.png)

![image-20211006202325055](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202325055.png)

![image-20211006202347087](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202347087.png)

![image-20211006202416727](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202416727.png)

![image-20211006202435474](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202435474.png)

![image-20211006202442993](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202442993.png)

![image-20211006202450670](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202450670.png)

![image-20211006202458488](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006202458488.png)

## Chapter 10. 전화: 무작위로 문자열 변경하기

![image-20211006215241567](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006215241567.png)

![image-20211006220047127](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006220047127.png)

![image-20211006224257293](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224257293.png)

![image-20211006224409652](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224409652.png)

![image-20211006224437868](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224437868.png)

![image-20211006224512935](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224512935.png)

![image-20211006224647292](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224647292.png)

![image-20211006224656619](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224656619.png)

![image-20211006224705174](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006224705174.png)

```python
#!/usr/bin/env python3
"""
Author : runner <runner@d7a07f2f85b2>
Date   : 2021-10-06
Purpose: Rock the Casbah
"""

import string
import argparse
import random
import os


# --------------------------------------------------
def get_args():
    """Get command-line arguments"""

    parser = argparse.ArgumentParser(
        description='Telephone',
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)

    parser.add_argument('text',
                        metavar='str',
                        type=str,
                        help='Input text or file')

    parser.add_argument('-s',
                        '--seed',
                        help='Random seed',
                        metavar='seed',
                        type=int,
                        default=None)

    parser.add_argument('-m',
                        '--mutations',
                        help='Percent mutations',
                        metavar='mutations',
                        type=float,
                        default=0.1)

    args = parser.parse_args()

    if not (0 <= args.mutations <= 1 ):
        parser.error(f'--mutations "{args.mutations}" must be between 0 and 1')

    if os.path.isfile(args.text):
        args.text = open(args.text).read().rstrip()
    
    return args


# --------------------------------------------------
def main():
    """Make a jazz noise here"""

    args = get_args()
    random.seed(args.seed)
    t = args.text
    alpha = ''.join(sorted(string.ascii_letters + string.punctuation))
    t_len = len(t)
    num_mutations = round(t_len * args.mutations)
    new_text = t

    for i in random.sample(range(t_len), num_mutations):
        new_text = new_text[:i] + random.choice(alpha.replace(new_text[i], '')) + new_text[i + 1:]
    
    print(f'You said: "{t}"\nI heard : "{new_text}"')


# --------------------------------------------------
if __name__ == '__main__':
    main()
```

![image-20211006231938092](/Kevin_Min/images/2021-10-06-tiny-python-project-chapter-9~10/image-20211006231938092.png)

