---
toc: true
layout: post
description: Soongsil University 2-2 System Programming 6th week.
categories: [markdown]
title: System Programming week 6
---
# System Programming Week 6

## Backward comparability

새로운 기술을 개발할 때 이전 기술과도 잘 동작하도록 설계하는 특성

## CISC architecture

Complex

## ISA

Instruction set of Architecture

## Information flowing through CPU and memory

Address, Data, Instruction

Condition code - Status를 표시해주는 코드

## Mechanisms in procedures

Passing control

-   to beginning of procedure code
-   back to return point

Passing data

-   Procedure arguments
-   return value

Memory management

-   Allocate during procedure execution
-   deallocate upon return

Mechanisms all implemented with machine instructions

x86-64 implementation of a procedure uses only those mechanisms required.

![image-20211008085851743](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008085851743.png)

## x86-64 Stack

Region of memory managed with stack discipline

Grows toward lower addresses

Register %rsp contains lowest stack address

-   address of top element

![image-20211008085944955](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008085944955.png)

stack pointer는 stack의 끝을 나타내는 pointer

stack은 위에서부터 아래로 쌓이고, heap은 아래에서부터 위로 쌓는다

![image-20211008090441015](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008090441015.png)

![image-20211008090447952](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008090447952.png)

![image-20211008090455907](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008090455907.png)

![image-20211008090506338](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008090506338.png)

## Procedure control flow

Use stack to support procedure call and return

Procedure call: `call label`

-   Push return address on stack
-   Jump to label

Return address:

-   Address of the next instruction right after call

Procedure return: `ret`

-   pop address from stack
-   jump to address

![image-20211008090731399](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008090731399.png)

![image-20211008090817579](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008090817579.png)

![image-20211008091002521](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091002521.png)

![image-20211008091011760](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091011760.png)

![image-20211008091019865](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091019865.png)

## Procedure data flow

![image-20211008091033753](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091033753.png)

![image-20211008091223043](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091223043.png)

## Stack-based languages

![image-20211008091240033](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091240033.png)

![image-20211008091429536](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091429536.png)

### Call chain example

![image-20211008091647636](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008091647636.png)

## Stack Frame

Content

-   Return information
-   Local storage (if needed)
-   Temporary space (if needed)

![image-20211008152722723](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152722723.png)

Management

-   Space allocated when enter procedure
    -   set-up code
    -   includes push by `call` instruction
-   Deallocated when return
    -   Finish code
    -   Includes pop by `ret` instruction

![image-20211008152753528](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152753528.png)

일단 main에서 시작, yoo 호출

![image-20211008152759216](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152759216.png)

![image-20211008152815288](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152815288.png)

![image-20211008152820416](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152820416.png)

![image-20211008152827847](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152827847.png)

![image-20211008152835905](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152835905.png)

![image-20211008152840783](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152840783.png)

![image-20211008152845893](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152845893.png)

![image-20211008152850367](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152850367.png)

![image-20211008152854981](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152854981.png)

![image-20211008152900343](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152900343.png)

## x86-64 / Linux Stack Frame

![image-20211008152943633](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008152943633.png)

Current Stack Frame (Top to Bottom)

-   Argument build - Parameters for function about to call
-   Local variables if can't keep in registers
-   Saved register context
-   Old frame pointer (optional)

Caller Stack Frame

-   Return address
    -   pushed by `call` instruction
-   Arguments for this call

![image-20211008153204164](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153204164.png)

![image-20211008153315722](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153315722.png)

![image-20211008153325561](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153325561.png)

![image-20211008153405751](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153405751.png)

![image-20211008153413906](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153413906.png)

![image-20211008153421612](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153421612.png)

## Register Saving Conventions

![image-20211008153603592](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153603592.png)

CPU내의 register들은 일종의 공유하는 책상 느낌. 내가 쓰다가 남이 쓰면 데이터가 날아갈 수 있는데, 이 데이터를 다른데 보관해둬야 함. 그런데 매번 책상의 모든 데이터를 다 옮기는 것은 불편하니까, 레지스터의 일부는 저장용도로 남겨두는 것.

![image-20211008153715346](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153715346.png)

경우에 따라 달라서 뭐가 더 좋은지에 대한 구분이 힘듦

![image-20211008153839239](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153839239.png)

![image-20211008153957750](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008153957750.png)

![image-20211008154055255](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154055255.png)

![image-20211008154104800](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154104800.png)

## Recursive function

![image-20211008154154471](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154154471.png)

![image-20211008154219682](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154219682.png)

![image-20211008154335199](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154335199.png)

![image-20211008154402627](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154402627.png)

![image-20211008154409542](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154409542.png)

![image-20211008154423654](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154423654.png)

## Observations about recursion

![image-20211008154442628](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154442628.png)

## x86-64 Procedure summary

![image-20211008154506229](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154506229.png)

## Array Allocation

![image-20211008154733853](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154733853.png)

![image-20211008154834886](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008154834886.png)

![image-20211008155015980](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155015980.png)

![image-20211008155119244](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155119244.png)

`movl (base, index, scale), Dest`

![image-20211008155227757](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155227757.png)

## Multidimensional (Nested) Arrays

![image-20211008155356930](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155356930.png)

![image-20211008155434657](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155434657.png)

## Nested Array Row Access

![image-20211008155511418](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155511418.png)

![image-20211008155544301](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155544301.png)

## Nested Array Element Access

![image-20211008155707066](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155707066.png)

![image-20211008155715792](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155715792.png)

## Multi-level array example

![image-20211008155829959](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155829959.png)

![image-20211008155842362](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008155842362.png)

![image-20211008160001130](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008160001130.png)

## N * M Matrix Code

![image-20211008160031292](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008160031292.png)

## Structure Representation

![image-20211008160507000](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008160507000.png)

![image-20211008160606843](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008160606843.png)

## Structures & Alignment

![image-20211008161026504](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161026504.png)

## Alignment principles

![image-20211008161101826](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161101826.png)

![image-20211008161251491](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161251491.png)

## Satisfying alignment with structures

![image-20211008161301869](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161301869.png)

## Meeting overall alignment requirement

![image-20211008161332164](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161332164.png)

## Array of structures

![image-20211008161401910](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161401910.png)

## Accessing array elements

![image-20211008161436606](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161436606.png)

## Saving space

![image-20211008161600410](/Kevin_Min/images/2021-10-06-system-programming-week-6/image-20211008161600410.png)

