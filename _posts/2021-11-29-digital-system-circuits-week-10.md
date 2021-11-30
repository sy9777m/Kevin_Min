---
toc: true
layout: post
description: Soongsil University 2-2 Digital System Circuits week 10.
categories: [markdown]
title: Digital System Circuits week 10
---
# Digital System Circuits week 10

## SR-latch Introduction

cross-coupled NOR gate

![image-20211130023147982](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023147982.png)

## Storing one bit - flip-flops example requiring bit storage

![image-20211130023155938](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023155938.png)

## First attempt at bit storage

![image-20211130023229253](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023229253.png)

## Bit storage using an SR Latch

![image-20211130023241528](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023241528.png)

![image-20211130023247677](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023247677.png)

Invalid condition = race condition

-   한 번 바뀌면 다시 바뀌지 않는 상태

## Example using SR Latch for bit storage

![image-20211130023300788](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023300788.png)

## Problem with SR Latch

![image-20211130023313917](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023313917.png)

![image-20211130023323797](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023323797.png)

![image-20211130023333918](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023333918.png)

glitch - unwanted spark caused by logic gate delay

## Solution: Level-sensitive SR Latch

![image-20211130023109651](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130023109651.png)

## Level-sensitive D Latch

![image-20211130030411499](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130030411499.png)

## Problem with level-sensitive D Latch

![image-20211130030536292](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130030536292.png)

![image-20211130030546389](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130030546389.png)

## D Flip-Flop

![image-20211130030558393](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130030558393.png)

![image-20211130031700597](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130031700597.png)

![image-20211130031707887](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130031707887.png)

## D Latch vs. D Flip-Flop

![image-20211130032715015](/Kevin_Min/images/2021-11-29-digital-system-circuits-week-11/image-20211130032715015.png)
