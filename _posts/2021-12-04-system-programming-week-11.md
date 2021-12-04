---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 11.
categories: [markdown]
title: System Programming week 11
---
# System Programming week 11

## Linking

여러 소스파일에 코드를 작성해서 프로그램 하나를 작성하게 되는데, 여러 파일을 합쳐주는 역할

## Example C Program

![image-20211204192625609](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204192625609.png)

## Static linking

![image-20211204192708349](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204192708349.png)

별도의 object file로 일단 컴파일, linker로 연결해서 하나의 executable file로 만듦

gcc는 compiler, optimizer, linker가 다 합쳐진 무언가라고 생각하면 됨

object file은 machine level language지만, executable하지는 않음

## Why linkers?

![image-20211204192851729](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204192851729.png)

![image-20211204193044469](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204193044469.png)

## What do linkers do?

![image-20211204193225173](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204193225173.png)

![image-20211204193234653](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204193234653.png)

memory <-> storage가 있음

storage에 작성한 source code들이 있고, 이를 활용해서 executable file을 만들어서 실행하면 해당 코드가 memory로 올라간다.

실행파일은 어디서 뭘 해야하는지 address가 다 적혀있다. - symbol이 아니라 address로 function을 호출

그런데 이 address가 virtual address임

-   예전에는 프로그램이 1개만 실행됨
-   그런데 최근에는 많은 프로그램이 동시에 실행되는데, virtual address space 덕분임
    -   언제 어떤 메모리에 올라갈지 모르겠지만, address를 virtual address space에 입력해둠
-   그래서 executable file은 virtual address를 기준으로 작성됨

## Three kinds of object files (modules)

![image-20211204194156251](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204194156251.png)

## Executable and linkable format (ELF)

![image-20211204194405029](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204194405029.png)

## ELF object file format

![image-20211204194422403](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204194422403.png)

![image-20211204194644393](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204194644393.png)

## Linker symbols

![image-20211204194901990](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204194901990.png)

## Symbol resolution

![image-20211204195203815](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195203815.png)

## Local symbol

![image-20211204195340780](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195340780.png)

## How linker resolves duplicate symbol definitions

![image-20211204195523378](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195523378.png)

## Examples

![image-20211204195621051](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195621051.png)

strong symbol 2개 선언 -> compile error (multiple definition)

![image-20211204195629237](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195629237.png)

strong symbol 2개 선언 -> compile error (multiple definition)

![image-20211204195638979](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195638979.png)

weak type global variable < strong type global variable: symbol resolution은 strong type에게 일어난다.

![image-20211204195648876](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195648876.png)

둘 다 weak면, random으로 뭘 건드리게 될지 모른다.

![image-20211204195658726](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204195658726.png)

double은 8bytes, int는 4bytes인데, foo5.c에서는 둘 다 strong으로 선언되어 있기 때문에 bar5.c에서 weak로 선언된 x에 -0.0을 넣으면 strong x에 접근하게 되서 다른 메모리 공간을 침범하게 됨

## Global variables

![image-20211204200217464](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200217464.png)

## Linker's symbol rules

![image-20211204200251181](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200251181.png)

## Linker puzzles

![image-20211204200345974](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200345974.png)

## Step 2: Relocation

![image-20211204200353973](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200353973.png)

## Relocation entries

![image-20211204200409981](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200409981.png)

## Relocated .text section

![image-20211204200536909](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200536909.png)

## Loading executable object files

![image-20211204200835179](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200835179.png)

## Packing commonly used functions

![image-20211204200928964](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211204200928964.png)

## Old-fashioned solution: static library

![image-20211205025733688](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205025733688.png)

linking time에 합쳐져서 executable file에 함께 들어가는 object flies

## Creating static libraries

![image-20211205025958072](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205025958072.png)

## Commonly used libraries

![image-20211205030055092](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030055092.png)

## Linking with static libraries

![image-20211205030144119](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030144119.png)

![image-20211205030156445](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030156445.png)

## Using static libraries

![image-20211205030243106](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030243106.png)

![image-20211205030257834](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030257834.png)

-L. <- 현재 directory에 libfun이 있는지 찾도록

-lmine <- archive에서 찾도록

순서만 바꿨더니 undefined reference error가 뜸 - linker는 command line order로 scan을 하게 됨

그래서 -lmine에서 먼저 resolution을 검사하고 libtest.o를 검사하게되니 undefined reference error가 발생하게 된 것

## Modern solution: shared libraries

![image-20211205030716879](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030716879.png)

dynamic link library - linking time에 library를 합치는 것이 아니라 load time에 dynamic하게 연동되는 library

![image-20211205030854708](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205030854708.png)

## Dynamic linking at load-time

![image-20211205031059780](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205031059780.png)

## Dynamic linking at run-time

![image-20211205031115640](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205031115640.png)

![image-20211205031220986](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205031220986.png)

![image-20211205031230567](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205031230567.png)

## Linking summary

![image-20211205031323720](/Kevin_Min/images/2021-12-04-system-programming-week-11/image-20211205031323720.png)
