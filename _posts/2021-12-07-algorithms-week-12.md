---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms week 12.
categories: [markdown]
title: Algorithms week 12
---
# Algorithms week 12

![image-20211207071420794](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207071420794.png)

![image-20211207071429748](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207071429748.png)

## Longest Common Subsequence

![image-20211207071611990](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207071611990.png)

![image-20211207071623525](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207071623525.png)

![image-20211207071632062](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207071632062.png)

## We sometimes want to find these

![image-20211207071646562](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207071646562.png)

## Recipe for applying dynamic programming

![image-20211207072048370](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072048370.png)

## Step 1: optimal substructure

![image-20211207072105323](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072105323.png)

![image-20211207072114914](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072114914.png)

## Step 2: Find a recursive formulation for the length of the longest common subsequence

![image-20211207072350584](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072350584.png)

![image-20211207072358870](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072358870.png)

![image-20211207072408646](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072408646.png)

## Step 3: use dynamic programming to find the length of the longest common subsequence

### LCS DP

![image-20211207072849043](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072849043.png)

### Example

![image-20211207072903251](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072903251.png)

![image-20211207072911272](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072911272.png)

## Step 4: If needed, keep track of some additional info so that the algorithm from step 3 can find the actual LCS.

![image-20211207072937862](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072937862.png)

![image-20211207072945233](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207072945233.png)

![image-20211207073257898](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073257898.png)

![image-20211207073305806](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073305806.png)

![image-20211207073312807](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073312807.png)

![image-20211207073320545](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073320545.png)

![image-20211207073327420](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073327420.png)

![image-20211207073334458](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073334458.png)

![image-20211207073341451](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073341451.png)

## Step 5: If needed, code this up like a reasonable person.

### This pseudocode actually isn't so bad

![image-20211207073647275](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073647275.png)

## What have we learned?

![image-20211207073658672](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073658672.png)

## Knapsack

### Example: Knapsack problem

![image-20211207073711683](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073711683.png)

![image-20211207073733220](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073733220.png)

### Some notation

![image-20211207073745440](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207073745440.png)

## Recipe for applying dynamic programming

![image-20211207115907866](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207115907866.png)

## Optimal structure

![image-20211207115919252](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207115919252.png)

![image-20211207115937549](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207115937549.png)

## Step 2: Find a recursive formulation for the value of the optimal solution

### Recursive relationship

![image-20211207120048389](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120048389.png)

## Step 3: Use dynamic programming to find the value of the optimal solution

### Let's write a bottom-up DP algorithm

![image-20211207120119754](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120119754.png)

## Step 4: If needed, keep track of some additional info so that the algorithm from Step 3 can find the actual solution.

### Let's write a bottom-up DP algorithm

![image-20211207120204853](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120204853.png)

![image-20211207120542232](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120542232.png)

### Example

![image-20211207120555733](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120555733.png)

![image-20211207120607323](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120607323.png)

![image-20211207120617834](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120617834.png)

![image-20211207120628535](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120628535.png)

![image-20211207120640009](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120640009.png)

![image-20211207120704371](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120704371.png)

![image-20211207120713980](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120713980.png)

![image-20211207120728180](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207120728180.png)

## What have we learned?

![image-20211207121150220](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121150220.png)

## 0/1 Knapsack

![image-20211207121228743](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121228743.png)

## Step 1: Identify optimal substructure.

### Optimal substructure: try 1

![image-20211207121243559](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121243559.png)

### This won't quite work

![image-20211207121309228](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121309228.png)

### Optimal structure: try 2

![image-20211207121329522](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121329522.png)

## Our sub-problems:

![image-20211207121345277](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121345277.png)

## Two cases

![image-20211207121453001](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121453001.png)

### Case 1: optimal solution for j items does not use item j.

![image-20211207121621772](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121621772.png)

### Case 2: optimal solution for j items uses item j

![image-20211207121700737](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121700737.png)

## Step 2: find a recursive formulation for the value of the optimal solution.

### Recursive relationship

![image-20211207121739588](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121739588.png)

## Step 3: use dynamic programming to find the value of the optimal solution.

### Bottom-up DP algorithm

![image-20211207121841801](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121841801.png)

## Example

![image-20211207121905657](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121905657.png)

![image-20211207121914313](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207121914313.png)

![image-20211207122020213](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122020213.png)

![image-20211207122029165](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122029165.png)

![image-20211207122037977](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122037977.png)

![image-20211207122046546](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122046546.png)

![image-20211207122056884](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122056884.png)

![image-20211207122107288](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122107288.png)

![image-20211207122117785](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122117785.png)

![image-20211207122129053](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122129053.png)

![image-20211207122218721](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122218721.png)

![image-20211207122229043](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122229043.png)

![image-20211207122249982](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122249982.png)

![image-20211207122259152](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122259152.png)

![image-20211207122309367](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122309367.png)

![image-20211207122319578](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122319578.png)

![image-20211207122328257](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122328257.png)

## What have we learned?

![image-20211207122621320](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122621320.png)

## Question

![image-20211207122636131](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122636131.png)

## Independent set

![image-20211207122912123](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122912123.png)

## Actually this problem is NP-complete. So we are unlikely to find an efficient algorithm

![image-20211207122939165](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207122939165.png)

## Step 1: identify optimal structure

### Optimal structure

![image-20211207123332584](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123332584.png)

### Case 1: the root is not in a maximal independent set

![image-20211207123402431](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123402431.png)

### Case 2: the root is in a maximal independent set

![image-20211207123422340](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123422340.png)

## Step 2: find a recursive formulation for the value of the optimal solution

### Recursive formulation: try 1

![image-20211207123630180](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123630180.png)

### Recursive formulation: try 2

![image-20211207123822559](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123822559.png)

## Step 2: find a recursive formulation for the value of the optimal solution

### A top-down DP algorithm

![image-20211207123901494](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123901494.png)

## Why is this different from divide-and-conquer?

![image-20211207123920179](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207123920179.png)

![image-20211207124315270](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207124315270.png)

## What have we learned?

![image-20211207124327964](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207124327964.png)

## Recap

![image-20211207124337430](/Kevin_Min/images/2021-12-07-algorithms-week-12/image-20211207124337430.png)
