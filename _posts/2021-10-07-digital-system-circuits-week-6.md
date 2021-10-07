---
toc: true
layout: post
description: Soongsil University 2-2 Digital System Circuits 6th week.
categories: [markdown]
title: Digital System Circuits week 6
---
# Digital System Circuits Week 6

![image-20211007131425282](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007131425282.png)

![image-20211007131434954](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007131434954.png)

![image-20211007131536125](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007131536125.png)

![image-20211007131654062](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007131654062.png)

## Completeness of NAND

![image-20211007131705582](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007131705582.png)

## Number of possible boolean functions

![image-20211007132127367](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007132127367.png)

## Decoders

![image-20211007132235512](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007132235512.png)

![image-20211007132708963](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007132708963.png)

## Multiplexor (Mux)

![image-20211007132821767](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007132821767.png)

![image-20211007132951199](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007132951199.png)

![image-20211007133116999](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007133116999.png)

Decoder: Code -> Signal / Encoder: Signal -> Code

Mux

![image-20211007133339738](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007133339738.png)

Demux

![image-20211007133402448](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007133402448.png)

Mux / Demux는 회선의 방향을 결정할 뿐, 0과 1의 결정에는 관여하지 않는다. 어디로 출력이 나갈지, 어디로 입력을 받을지 결정하는 것.

### Muxes commonly together - N-bit Mux

![image-20211007133723156](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007133723156.png)

![image-20211007133843501](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007133843501.png)

![image-20211007134315165](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007134315165.png)

## Critical delay and critical path

![image-20211007134739202](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007134739202.png)

## Active low inputs

![image-20211007134942656](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007134942656.png)

## Schematic capture and simulation

![image-20211007135105884](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211007135105884.png)

## Introduction to optimization of digital logic design

How can we build better circuits?

-   Delay - the time from input changing to new correct stable output
-   Size - the number of transistors

![image-20211008024400694](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008024400694.png)

![image-20211008024412197](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008024412197.png)

transistor 갯수는 입력 당 2개 생각하면 됨

## Tradeoff

Improves some, but worsens other, criteria of interest

![image-20211008024628036](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008024628036.png)

Optimization은 해야 하는 것, Tradeoff는 선택의 문제

## Optimization and Trade off

Optimizations

-   All criteria of interest are improved (or at least kept the same)

Tradeoff

-   Some criteria of interest are improved, while others are worsened.

We obviously prefer optimizations, but often must accept tradeoffs.

-   You can't build a car that is the most comfortable and has the best fuel efficiency, and is the fastest - you have to give up something to gain other things.

# Combinational logic optimization and tradeoffs

![image-20211008025056715](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008025056715.png)

![image-20211008025218642](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008025218642.png)

보통 sum-of-products로 주어지는 회로는 two-level size라서 delay는 일정해서 transistor를 줄이는 방향으로 optimization을 한다.

## Algebraic two-level size optimization

![image-20211008025347002](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008025347002.png)

## Karnaugh maps for two-level size optimization

Karnaugh maps (K-maps)

![image-20211008025721847](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008025721847.png)

K-map에서 인접한 11은 줄일 수 있다는 의미

# Digital design process

![image-20211008031116729](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008031116729.png)

## What is an HDL?

![image-20211008032320925](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008032320925.png)

It looks like a programming language but not a programming language.

-   It is always critical to recall you are describing hardware.
-   This code's primary purpose is to generate hardware.
-   The hardware this code describes (a counter) can be simulated on a computer. In this secondary use of the language it does act more like a programming language.

## Simulating / Validating HDL

![image-20211008032329562](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008032329562.png)

## What is synthesis?

-   Takes a description of what a circuit does
-   Creates the hardware to do it

![image-20211008032546838](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008032546838.png)

## Synthesizing the hardware described

-   All hardware created during synthesis
    -   Even if a is true, still computing d&c
-   learn to understand how descriptions are translated to hardware

![image-20211008032827627](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008032827627.png)

## Why use an HDL?

Enables larger designs via rich syntax, modularity

-   more abstract than schematics, allows larger designs
    -   register transfer level description
    -   wide datapaths (16, 32, or 64 bits wide) can be abstracted to a single vecotr
    -   synthesis tool does the bulk of the tedious repetitive work vs schematic capture

Portable design

-   Behavioral or dataflow Verilog can be synthesized to a new process library with little effort

![image-20211008033148367](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008033148367.png)

![image-20211008033334873](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008033334873.png)

# Homework

## Week 5

![image-20211008034552330](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034552330.png)

![image-20211008034606282](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034606282.png)

![image-20211008034615692](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034615692.png)

![image-20211008034623776](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034623776.png)

![image-20211008034630789](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034630789.png)

![image-20211008034638331](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034638331.png)

![image-20211008034644713](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034644713.png)

## Week 6

![image-20211008034716106](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034716106.png)

![image-20211008034722899](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034722899.png)

![image-20211008034735938](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034735938.png)

![image-20211008041829289](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008041829289.png)

![image-20211008034747145](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034747145.png)

![image-20211008034754012](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034754012.png)

![image-20211008034801316](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034801316.png)

![image-20211008034811025](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034811025.png)

![image-20211008044410708](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008044410708.png)

![image-20211008034817913](/Kevin_Min/images/2021-10-07-digital-system-circuits-week-6/image-20211008034817913.png)

