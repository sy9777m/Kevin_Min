---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms midterm.
categories: [markdown]
title: Algorithms midterm
---
# Algorithms Midterm

Computer science is abstraction.

Abstraction is to create a new model that allows to ignore irrelevant details.

## What is an algorithm?

Mathematical abstraction of computer program

-   At the heart of programs lie algorithms

Well-specified procedure for solving a computational problem.

Computational problem = mapping from inputs to outputs

## Analysis of algorithm

Does an algorithm actually work? - correctness

Is it fast? - Time/space efficiency, lower bounds, optimality

## Sorting problem

![image-20211021045928551](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021045928551.png)

## Insertion sort

Intuition - maintain a growing sorted list. For each element, put it into the 'right place' in this growing list.

![image-20211021050146237](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021050146237.png)

Key insight - to reason about the behavior of algorithms, it often helps to look for things that don't change.

### Proving correctness

There's name for a condition that is true before and after each iteration of a loop: a loop invariant

#### four components in a proof by induction

-   Inductive hypothesis - The loop invariant holds after the ith iteration.
-   Base case - The loop invariant holds before the first iteration.
-   Inductive step - If the loop invariant holds after the ith iteration, then it holds after the (i + 1)st iteration.
-   Conclusion - If the loop invariant holds after the last iteration, then the algorithm is correct.

## Analyzing runtime

![image-20211021051227989](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021051227989.png)

## Runtime analysis

-   Worst-case analysis - What is the runtime of the algorithm on the worst possible input?
    -   Algorithm performs at least this fast for every input.
-   Best-case analysis - What is the runtime of the algorithm on the best possible input?
-   Average-case analysis - What is the runtime of the algorithm on the average input?

## Asymptotic analysis

What does it mean to measure 'runtime' of an algorithm?

-   Engineers probably care most about the 'real-world time' - how long does the algorithm take in seconds, etc?
-   This heavily depends on computer hardware, programming language, etc.
-   Instead, we want to use a universal measure of runtime that's independent of these considerations.
-   Time-complexity

![image-20211021064234706](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064234706.png)

![image-20211021064244895](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064244895.png)

![image-20211021064308655](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064308655.png)

## Big-O means upper-bound

![image-20211021064326937](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064326937.png)

![image-20211021064339047](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064339047.png)

![image-20211021064404835](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064404835.png)

![image-20211021064434353](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064434353.png)

![image-20211021064442732](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064442732.png)

![image-20211021064450186](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064450186.png)

![image-20211021064459872](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021064459872.png)

![image-20211021065532173](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021065532173.png)

## Big-$\Omega$ means lower-bound

![image-20211021065624103](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021065624103.png)

![image-20211021065632773](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021065632773.png)

![image-20211021065713427](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021065713427.png)

## Big-$\Theta$ means upper and lower-bound

![image-20211021065743151](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021065743151.png)

## Asymptotic analysis

We call this asymptotic runtime as time-complexity

![image-20211021113646297](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021113646297.png)

![image-20211021113654535](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021113654535.png)

![image-20211021113707205](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021113707205.png)

## Sort

-   Insertion sort - It finds a proper (sorted) position, and insert an element into there
-   Selection sort - It picks a min/max element from the unsorted list, and put the element into the front/end of the sorted list.
-   Bubble sort - It pushes higher values to the end of the list. The highest element in the list will float toward the end of the list.

## Selection sort

![image-20211021114006059](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114006059.png)

## Bubble sort

![image-20211021114017977](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114017977.png)

## Merge sort

Merge sort uses divide-and-conquer.

Intuition - Divide the list into halves, recursively sort them, merge the sorted halves into a whole sorted list, and return this list.

### Divide and conquer

Divide - Break the current problem into smaller (easier) sub-problems.

Conquer - Solve the smaller problems and collect the results to solve the current problem.

![image-20211021114147750](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114147750.png)

![image-20211021114156442](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114156442.png)

![image-20211021114323616](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114323616.png)

![image-20211021114206080](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114206080.png)

![image-20211021114213527](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114213527.png)

![image-20211021114342564](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114342564.png)

### Providing Correctness

![image-20211021114713745](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021114713745.png)

#### iterative algorithm

1.   Find the loop invariant
2.   Define the inductive hypothesis (internal state at iteration i)
3.   Prove the base case
4.   Prove the inductive step
5.   Prove the conclusion

#### recursive algorithm

1.   Define the inductive hypothesis (correct for inputs of sizes 1 to i)
2.   Prove the base case (i < small constant)
3.   Prove the inductive step (i >= i + 1 or {1, 2, ..., i} => i + 1)
4.   Prove the conclusion (i = n => correct)

### Analyzing runtime

![image-20211021115113577](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115113577.png)

![image-20211021115128435](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115128435.png)

![image-20211021115139728](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115139728.png)

![image-20211021115153888](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115153888.png)

A recurrence relation is a function or sequence whose values are defined in terms of earlier or smaller values.

Our recurrence relation for the runtime of merge sort isn't very useful unless we can define the runtime as closed-form expression.

![image-20211021115320101](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115320101.png)

![image-20211021115325460](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115325460.png)

![image-20211021115332666](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115332666.png)

![image-20211021115402489](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115402489.png)

There are a few different methods to translate a recurrence relation for T(n) to a closed form expression for T(n).

-   Recursion tree method
-   Iteration method
-   Master method
-   Substitution method

#### Recursion tree method

![image-20211021115511422](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115511422.png)

![image-20211021115549864](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115549864.png)

#### Iteration method

![image-20211021115644792](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115644792.png)

#### A formula that solves recurrences when all of the sub-problems are the same size.

![image-20211021115749458](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021115749458.png)

![image-20211021120117774](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021120117774.png)

![image-20211021120338604](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021120338604.png)

![image-20211021120353984](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021120353984.png)

### Substitution method

![image-20211021120419695](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021120419695.png)

![image-20211021120855580](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021120855580.png)

![image-20211021120938894](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021120938894.png)

![image-20211021121021910](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021121021910.png)

![image-20211021121033424](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021121033424.png)

## Linear-time selection

![image-20211021121111444](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021121111444.png)

![image-20211021121435241](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021121435241.png)

![image-20211021123527621](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021123527621.png)

![image-20211021123604626](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021123604626.png)

![image-20211021123614720](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021123614720.png)

![image-20211021123705893](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021123705893.png)

Intuition - Partition the list about a pivot selected at random, either return the pivot itself or recurse on the left or right sublists.

![image-20211021123841793](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021123841793.png)

![image-20211021123859299](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021123859299.png)

![image-20211021124013222](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124013222.png)

### Analyzing runtime

![image-20211021124053956](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124053956.png)

![image-20211021124117908](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124117908.png)

![image-20211021124206062](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124206062.png)

![image-20211021124221045](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124221045.png)

![image-20211021124237358](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124237358.png)

![image-20211021124302121](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124302121.png)

![image-20211021124334872](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124334872.png)

### Another divide and conquer algorithm

![image-20211021124543973](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124543973.png)

![image-20211021124607439](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124607439.png)

![image-20211021124642884](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124642884.png)

![image-20211021124756000](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124756000.png)

![image-20211021124807814](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124807814.png)

![image-20211021124921869](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021124921869.png)

![image-20211021125019839](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125019839.png)

![image-20211021125052810](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125052810.png)

![image-20211021125120172](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125120172.png)

![image-20211021125140424](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125140424.png)

![image-20211021125152001](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125152001.png)

![image-20211021125306215](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125306215.png)

![image-20211021125319020](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125319020.png)

![image-20211021125346128](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125346128.png)

![image-20211021125402720](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125402720.png)

![image-20211021125413114](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125413114.png)

## (Randomized) Quick sort

![image-20211021125455038](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125455038.png)

![image-20211021125508556](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125508556.png)

![image-20211021125515292](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125515292.png)

![image-20211021125522704](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125522704.png)

![image-20211021125640746](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125640746.png)

![image-20211021125710320](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125710320.png)

![image-20211021125720635](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125720635.png)

## Lower-bound of comparison-based sorting

![image-20211021125835592](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125835592.png)

![image-20211021125859358](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125859358.png)

![image-20211021125908463](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125908463.png)

### Decision tree

![image-20211021125927533](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125927533.png)

![image-20211021125938128](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021125938128.png)

![image-20211021130018106](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130018106.png)

![image-20211021130030014](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130030014.png)

![image-20211021130043823](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130043823.png)

## Comparison-based sorting

![image-20211021130236653](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130236653.png)

## Linear-time sorting

### Is linear-time sorting nonsense?

![image-20211021130330928](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130330928.png)

### Counting sort

![image-20211021130456924](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130456924.png)

![image-20211021130514580](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130514580.png)

### Bucket sort

![image-20211021130527622](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130527622.png)

![image-20211021130538816](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130538816.png)

![image-20211021130545390](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130545390.png)

![image-20211021130623552](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130623552.png)

![image-20211021130645631](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130645631.png)

### Radix sort

![image-20211021130700769](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130700769.png)

![image-20211021130723160](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130723160.png)

![image-20211021130735725](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130735725.png)

![image-20211021130753189](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130753189.png)

![image-20211021130809763](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130809763.png)

![image-20211021130815905](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130815905.png)

### The story so far

![image-20211021130834178](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130834178.png)

### Comparison-based vs. linear-time sorting

![image-20211021130911653](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021130911653.png)

## Data structures

![image-20211021131022047](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021131022047.png)

## Hash table

![image-20211021135954380](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021135954380.png)

![image-20211021140007618](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140007618.png)

![image-20211021140014875](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140014875.png)

![image-20211021140038533](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140038533.png)

![image-20211021140048914](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140048914.png)

![image-20211021140107324](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140107324.png)

![image-20211021140117131](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140117131.png)

![image-20211021140127261](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140127261.png)

![image-20211021140147163](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140147163.png)

![image-20211021140210438](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140210438.png)

![image-20211021140331091](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140331091.png)

### Hash collision

![image-20211021140345342](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140345342.png)

### Chaining

![image-20211021140401201](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140401201.png)

### Aside: Hash tables with open addressing

![image-20211021140436508](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140436508.png)

![image-20211021140558531](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140558531.png)

### Worst-case analysis

![image-20211021140628307](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140628307.png)

![image-20211021140646044](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140646044.png)

![image-20211021140657468](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140657468.png)

![image-20211021140712112](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140712112.png)

![image-20211021140724599](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140724599.png)

## A simple (deterministic) hash function

![image-20211021140802968](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140802968.png)

![image-20211021140819066](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140819066.png)

![image-20211021140841480](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140841480.png)

![image-20211021140851270](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140851270.png)

![image-20211021140930844](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140930844.png)

### Summary

![image-20211021140941021](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021140941021.png)

## Tree algorithms

![image-20211021141100050](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141100050.png)

### Sorted arrays

![image-20211021141124175](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141124175.png)

### Sorted linked lists

![image-20211021141138896](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141138896.png)

### motivation for Binary search tree

![image-20211021141204027](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141204027.png)

## Binary search tree

### Recall the data structure

![image-20211021141230971](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141230971.png)

![image-20211021141237742](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141237742.png)

![image-20211021141247448](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141247448.png)

![image-20211021141307041](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141307041.png)

### Binary tree terminology

![image-20211021141324893](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141324893.png)

## Binary search trees

![image-20211021141408613](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141408613.png)

![image-20211021141420978](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141420978.png)

kinda like quick sort

![image-20211021141450278](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141450278.png)

### Search in a binary search tree

![image-20211021141516883](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141516883.png)

### Insert in a binary search tree

![image-20211021141546068](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141546068.png)

### Delete in a binary search tree

![image-20211021141622910](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141622910.png)

#### Several delete cases

![image-20211021141651027](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141651027.png)

![image-20211021141702181](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141702181.png)

![image-20211021141732651](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141732651.png)

![image-20211021141742085](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141742085.png)

![image-20211021141752435](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141752435.png)

![image-20211021141857775](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141857775.png)

### How long do these operations take?

![image-20211021141912341](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141912341.png)

![image-20211021141923868](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141923868.png)

![image-20211021141941401](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021141941401.png)

## Self-balancing binary search tree

### Idea 1: rotations

![image-20211021142015744](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142015744.png)

![image-20211021142037839](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142037839.png)

![image-20211021142049696](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142049696.png)

![image-20211021142117873](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142117873.png)

### Idea 2: have some proxy for balance

![image-20211021142134160](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142134160.png)

## Red-black trees

![image-20211021142149756](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142149756.png)

### these rules are the proxy for balance

![image-20211021142216503](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142216503.png)

![image-20211021142247516](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142247516.png)

![image-20211021142653695](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142653695.png)

### Intuition

![image-20211021142724709](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142724709.png)

### Inserting into a red-black tree

![image-20211021142821101](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142821101.png)

![image-20211021142849669](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142849669.png)

![image-20211021142900482](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142900482.png)

![image-20211021142914061](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142914061.png)

![image-20211021142931249](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142931249.png)

![image-20211021142942187](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142942187.png)

![image-20211021142956735](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021142956735.png)

![image-20211021143016512](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143016512.png)

![image-20211021143054322](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143054322.png)

![image-20211021143108138](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143108138.png)

![image-20211021143130638](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143130638.png)

![image-20211021143141392](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143141392.png)

### Deleting from a red-black tree

![image-20211021143157008](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143157008.png)

![image-20211021143208450](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143208450.png)

![image-20211021143233556](/Kevin_Min/images/2021-10-20-algorithms-midterm/image-20211021143233556.png)

