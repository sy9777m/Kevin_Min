---
toc: true
layout: post
description: Soongsil University 2-2 Digital System Circuits week 9.
categories: [markdown]
title: Digital System Circuits week 9
---
# Digital System Circuits week 9

## Storing one bit-flip-flop example requiring bit storage

![image-20211106052440812](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106052440812.png)

## First attempt at bit storage

![image-20211106053105389](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106053105389.png)

feedback은 안정하거나, 진동하는 결과 2개를 가진다.

![image-20211106053518574](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106053518574.png)

짝수 inverter - 중간에서 일정한 값을 계속 추출 할 수 있음 / 홀수 inverter - 오실레이터, 진동

or gate는 1 bit storage를 만들 수 있음 / and gate는 1회용 bit storage를 만들 수 있음

## Bit storage using an SR latch

![image-20211106054204566](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106054204566.png)

cross coupled NOR gates

둘 다 1인 상태만 피하면 됨

![image-20211106054213870](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106054213870.png)

## Verilog module

![image-20211106063404373](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106063404373.png)

## Declaring a module

![image-20211106063346175](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106063346175.png)

## Good HDL "self comments"

![image-20211106063510324](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106063510324.png)

## Declaring ports

![image-20211106063703927](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106063703927.png)

## Module styles

![image-20211106064317364](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106064317364.png)

Dataflow - RTL

## Structural

![image-20211106064327637](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106064327637.png)

## Structural example

![image-20211106064338310](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106064338310.png)

시간제한이 있다거나 하는 특별한 상황에서 사용

## RTL example

![image-20211106064350967](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106064350967.png)

논리식

## Behavioral example

![image-20211106064400540](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106064400540.png)

## FSM Review

![image-20211106064413101](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-9/image-20211106064413101.png)

