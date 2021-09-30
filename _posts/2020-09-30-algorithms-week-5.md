---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms 5th week.
categories: [markdown]
title: Algorithms week 5
---
# Algorithms Week 5

## Linear time sorting

-   Comparison-based sorting에 성능적인 한계가 있음
-   이러한 단점을 해결하기 위한 linear-time sorting 기법들이 있음

## (Randomized) Quicksort

It behaves as follows:

-   If the list has 0 or 1 elements it's sorted.
-   Otherwise, choose a pivot and partition around it.
-   Recursively apply quicksort to the sublists to the left and right of the pivot.

![image-20210930183827208](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930183827208.png)

![image-20210930183850182](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930183850182.png)

Worst-case runtime - $O(n^{2})$: When `pivot = array[r]`

### Randomized Quicksort

![image-20210930184455769](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930184455769.png)

Worst-case - $O(n^{2})$: Think of this as the adversary chooses the randomness.

Expected - $O(n\log{n})$

### Initial observations

There's a really good case, in which partition always picks the median element as the pivot.

![image-20210930184713329](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930184713329.png)

There's a really bad case, in which partition always picks the smallest or largest element as the pivot.

![image-20210930184746442](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930184746442.png)

### Expected runtime of randomized quicksort

![image-20210930184913455](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930184913455.png)

## Lower-bound of comparison-based sorting

### Sorting

We've seen a few sorting algorithms

-   Insertion sort is worst-case $O(n^{2})$-time.
-   Mergesort is worst-case $O(n\log{n})$-time.
-   Quicksort is worst-case $O(n\log{n})$-time.

Comparison-based algorithms use "comparisons" to achieve their output.

-   Linear-time select is a comparison-based algorithms.
-   quicksort, mergesort, insertionsort

![image-20210930185250500](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185250500.png)

![image-20210930185318393](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185318393.png)

## Decision tree

![image-20210930185525497](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185525497.png)

![image-20210930185537302](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185537302.png)

The leaves of this tree are all possible orderings of the items: when we reach a leaf we return it.

Running the algorithm on a given input corresponds to taking a particular path through the tree.

![image-20210930185728867](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185728867.png)

![image-20210930185812594](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185812594.png)

![image-20210930185847662](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2020-09-30-algorithms-week-5\image-20210930185847662.png)

