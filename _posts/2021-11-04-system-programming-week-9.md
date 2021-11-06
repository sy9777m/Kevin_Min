---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 9.
categories: [markdown]
title: System Programming week 9
---
# System Programming week 9

## Program optimization

### Performance realities

There's more to performance than asymptotic complexity.

Constant factors matter too!

-   Easily see 10:1 performance range depending on how code is written.
-   Must optimize at multiple levels:
    -   algorithm, data representations, procedures, and loops

![image-20211104124636896](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104124636896.png)

### Optimizing compiler

Provide efficient mapping of program to machine

-   register allocation
-   code selection and ordering (scheduling)
-   dead code elimination
-   eliminating minor inefficiencies

Don't (usually) improve asymptotic efficiency

-   up to programmer to select best overall algorithm
-   big-O savings are (often) more important than constant factors
    -   but constant factors also matter

Have difficulty overcoming "optimization blockers"

-   potential memory aliasing
-   potential procedure side-effects

### Limitations of optimizing compilers

operate under fundamental constraint

-   Must not cause any change in program behavior
    -   except, possibly when program making use of nonstandard language features
-   often prevents it from making optimizations that would only affect behavior under pathological conditions.

Behavior that may be obvious to the programmer can be obfuscated by language and coding styles

Most analysis is performed only within procedures

-   whole-program analysis is too expensive in most cases
-   Newer versions of GCC do interprocedural analysis within individual files.
    -   but, not between code in different files

most analysis is based only on static information

-   compiler has difficult anticipating run-time inputs.

When in doubt, the compiler must be conservative.

### Generally useful optimization

optimizations that you or the compiler should do regardless of processor / compiler

![image-20211104125409736](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104125409736.png)

![image-20211104125507441](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104125507441.png)

### Reduction in strength

Replace costly operation with simpler one

Shift, add instead of multiply or divide

![image-20211104125538581](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104125538581.png)

## Share common subexpressions

Reuse portions of expressions

GCC will do this with `-O1`

![image-20211104125955469](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104125955469.png)

## Optimization Blocker #1: Memory aliasing

![image-20211104130102398](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104130102398.png)

![image-20211104130109095](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104130109095.png)

Aliasing

-   Two different memory references specify single location
-   Easy to have happen in C
    -   Since allowed to address arithmetic
    -   Direct access to storage structures
-   Get in habit of introducing local variables
    -   Accumulating within loops
    -   Your way of telling compiler not to check for aliasing

## Optimization Blocker #2: Procedure calls

![image-20211104130434564](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104130434564.png)

만약 function이 global state를 바꾸면 기대한 return이 아닐 수 있다.

![image-20211104130441996](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104130441996.png)

## Lower case conversion performance

![image-20211104130458892](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211104130458892.png)

## Convert Loop to goto form

![image-20211105040355474](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040355474.png)

## Calling Strlen

![image-20211105040446251](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040446251.png)

strlen은 굉장히 비싼 연산임. null로 끝날 때까지 찾아서 length를 계산하기 때문.

## Improving performance

![image-20211105040452997](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040452997.png)

## Lower case conversion performance

![image-20211105040509578](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040509578.png)

## Optimization Blocker #2: Procedure calls

![image-20211105040532095](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040532095.png)

## Optimization example: vector accumul.

![image-20211105040705243](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040705243.png)

## Benchmark computation

![image-20211105040859420](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040859420.png)

![image-20211105040934355](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105040934355.png)

## Basic optimizations

![image-20211105041021277](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105041021277.png)

![image-20211105042331170](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105042331170.png)

## Effect of basic optimizations

![image-20211105042339362](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105042339362.png)

## Modern CPU design

![image-20211105042421627](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105042421627.png)

## Superscalar processor

![image-20211105042705329](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105042705329.png)

## Pipelined functional units

![image-20211105042819389](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105042819389.png)

## Haswell CPU

![image-20211105043032830](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043032830.png)

## Loop unrolling (2 x 1)

![image-20211105043057963](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043057963.png)

superscalar processor의 특징을 활용한 optimization

## Effect of loop unrolling

![image-20211105043230620](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043230620.png)

## Loop unrolling with reassociation (2x1a)

![image-20211105043335484](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043335484.png)

## Effect of reassociation

![image-20211105043400630](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043400630.png)

## Reassociated computation

![image-20211105043604627](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043604627.png)

## Getting high performance

![image-20211105043610158](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043610158.png)

## Cycles per element (CPE)

![image-20211105043624140](/Kevin_Min/images/2021-11-04-system-programming-week-9/image-20211105043624140.png)

