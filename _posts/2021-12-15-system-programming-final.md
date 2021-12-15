---
toc: true
layout: post
description: Soongsil University 2-2 System Programming final summary.
categories: [markdown]
title: System Programming final
---
# System Programming final

## Optimization

### Performance realities

![image-20211215144546753](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215144546753.png)

### Optimizing compilers

![image-20211215144725841](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215144725841.png)

### Limitations of optimizing compilers

![image-20211215144905925](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215144905925.png)

![image-20211215144849316](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215144849316.png)

### Optimization blocker #1: Memory Aliasing

![image-20211215145343566](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145343566.png)

![image-20211215145419970](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145419970.png)

![image-20211215145428740](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145428740.png)

### Optimization blocker #2: Procedure calls

![image-20211215145508439](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145508439.png)

![image-20211215145725188](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145725188.png)

![image-20211215145752636](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145752636.png)

![image-20211215145800308](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145800308.png)

### Modern CPU design

![image-20211215145928096](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215145928096.png)

### Superscalar processor

![image-20211215150002279](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150002279.png)

### Getting high performance

![image-20211215150346399](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150346399.png)

## Memory hierarchy

### Random-access memory (RAM)

![image-20211215150432950](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150432950.png)

![image-20211215150509856](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150509856.png)

### Nonvolatile memories

![image-20211215150522743](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150522743.png)

### Traditional bus structure connecting CPU and memory

![image-20211215150642886](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150642886.png)

### Memory read/write transaction

![image-20211215150703490](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150703490.png)

![image-20211215150711785](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150711785.png)

![image-20211215150722569](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150722569.png)

![image-20211215150728435](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150728435.png)

![image-20211215150744275](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150744275.png)

![image-20211215150800301](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150800301.png)

### What's inside a disk drive?

![image-20211215150824606](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150824606.png)

### Disk geometry

![image-20211215150844651](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150844651.png)

![image-20211215150906394](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150906394.png)

### Disk capacity

![image-20211215150917218](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215150917218.png)

### Recording zones

![image-20211215151054065](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151054065.png)

### Computing disk capacity

![image-20211215151122100](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151122100.png)

### Disk operation

![image-20211215151150203](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151150203.png)

![image-20211215151200424](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151200424.png)

### Disk structure

![image-20211215151225591](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151225591.png)

### Disk access

![image-20211215151236801](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151236801.png)

![image-20211215151244304](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151244304.png)

![image-20211215151251903](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151251903.png)

![image-20211215151259432](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151259432.png)

![image-20211215151306641](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151306641.png)

![image-20211215151311831](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151311831.png)

![image-20211215151318227](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151318227.png)

![image-20211215151326242](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151326242.png)

![image-20211215151332263](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151332263.png)

### Disk access time

![image-20211215151349882](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151349882.png)

![image-20211215151400304](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151400304.png)

### Logical disk blocks

![image-20211215151431642](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151431642.png)

### I/O bus

![image-20211215151530662](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151530662.png)

### Reading a disk sector

![image-20211215151613808](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151613808.png)

![image-20211215151624855](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151624855.png)

![image-20211215151638756](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151638756.png)

### Solid state disks (SSD)

![image-20211215151655459](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151655459.png)

### SSD performance characteristics

![image-20211215151749406](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151749406.png)

### SSD tradeoffs vs rotating disks

![image-20211215151818028](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151818028.png)

### The CPU-Memory gap

![image-20211215151840596](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151840596.png)

### Locality

![image-20211215151901313](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151901313.png)

Temporal locality - 썼던 거 또 쓸 가능성이 높다.

Spatial locality - 썼던거에서 가까운 것을 쓸 가능성이 높다.

![image-20211215151944282](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215151944282.png)

### Qualitative estimates of locality

![image-20211215152006223](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152006223.png)

![image-20211215152033194](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152033194.png)

### Memory hierarchies

![image-20211215152130353](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152130353.png)

![image-20211215152226080](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152226080.png)

![image-20211215152628327](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152628327.png)

### Caches

![image-20211215152309457](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152309457.png)

### General cache concepts

![image-20211215152416373](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152416373.png)

#### General cache concepts: hit

![image-20211215152431250](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152431250.png)

#### General cache concepts: miss

![image-20211215152458178](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152458178.png)

### General caching concepts: types of cache misses

![image-20211215152535039](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152535039.png)

### Summary

![image-20211215152656484](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152656484.png)

## Linking

### Static linking

![image-20211215152720272](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152720272.png)

### Why linkers?

![image-20211215152745875](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152745875.png)

![image-20211215152756740](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152756740.png)

### What do linkers do?

![image-20211215152835897](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152835897.png)

![image-20211215152924412](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215152924412.png)

### Three kinds of object files (modules)

![image-20211215153018895](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153018895.png)

### Executable and linkable format (ELF)

![image-20211215153104282](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153104282.png)

### ELF object file format

![image-20211215153122082](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153122082.png)

![image-20211215153200856](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153200856.png)

### Linker symbols

![image-20211215153255564](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153255564.png)

### Steps: symbol resolution

![image-20211215153348934](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153348934.png)

### Local symbols

![image-20211215153417302](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153417302.png)

### How linker resolves duplicate symbol definitions

![image-20211215153738202](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153738202.png)

### Linker's symbol rules

![image-20211215153800893](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153800893.png)

### Linker puzzles

![image-20211215153830231](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153830231.png)

### Example

![image-20211215153922052](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153922052.png)

![image-20211215153931683](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153931683.png)

![image-20211215153950579](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215153950579.png)

![image-20211215154031403](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154031403.png)

![image-20211215154110354](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154110354.png)

### Global variables

![image-20211215154120087](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154120087.png)

### Steps: relocation

![image-20211215154136732](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154136732.png)

![image-20211215154146292](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154146292.png)

![image-20211215154155429](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154155429.png)

### Loading executable object files

![image-20211215154243945](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154243945.png)

### Packing commonly used functions

![image-20211215154339943](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154339943.png)

### Old-fashioned solution: static libraries

![image-20211215154418757](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154418757.png)

### Creating static libraries

![image-20211215154434218](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154434218.png)

### Commonly used libraries

![image-20211215154514939](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154514939.png)

### Linking with static libraries

![image-20211215154529866](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154529866.png)

![image-20211215154538381](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154538381.png)

### Using static libraries

![image-20211215154557361](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154557361.png)

![image-20211215154604985](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154604985.png)

### Modern solution: shared libraries

![image-20211215154719147](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154719147.png)

![image-20211215154808325](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154808325.png)

### Dynamic linking at load-time

![image-20211215154833477](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154833477.png)

### Dynamic linking at run-time

![image-20211215154858202](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154858202.png)

![image-20211215154907835](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154907835.png)

![image-20211215154915330](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154915330.png)

### Linking summary

![image-20211215154940892](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215154940892.png)

## Library interpositioning

![image-20211215155013329](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155013329.png)

### Some interpositioning applications

![image-20211215155034473](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155034473.png)

![image-20211215155125396](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155125396.png)

### Example program

![image-20211215155138897](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155138897.png)

### Compile-time interpositioning

![image-20211215155209787](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155209787.png)

![image-20211215155229263](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155229263.png)

### Link-time interpositioning

![image-20211215155305908](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155305908.png)

![image-20211215155318738](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155318738.png)

### Load/run-time interpositioning

![image-20211215155358628](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155358628.png)

![image-20211215155422889](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155422889.png)

![image-20211215155431503](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155431503.png)

### Interpositioning recap

![image-20211215155445470](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155445470.png)

## Exceptional control flow

### Control flow

![image-20211215155543089](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215155543089.png)

### Altering the control flow

![image-20211215161111328](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161111328.png)

### Exceptional control flow

![image-20211215161142036](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161142036.png)

### Exceptions

![image-20211215161250379](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161250379.png)

### Interrupt vectors

![image-20211215161310796](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161310796.png)

### Asynchronous exceptions (interrupts)

![image-20211215161355576](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161355576.png)

### Synchronous exceptions

![image-20211215161416413](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161416413.png)

Trap - 의도적

faults - 의도하지 않았으나 복구 가능

aborts - 의도하지 않았고 복구 불능

### Trap example: opening file

![image-20211215161442267](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161442267.png)

### Fault example: page fault

![image-20211215161523360](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161523360.png)

### Faults example: invalid memory reference

![image-20211215161625510](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161625510.png)

### Exception table IA32 (Excerpt)

![image-20211215161649703](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161649703.png)

## Processes

![image-20211215161709579](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161709579.png)

### concurrent processes

![image-20211215161745378](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161745378.png)

### User view of concurrent processes

![image-20211215161831969](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161831969.png)

### Context switching

![image-20211215161848037](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161848037.png)

### fork: creating new processes

![image-20211215161912373](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161912373.png)

![image-20211215161926846](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161926846.png)

![image-20211215161946170](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215161946170.png)

![image-20211215162011407](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162011407.png)

![image-20211215162028567](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162028567.png)

![image-20211215162054274](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162054274.png)

![image-20211215162103703](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162103703.png)

### exit: ending a process

![image-20211215162124672](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162124672.png)

### Zombies

![image-20211215162138337](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162138337.png)

![image-20211215162226222](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162226222.png)

![image-20211215162235277](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162235277.png)

### wait: synchronizing with children

![image-20211215162306110](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162306110.png)

![image-20211215162514724](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162514724.png)

![image-20211215162525382](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162525382.png)

### waitpid(): waiting for a specific process

![image-20211215162607207](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162607207.png)

### execve: loading and running programs

![image-20211215162638420](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162638420.png)

![image-20211215162717200](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162717200.png)

### Summary

![image-20211215162757271](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162757271.png)

![image-20211215162806878](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162806878.png)

## Exceptional control flow: signals

### The world of multitasking

![image-20211215162915346](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215162915346.png)

### Programmer's model of multitasking

![image-20211215163033847](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163033847.png)

### Unix process hierarchy

![image-20211215163108444](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163108444.png)

### Shell programs

![image-20211215163119120](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163119120.png)

### Simple shell eval function

![image-20211215163145993](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163145993.png)

### What is a background job?

![image-20211215163159317](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163159317.png)

### Problem with simple shell example

![image-20211215163213761](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163213761.png)

### ECF to the rescue!

![image-20211215163500474](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163500474.png)

## Signals

![image-20211215163537428](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163537428.png)

### Sending a signal

![image-20211215163615154](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163615154.png)

### Receiving a signal

![image-20211215163701451](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163701451.png)

### Pending and blocked signals

![image-20211215163738766](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215163738766.png)

### Signal concepts

![image-20211215164230478](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164230478.png)

### Process groups

![image-20211215164258124](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164258124.png)

### Sending signals with /bin/kill program

![image-20211215164328235](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164328235.png)

### Sending signals from the keyboard

![image-20211215164354351](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164354351.png)

### Receiving signals

![image-20211215164433765](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164433765.png)

### Default actions

![image-20211215164511607](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164511607.png)

### Installing signal handlers

![image-20211215164524338](/Kevin_Min/images/2021-12-15-system-programming-final/image-20211215164524338.png)
