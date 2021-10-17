---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms 7th week.
categories: [markdown]
title: Algorithms week 7
---
# Algorithms Week 7

## Binary search tree

![image-20211013235723717](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211013235723717.png)

![image-20211013235805633](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211013235805633.png)

Turns out that's not a great idea. Instead we turn to...

### Idea 1: Rotations

![image-20211013235957906](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211013235957906.png)

![image-20211014000228750](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014000228750.png)

Does this work?

Whenever something seems unbalanced, do rotations until it's okay gain. -> Even for me this is pretty vague. What do we mean by "seems unbalanced"? What's "okay"?

### Idea 2: have some proxy for balance

![image-20211014000513219](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014000513219.png)

![image-20211014000525049](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014000525049.png)

## Red-Black Trees

![image-20211014000607957](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014000607957.png)

![image-20211014000937523](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014000937523.png)

This is pretty balanced.

-   The black nodes are balanced.
-   The red nodes are "spread out" so they don't mess things up too much.

We can maintain this property as we insert/delete nodes, by using rotations.

The Red-Black structure is a proxy for balance. It's just a little weaker than perfect balance, but we can actually maintain it.

![image-20211014001326840](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014001326840.png)

![image-20211014001404332](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014001404332.png)

Okay, so it's balanced, but can we maintain it? -> Yes

![image-20211014001805278](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014001805278.png)

![image-20211014001830521](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014001830521.png)

![image-20211014001901422](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014001901422.png)

![image-20211014001923388](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014001923388.png)

![image-20211014002046260](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014002046260.png)

일단 red로 insert하고, grandparent와 parent의 색을 바꿈

![image-20211014002127476](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014002127476.png)

![image-20211014002150066](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014002150066.png)

root까지 recursive하게 색을 바꿔주면서 올라가면 됨

![image-20211014002328862](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014002328862.png)

![image-20211014002445454](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014002445454.png)

![image-20211014002529027](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014002529027.png)

![image-20211014003022520](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003022520.png)

딱 하나의 case만 고치는 예제 코드

### Deleting from a Red-Black tree

![image-20211014003555547](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003555547.png)

![image-20211014003626363](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003626363.png)

![image-20211014003718968](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003718968.png)

![image-20211014003723654](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003723654.png)

![image-20211014003749633](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003749633.png)

![image-20211014003913792](/Kevin_Min/images/2021-10-14-algorithms-week-7/image-20211014003913792.png)

