---
toc: true
layout: post
description: Soongsil University 2-2 Digital System Circuits week 10.
categories: [markdown]
title: Digital System Circuits week 10
---
# Digital System Circuits week 10

## Example using SR latch for bit storage

![image-20211106054228740](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106054228740.png)

메모리는 왜 필요한가? - 메모리 없이는 구현 할 수 없는 시스템이 있다.

## Problem with SR latch

![image-20211106055656215](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106055656215.png)

Race condition (S, R이 둘 다 1일 때) condition이 latch로 바뀌면 latch에 모순이 생기고 오실레이터가 됨

t, q가 둘 다 타이밍을 맞춰서 바뀌면서 진동하다가, delay 차이로 인해 서로가 다른 값을 갖게 되는 순간 안정화로 돌입한다.

![image-20211106060923949](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106060923949.png)

![image-20211106060931716](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106060931716.png)

항상 reset이 set보다 늦게 결정되는 문제(glitch)가 발생한다.

같은 신호인데 다른 delay를 가지면 많은 문제가 발생한다.

## Solution: Level-sensitive SR latch

![image-20211106060951190](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106060951190.png)

clock signal을 도입

기존에 NOT 회로를 추가해서 구현하는 방식은 논리회로로 방법을 찾은 것이었음. 현재 피하고 싶은 것은 race condition. 그런데 이 방식에서는 delay로 인해 glitch가 발생한다.

c가 1이면 1, 0이면 0이 되는 구조 -> clock을 설정하고 SR의 값을 바꾸면 glitch가 예방됨

stabilized된 다음에 신호를 통과시키면 된다.

## Level-sensitive D latch

![image-20211106062458526](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106062458526.png)

## Half-adder

![image-20211106091616438](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106091616438.png)

## Full-adder

![image-20211106091956789](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106091956789.png)

## Full-adder using half adder

![image-20211106092935868](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106092935868.png)

## Carry-ripple adder

![image-20211106093019250](/Kevin_Min/images/2021-11-06-digital-system-circuits-week-10/image-20211106093019250.png)

