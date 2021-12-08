---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms final summary.
categories: [markdown]
title: Algorithms final summary
---
# Algorithms final summary

## How do we represent graphs?

![image-20211209000613505](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000613505.png)

![image-20211209000621212](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000621212.png)

## Trade-offs

![image-20211209000632595](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000632595.png)

## DFS

### Running time to explore just the connected component we started in

![image-20211209000717087](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000717087.png)

## Topological ordering

![image-20211209000831977](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000831977.png)

### DAG (Directed Acyclic Graph)

![image-20211209000759261](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000759261.png)

![image-20211209000811117](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000811117.png)

directed graph with no directed cycles

### Finish times seems useful

![image-20211209000845819](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000845819.png)

![image-20211209000857699](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000857699.png)

![image-20211209000925934](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000925934.png)

![image-20211209000931435](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000931435.png)

![image-20211209000948588](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209000948588.png)

## BFS

![image-20211209001004783](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209001004783.png)

### Running time to explore the whole thing

![image-20211209001215828](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209001215828.png)

### Shortest path

![image-20211209001229430](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209001229430.png)

## Shortest path problem

![image-20211209001309197](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209001309197.png)

## Dijkstra algorithm

![image-20211209000434398](C:\Users\Siyun\OneDrive\project\Kevin_Min\images\2021-12-09-algorithms-final\image-20211209000434398.png)

![image-20211209001335284](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209001335284.png)

### Why does this work?

![image-20211209002512642](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002512642.png)

![image-20211209002004336](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002004336.png)

![image-20211209002130087](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002130087.png)

![image-20211209002249578](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002249578.png)

![image-20211209002331356](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002331356.png)

![image-20211209002352183](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002352183.png)

![image-20211209002447072](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002447072.png)

![image-20211209002536085](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002536085.png)

### Running time

![image-20211209002549675](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002549675.png)

![image-20211209002803483](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002803483.png)

![image-20211209002809127](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002809127.png)

### If we use a red-black tree

![image-20211209002821345](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209002821345.png)

### Dijkstra drawbacks

![image-20211209005014090](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005014090.png)

## Bellman-Ford

![image-20211209005335064](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005335064.png)

![image-20211209005359661](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005359661.png)

![image-20211209005413194](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005413194.png)

![image-20211209005549151](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005549151.png)

### Running time

![image-20211209005614527](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005614527.png)

### Bellman-Ford and negative edge weights

![image-20211209005635278](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005635278.png)

![image-20211209005849648](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005849648.png)

![image-20211209005857800](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209005857800.png)

![image-20211209013121078](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013121078.png)

## Recap: shortest paths

![image-20211209013207753](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013207753.png)

## Dynamic programming

![image-20211209013510782](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013510782.png)

### Elements of dynamic programming

![image-20211209013541321](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013541321.png)

![image-20211209013616339](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013616339.png)

![image-20211209013628300](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013628300.png)

## Bottom up approach

![image-20211209013652718](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013652718.png)

![image-20211209013707973](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013707973.png)

## Top down approach

![image-20211209013719208](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013719208.png)

## Floyd-Warshall

![image-20211209013837247](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013837247.png)

![image-20211209013845254](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013845254.png)

### Optimal substructure

![image-20211209013902576](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209013902576.png)

### How can we find $D^{k}[u, v]$ using $D^{k-1}$

![image-20211209014219712](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014219712.png)

![image-20211209014227969](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014227969.png)

![image-20211209014233898](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014233898.png)

![image-20211209014322974](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014322974.png)

![image-20211209014330876](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014330876.png)

## Floyd-Warshall algorithm

![image-20211209014349302](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014349302.png)

![image-20211209014401446](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014401446.png)

## Graph algorithms

![image-20211209014439149](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014439149.png)

## Recap

![image-20211209014543078](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014543078.png)

## Longest common subsequence

![image-20211209014616466](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014616466.png)

![image-20211209014623288](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014623288.png)

![image-20211209014633642](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014633642.png)

## Recipe for applying dynamic programming

![image-20211209014654548](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014654548.png)

## Step 1: optimal substructure

![image-20211209014724644](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014724644.png)

## Step 2: find a recursive formulation for the length of the longest common subsequence

![image-20211209014817181](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014817181.png)

![image-20211209014843751](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014843751.png)

![image-20211209014900506](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209014900506.png)

## Step 3: use dynamic programming to find the length of the longest common subsequence

![image-20211209015015942](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015015942.png)

![image-20211209015039116](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015039116.png)

## Step 4: If needed, keep track of some additional info so that the algorithm from step 3 can find the actual LCS.

![image-20211209015112353](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015112353.png)

![image-20211209015120089](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015120089.png)

## Step 5: if needed, code this up like a reasonable person

![image-20211209015202864](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015202864.png)

## Knapsack

![image-20211209015228375](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015228375.png)

## Step 1: Identify optimal substructure

![image-20211209015846410](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015846410.png)

![image-20211209015856760](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015856760.png)

## Step 2: Find a recursive formulation for the value of the optimal solution

![image-20211209015937256](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209015937256.png)

## Step 3: Use dynamic programming to find the value of the optimal solution

![image-20211209020001333](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020001333.png)

## Step 4: If needed, keep track of some additional info so that the algorithm from step 3 can find the actual solution.

![image-20211209020034357](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020034357.png)

![image-20211209020044601](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020044601.png)

![image-20211209020056804](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020056804.png)

![image-20211209020124989](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020124989.png)

## 0/1 knapsack

![image-20211209020149430](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020149430.png)

## Step 1: identify optimal substructure

![image-20211209020204533](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020204533.png)

![image-20211209020213417](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020213417.png)

![image-20211209020228603](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020228603.png)

![image-20211209020241679](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020241679.png)

![image-20211209020249164](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020249164.png)

![image-20211209020259097](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020259097.png)

![image-20211209020655701](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020655701.png)

## Step 2: find a recursive formulation for the value of the optimal solution

![image-20211209020722384](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020722384.png)

## Step 3: use dynamic programming to find the value of the optimal solution

![image-20211209020752779](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020752779.png)

![image-20211209020817580](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020817580.png)

## Question: how did we know which substructure to use in which variant of knapsack?

![image-20211209020849652](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020849652.png)

## Independent set

![image-20211209020920665](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209020920665.png)

## NP-complete

so we are unlikely to find an efficient algorithm.

## Step 1: Identify optimal substructure

![image-20211209021025874](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021025874.png)

### Case 1: the root is not in a maximal independent set

![image-20211209021047954](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021047954.png)

### Case 2: the root is in a maximal independent set

![image-20211209021103251](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021103251.png)

## Step 2: find a recursive formulation for the value of the optimal solution

![image-20211209021123134](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021123134.png)

![image-20211209021139075](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021139075.png)

## Step 3: use dynamic programming to find the value of the optimal solution

![image-20211209021201306](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021201306.png)

## Greedy algorithms

![image-20211209021324373](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021324373.png)

### Unbounded knapsack

![image-20211209021345116](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021345116.png)

## Activity selection

![image-20211209021408630](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021408630.png)

![image-20211209021414684](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021414684.png)

![image-20211209021421917](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021421917.png)

### At least it's fast

![image-20211209021433300](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021433300.png)

## What makes it greedy?

![image-20211209021444945](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021444945.png)

## Three questions

![image-20211209021457797](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021457797.png)

![image-20211209021521186](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021521186.png)

## Sub-problem graph view

![image-20211209021656538](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021656538.png)

![image-20211209021702523](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021702523.png)

![image-20211209021707642](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021707642.png)

![image-20211209021715120](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021715120.png)

## Huffman coding

![image-20211209021950587](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209021950587.png)

![image-20211209022023177](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022023177.png)

## Minimum spanning tree

![image-20211209022115678](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022115678.png)

## Prim's algorithm

![image-20211209022141925](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022141925.png)

## Kruskal's algorithm

![image-20211209022219290](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022219290.png)

![image-20211209022230484](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022230484.png)

![image-20211209022237293](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022237293.png)

![image-20211209022256998](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022256998.png)

## Both Prim and Kruskal

![image-20211209022318333](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022318333.png)

## Class of "P" problems

![image-20211209022503811](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022503811.png)

![image-20211209022514576](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022514576.png)

## Tractable / Intractable problems

![image-20211209022530970](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022530970.png)

## Hamiltonian cycle

![image-20211209022658129](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022658129.png)

## Traveling salesman problem

![image-20211209022712564](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022712564.png)

![image-20211209022725181](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022725181.png)

## Intractable problems

![image-20211209022736552](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022736552.png)

## P vs. NP

![image-20211209022753608](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022753608.png)

## Nondeterministic algorithms

![image-20211209022808803](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022808803.png)

## Nondeterministic and NP algorithms

![image-20211209022821913](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022821913.png)

![image-20211209022836427](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022836427.png)

## Class of "NP" problems

![image-20211209022913587](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022913587.png)

![image-20211209022932710](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022932710.png)

## Is P = NP?

![image-20211209022959233](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209022959233.png)

## Reductions

![image-20211209023036923](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023036923.png)

## Polynomial reductions

![image-20211209023052857](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023052857.png)

![image-20211209023101335](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023101335.png)

## NP-completeness

![image-20211209023119201](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023119201.png)

![image-20211209023131816](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023131816.png)

## Providing NP-completeness in practice

![image-20211209023211015](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023211015.png)

![image-20211209023219814](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023219814.png)

## P & NP-complete problems

![image-20211209023254097](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023254097.png)

![image-20211209023301368](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023301368.png)

## Satisfiability problem (SAT)

![image-20211209023325167](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023325167.png)

## CNF satisfiability

![image-20211209023337145](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023337145.png)

## 3-CNF satisfiability (3-SAT)

![image-20211209023353343](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023353343.png)

![image-20211209023400463](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023400463.png)

## Clique![image-20211209023409704](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023409704.png)

### Clique verifier

![image-20211209023425272](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023425272.png)

![image-20211209023432422](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023432422.png)

![image-20211209023440986](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023440986.png)

## Classes of problems

![image-20211209023501263](/Kevin_Min/images/2021-12-09-algorithms-final-summary/image-20211209023501263.png)
