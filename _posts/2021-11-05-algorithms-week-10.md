---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms week 10.
categories: [markdown]
title: Algorithms week 10
---
# Algorithms week 10

## Back to this example

![image-20211105154620461](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154620461.png)

## Dijkstra's algorithm

![image-20211105154634909](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154634909.png)

### Intuition

![image-20211105154644192](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154644192.png)

![image-20211105154653856](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154653856.png)

![image-20211105154659840](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154659840.png)

![image-20211105154706273](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154706273.png)

![image-20211105154713292](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154713292.png)

![image-20211105154720858](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154720858.png)

![image-20211105154730966](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105154730966.png)

## How do we actually implement this?

![image-20211105155406001](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155406001.png)

## Dijkstra by example

![image-20211105155420483](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155420483.png)

![image-20211105155431038](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155431038.png)

![image-20211105155439388](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155439388.png)

![image-20211105155447468](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155447468.png)

![image-20211105155622120](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155622120.png)

![image-20211105155631690](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155631690.png)

![image-20211105155640018](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155640018.png)

![image-20211105155649627](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155649627.png)

![image-20211105155656987](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155656987.png)

![image-20211105155704100](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155704100.png)

![image-20211105155711081](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155711081.png)

![image-20211105155719083](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155719083.png)

![image-20211105155726009](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155726009.png)

![image-20211105155735415](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155735415.png)

## Dijkstra's algorithm

![image-20211105155747640](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105155747640.png)

![image-20211105160347966](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105160347966.png)

![image-20211105160354164](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105160354164.png)

![image-20211105160403823](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105160403823.png)

## Why does this work?

![image-20211105160413886](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105160413886.png)

## Claim 1

![image-20211105160426595](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105160426595.png)

## Claim 2

![image-20211105160437243](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105160437243.png)

![image-20211105161455991](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161455991.png)

![image-20211105161506768](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161506768.png)

![image-20211105161518358](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161518358.png)

![image-20211105161543479](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161543479.png)

![image-20211105161552447](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161552447.png)

![image-20211105161600521](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161600521.png)

## Why does this work?

![image-20211105161616726](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161616726.png)

## What did we just learn?

![image-20211105161628610](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161628610.png)

## Running time?

![image-20211105161810146](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161810146.png)

## We need a data structure that:

![image-20211105161826227](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105161826227.png)

## If we use an array

![image-20211105162124216](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162124216.png)

![image-20211105162331921](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162331921.png)

## If we use an a red-black tree

![image-20211105162136427](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162136427.png)

## Heaps support these operations

![image-20211105162147658](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162147658.png)

![image-20211105162606249](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162606249.png)

## Say we use a Fibonacci heap

![image-20211105162619212](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162619212.png)

## Dijkstra is used in practice

![image-20211105162636344](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162636344.png)

## Dijkstra drawbacks

![image-20211105162647934](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162647934.png)

## Bellman-Ford algorithm

![image-20211105162913151](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105162913151.png)

time complexity가 Dijkstra's algorithm보다 높다

## Recall: Shortest path problem

![image-20211105194544656](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105194544656.png)

## Why negative edge weights?

![image-20211105194756414](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105194756414.png)

## One problem with negative edge weights

![image-20211105195008495](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105195008495.png)

음의 가중치가 존재할 때, shortest path는 무엇인가 - cycle이 없어야 한다. 무한히 negative cycle을 돌면 -inf 값으로 수렴하기 때문

그래서 negative cycle이 있을 때 shortest path는 의미가 없다.

## Bellman-Ford algorithm

![image-20211105195238896](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105195238896.png)

u의 인접노드를 전부 돌면서 최단거리 계산

## For some reasons

![image-20211105195254112](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105195254112.png)

## Bellman-Ford

![image-20211105200639135](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200639135.png)

![image-20211105200756719](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200756719.png)

![image-20211105200804777](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200804777.png)

![image-20211105200813046](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200813046.png)

![image-20211105200819910](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200819910.png)

![image-20211105200829993](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200829993.png)

## This seems much slower than Dijkstra

![image-20211105200844470](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105200844470.png)

m = number of edges

n = number of vertices

## One problem with negative edge weights

![image-20211105201504489](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105201504489.png)

## Bellman-Ford and negative edge weights

![image-20211105201626437](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105201626437.png)

## Negative edge weights

![image-20211105201837777](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105201837777.png)

![image-20211105201845614](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105201845614.png)

## Back to the correctness

![image-20211105201858968](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105201858968.png)

## How Bellman-Ford deals with negative weights

![image-20211105202208598](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105202208598.png)

## Bellman-Ford algorithm

![image-20211105202220591](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105202220591.png)

![image-20211105204044922](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105204044922.png)

![image-20211105204054892](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105204054892.png)

## What have we learned?

![image-20211105204109802](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105204109802.png)

## Bellman-Ford is also used in practice

![image-20211105204123292](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105204123292.png)

## Recap: shortest paths

![image-20211105204135725](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105204135725.png)

## Outline

![image-20211105205648715](/Kevin_Min/images/2021-11-05-algorithms-week-10/image-20211105205648715.png)

