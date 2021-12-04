---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 12.
categories: [markdown]
title: System Programming week 12
---
# System Programming week 12

## Control flow

![image-20211205031612545](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205031612545.png)

executable object file은 disk에 있고, CPU는 단지 sequential하게 instruction을 실행할 뿐

## Altering the control flow

![image-20211205031623976](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205031623976.png)

program의 의지에 따라서 flow를 control하는 방법들이 있음 - jumps, branches, call, return

그러나 이런 방법 만으로는 제어에 한계가 있음 - system의 상태가 변해도 program을 여전히 제어 할 수 있어야 함

## Exceptional control flow

![image-20211205031636463](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205031636463.png)

![image-20211205032019933](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032019933.png)

## Exceptions

![image-20211205032204555](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032204555.png)

![image-20211205032213282](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032213282.png)

## Exception tables (interrupt vectors)

![image-20211205032338677](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032338677.png)

## Asynchronous exceptions (interrupts)

![image-20211205032409230](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032409230.png)

Exception은 일단 문제가 생긴 것, 일이 생긴거임 - 실행하는 일이랑 별로 상관없는 문제가 asynchronous exception

## Synchronous exceptions

![image-20211205032644309](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032644309.png)

![image-20211205032823075](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032823075.png)

traps - 의도적으로 system에 요청하는 것

faults - 뭘 잘못했는지 모르겠는데 system state를 바꾼 이벤트, architecture dependent함

abort - 누가봐도 심각한 오류

## System calls

![image-20211205032837793](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032837793.png)

## System call example: opening file

![image-20211205033030378](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033030378.png)

## Trap example: opening file

![image-20211205032659505](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205032659505.png)

## Fault example: page fault

![image-20211205033220557](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033220557.png)

## Fault example: invalid memory reference

![image-20211205033248878](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033248878.png)

## Exception table IA32 (Excerpt)

![image-20211205033406882](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033406882.png)

## Process

![image-20211205033416309](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033416309.png)

![image-20211205033430148](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033430148.png)

## Multiprocessing: the illusion

![image-20211205033632959](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033632959.png)

## Multiprocessing example

![image-20211205033700330](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033700330.png)

## Multiprocessing: the (traditional) reality

![image-20211205033729557](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033729557.png)

![image-20211205033940070](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033940070.png)

![image-20211205033945862](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033945862.png)

![image-20211205033953376](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205033953376.png)

## Concurrent processes

![image-20211205034038132](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034038132.png)

![image-20211205034044931](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034044931.png)

## User view of concurrent processes

![image-20211205034150488](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034150488.png)

## Context switching

![image-20211205034207252](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034207252.png)

![image-20211205034220350](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034220350.png)

## System call error handling

![image-20211205034316526](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034316526.png)

## Error-reporting functions

![image-20211205034451144](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034451144.png)

## Error-handling wrappers

![image-20211205034509632](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034509632.png)

## Obtaining process IDs

![image-20211205034525676](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034525676.png)

## Creating and terminating processes

![image-20211205034555870](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034555870.png)

## Terminating processes

![image-20211205034648743](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034648743.png)

## Creating processes

![image-20211205034845599](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205034845599.png)

shell도 하나의 program

## fork example

![image-20211205035111223](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035111223.png)

---

안 봐도 되지만

## Modeling fork with process graph

![image-20211205035332355](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035332355.png)

## Process graph example

![image-20211205035344789](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035344789.png)

## Interpreting process graphs

![image-20211205035405638](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035405638.png)

## fork example: nested forks in parent

![image-20211205035428141](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035428141.png)

---

## Reaping child processes

![image-20211205035444942](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035444942.png)

## Non-terminating child example

![image-20211205035702885](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035702885.png)

## Zombie example

![image-20211205035815615](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035815615.png)

## wait: synchronizing with children

![image-20211205035835451](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035835451.png)

## Another wait example

![image-20211205035930309](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205035930309.png)

## waitpid: waiting for a specific process

![image-20211205040012770](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205040012770.png)

## execve: loading and running programs

![image-20211205040101087](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205040101087.png)

## structure of the stack when a new program starts

![image-20211205040238974](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205040238974.png)

## execve example

![image-20211205040623546](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205040623546.png)

## summary

![image-20211205040608857](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205040608857.png)

![image-20211205040824049](/Kevin_Min/images/2021-12-05-system-programming-week-12/image-20211205040824049.png)
