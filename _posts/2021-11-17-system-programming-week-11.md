---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 11.
categories: [markdown]
title: System Programming week 11
---
# System Programming week 11

## Example C Program

![image-20211117132356697](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132356697.png)

## Static Linking

![image-20211117132408746](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132408746.png)

object file은 machine level까지 complie되었지만, 아직 executable file은 아닌 상황

## Why Linkers?

![image-20211117132521952](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132521952.png)

![image-20211117132527826](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132527826.png)

## What do Linkers do?

![image-20211117132540562](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132540562.png)

각종 symbol들의 위치를 결정하는 과정을 symbol resolution이라고 함

linker가 symbol resolution을 할 때, 각 symbol은 딱 하나만 있어야 함 -> 여러개가 있는 경우 error

![image-20211117132548432](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132548432.png)

executable file을 만들 때, 각 symbol의 위치는 virtual address

code는 code끼리, data는 data끼리 모아서 merge

## Three kinds of object files (modules)

![image-20211117132604418](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132604418.png)

machine language로 바뀌면 일단 전부 object file

Shared object file - dynamic하게 linking되고, 실행될 때 memory로 load됨

## Executable and linkable format (ELF)

![image-20211117132620767](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132620767.png)

하나의 format을 가지고 여러개의 object file을 모두 지원해야 함

## ELF object file format

![image-20211117132636156](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132636156.png)

![image-20211117132648282](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132648282.png)

## Linker symbols

![image-20211117132700684](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117132700684.png)

local symbol로 사용하고자 한다면 이름이 겹치는 symbol 앞에 static이라고 붙이면 된다. 그러면 exclusive하게 해당 module 내에서만 사용된다. 외부에서 사용이 불가능.

local linker symbol은 local program variable과는 다름

## Symbol resolution

![image-20211117140234769](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140234769.png)

## Local symbol

![image-20211117140244731](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140244731.png)

## How linker resolves duplicate symbol definitions

![image-20211117140300313](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140300313.png)

## Linker's symbol rules

![image-20211117140311113](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140311113.png)

## Linker puzzles

![image-20211117140320861](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140320861.png)

## Example

![image-20211117140924815](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140924815.png)

![image-20211117140933277](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140933277.png)

![image-20211117140940976](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140940976.png)

![image-20211117140953639](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117140953639.png)

![image-20211117141046856](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117141046856.png)

## Global varaibles

![image-20211117141057132](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117141057132.png)

## Relocation

![image-20211117141107247](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117141107247.png)

## Relocation entries

![image-20211117142256520](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117142256520.png)

## Relocated .text section

![image-20211117142311040](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117142311040.png)

## Loading Executable object files

![image-20211117142445376](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117142445376.png)

## Packaging commonly used functions

![image-20211117142931293](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117142931293.png)

## Old-fashioned solution: static libraries

![image-20211117143311349](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143311349.png)

## Creating static libraries

![image-20211117143322683](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143322683.png)

## Commonly used libraries

![image-20211117143333799](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143333799.png)

## Linking with static libraries

![image-20211117143349136](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143349136.png)

![image-20211117143750075](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143750075.png)

## Using static libraries

![image-20211117143800698](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143800698.png)

![image-20211117143831338](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117143831338.png)

## Modern solution: shared libraries

![image-20211117144259279](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144259279.png)

![image-20211117144309121](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144309121.png)

## Dynamic linking at load-time

![image-20211117144323427](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144323427.png)

## Dynamic linking at run-time

![image-20211117144732217](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144732217.png)

![image-20211117144804414](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144804414.png)

![image-20211117144814265](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144814265.png)

## Linking summary

![image-20211117144910902](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117144910902.png)

## Control flow

![image-20211117145052736](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117145052736.png)

## Altering the control flow

![image-20211117145104441](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117145104441.png)

## Exceptional control flow

![image-20211117145432982](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117145432982.png)

![image-20211117145517364](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117145517364.png)

## Exception

![image-20211117145442495](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117145442495.png)

## Interrupt vectors

![image-20211117145457838](/Kevin_Min/images/2021-11-17-system-programming-week-11/image-20211117145457838.png)

