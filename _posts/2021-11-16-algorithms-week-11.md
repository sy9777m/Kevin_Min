---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms week 11.
categories: [markdown]
title: Algorithms week 11
---
# Algorithms week 11

## Dynamic programming

-   Bellman-Ford algorithm
-   Fibonacci Numbers
-   Floyd-Warshall algorithm

Another problems

-   Longest common subsequence
-   knapsack
-   Independent sets

## Bellman-Ford

![image-20211116154308897](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116154308897.png)

![image-20211116154448448](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116154448448.png)

## Bellman-Ford vs. Dijkstra

![image-20211116154501152](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116154501152.png)

## Bellman-Ford

![image-20211116154518038](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116154518038.png)

![image-20211116154858372](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116154858372.png)

![image-20211116154908832](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116154908832.png)

![image-20211116155451181](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155451181.png)

![image-20211116155458680](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155458680.png)

![image-20211116155506398](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155506398.png)

![image-20211116155513536](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155513536.png)

### Interpretation of $d^{(i)}$

![image-20211116155534589](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155534589.png)

## Why does Bellman-Ford work?

![image-20211116155547256](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155547256.png)

### Inductive step

![image-20211116155601590](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116155601590.png)

## Proof by induction

![image-20211116160310811](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116160310811.png)

## Bellman-Ford Algorithm

![image-20211116160408418](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116160408418.png)

## Shortest paths

![image-20211116160420769](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116160420769.png)

## Aside: Link-state vs Distance-vector

![image-20211116160435312](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116160435312.png)

## Important thing about Bellman-Ford for the rest of this lecture

![image-20211116163954629](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116163954629.png)

## Bellman-Ford is an example of dynamic programming!

![image-20211116164016489](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164016489.png)

### Example: How to compute Fibonacci numbers

![image-20211116164227743](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164227743.png)

## Candidate algorithm

![image-20211116164240307](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164240307.png)

![image-20211116164415290](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164415290.png)

## Maybe this would be better

![image-20211116164427531](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164427531.png)

![image-20211116164711518](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164711518.png)

## What is dynamic programming?

![image-20211116164722207](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164722207.png)

## Elements of dynamic programming

![image-20211116164928672](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164928672.png)

![image-20211116164935415](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164935415.png)

![image-20211116164944044](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116164944044.png)

## Two ways to think about and/or implement DP algorithms

-   Top down
-   Bottom up

## Bottom up approach

![image-20211116165425927](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165425927.png)

![image-20211116165432333](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165432333.png)

![image-20211116165438534](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165438534.png)

![image-20211116165447382](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165447382.png)

## Top down approach

![image-20211116165458926](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165458926.png)

### Example of top-down Fibonacci

![image-20211116165514624](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165514624.png)

## Memo-ization visualization

![image-20211116165640104](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165640104.png)

![image-20211116165648879](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116165648879.png)

## Dynamic programming

![image-20211116170421334](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116170421334.png)

## Floyd-Warshall

![image-20211116170436913](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116170436913.png)

![image-20211116172910024](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116172910024.png)

## Optimal substructure

![image-20211116173401233](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173401233.png)

![image-20211116173412503](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173412503.png)

![image-20211116173422232](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173422232.png)

![image-20211116173433795](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173433795.png)

![image-20211116173444781](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173444781.png)

## Aside: simple paths

![image-20211116173941190](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173941190.png)

## Case 2 continued

![image-20211116173951578](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116173951578.png)

![image-20211116174044238](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116174044238.png)

![image-20211116174050402](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116174050402.png)

## Floyd-Warshall algorithm

![image-20211116174102136](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116174102136.png)

## We've basically just shown

![image-20211116185859072](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116185859072.png)

## What if there are negative cycles?

![image-20211116185913330](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116185913330.png)

![image-20211116185920257](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116185920257.png)

## What have we learned?

![image-20211116185933063](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116185933063.png)

## Graph algorithms

![image-20211116190732161](/Kevin_Min/images/2021-11-16-algorithms-week-11/image-20211116190732161.png)

