---
toc: true
layout: post
description: Soongsil University 2-2 System Programming 5th week.
categories: [markdown]
title: System Programming week 5
---
# System Programming Week 5

## Control: Condition codes

## Processor State

![image-20210930170733781](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930170733781.png)

## Condition Codes (Implicit Setting)

### Single bit register

`addq Src, Dest`

`t = a + b`

-   CF (Carry Flag) for unsigned
    -   CF set if carry out from most significant bit (unsigned overflow, 비트연산으로 인해 most significant bit의 overflow가 일어났을 때)
-   ZF (Zero Flag)
    -   ZF set if `t == 0`
-   SF (Sign Flag) for signed
    -   SF set if `t < 0` (as signed)
-   OF (Overflow Flag) for signed
    -   set if two's-complement (signed) overflow: `(a > 0 && b > 0 && t < 0) || (a < 0 && b < 0 && t  >= 0)`

Not set by `leaq` instruction

## Condition codes (Explicit Setting by Compare Instruction)

`cmpq Src2, Src1`

`cmpq b, a` like computing a - b without setting destination. (빼기 연산으로 compare 연산을 함)

-   CF set if carry out from most significant bit (used for unsigned comparisions)
-   ZF set if `a == b`
-   SF set if `(a - b) < 0` (as signed)
-   OF set if two's-complement (signed) overflow `(a > 0 && b < 0 && (a - b) < 0) || (a < 0 && b < 0 && (a - b) >=0)`

## Condition Codes (Explicit Setting: Test)

### Explicit Setting by Test instruction

`testq Src2, Src1`

-   `testq b, a` like computing `a & b` without setting destination.
    -   bit by bit으로 comparison 연산
-   Sets condition codes based on value of Src1 & Src2
-   Useful to have one of the operands be a mask
-   ZF set when `a & b == 0`
-   SF set when `a & b < 0`

## Reading condition codes

![image-20210930172123796](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930172123796.png)

![image-20210930172302038](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930172302038.png)

![image-20210930172404709](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930172404709.png)

## Condition branches

## Jumping

jX Instructions - jump to different part of code depending on condition codes

![image-20210930172738658](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930172738658.png)

![image-20210930172901805](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930172901805.png)

## Expressing with Goto Code

C allows `goto` statement

Jump to position designated by label.

![image-20210930173048877](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930173048877.png)

![image-20210930173152631](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930173152631.png)

## Using conditional moves

### Conditional move instructions

-   instruction supports: if (Test) Dest <- Src
-   GCC tries to use them
    -   but, only when known to be safe.
-   Branch의 모든 계산을 다 끝내놓고, 조건에 맞는 결과만 가져와서 씀

### Why?

-   Branches are very disruptive to instruction flow through pipelines.
-   Conditional moves do not require control transfers.

![image-20210930173601313](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930173601313.png)

![image-20210930173718105](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930173718105.png)

## Bad cases for conditional move

![image-20210930173841921](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930173841921.png)

## Loops

## "Do-While" Loop example

![image-20210930174209931](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174209931.png)

Do-While statement가 assembly에서 가장 직관적으로 변환됨

![image-20210930174459270](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174459270.png)

## "Do-While" translation

![image-20210930174738332](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174738332.png)

## "While" translation

![image-20210930174805078](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174805078.png)

`-Og`는 optimization을 끄는 것

![image-20210930174900564](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174900564.png)

![image-20210930174936578](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174936578.png)

![image-20210930174949988](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930174949988.png)

## "For" loop form

![image-20210930175111562](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175111562.png)

![image-20210930175427826](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175427826.png)

![image-20210930175439525](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175439525.png)

![image-20210930175457916](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175457916.png)

## Switch statement

왜 if statement보다 switch statement가 더 성능이 좋은지 이해하기

### Switch statement example

![image-20210930175632717](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175632717.png)

### Jump table structure

![image-20210930175743399](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175743399.png)

Jump table을 작성해서 argument가 들어오자 마자 조건에 맞는 Code block으로 바로 jump 할 수 있는 code block의 address를 저장하고 있는 jump table을 활용함. -> 계산을 하지 않아도 됨

if statement로 many cases를 사용하면 하나하나 conditions들을 연산해야 하기 때문에 switch statement가 더 빠름

### Switch statement example

![image-20210930175957830](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930175957830.png)

![image-20210930180142350](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180142350.png)

## Assembly setup explanation

![image-20210930180235632](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180235632.png)

### Table structure

-   Each targe requires 8 bytes
-   Base address `.L4`

### Jumping

-   Direct: jmp `.L8`
-   Jump target is denoted by label `.L8`
-   Indirect: jmp `*.L4(, %rdi, 8)`
-   Must scale by factor of 8 (addresses are 8 bytes)
-   Fetch target from effective Address `.L4 + x * 8`
    -   only for $0<=x<=6$

![image-20210930180427390](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180427390.png)

### Code blocks (`x == 1`)

![image-20210930180437329](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180437329.png)

### Handling Fall-through

![image-20210930180520109](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180520109.png)

### Code blocks (`x == 2, x == 3`)

![image-20210930180714933](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180714933.png)

### Code blocks (`x == 5, x == 6, default`)

![image-20210930180748232](/Kevin_Min/images/2021-09-30-system-programming-week-5/image-20210930180748232.png)
