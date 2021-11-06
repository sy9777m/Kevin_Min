---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms week 9.
categories: [markdown]
title: Algorithms week 9
---
# Algorithms week 9

## Topological ordering

위상정렬

### Application of DFS

![image-20211105053608856](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105053608856.png)

![image-20211105053831906](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105053831906.png)

dependencies를 고려해서 올바른 순서를 찾아주는 sorting -> topological sorting

## Directed Acyclic Graphs

![image-20211105053951010](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105053951010.png)

## Topological ordering

![image-20211105054105226](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054105226.png)

## Let's do DFS

![image-20211105054235979](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054235979.png)

## Finish times seem useful

![image-20211105054348814](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054348814.png)

## A more general statement

![image-20211105054541891](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054541891.png)

![image-20211105054754679](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054754679.png)

![image-20211105054803920](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054803920.png)

## Back to this problem

![image-20211105054817242](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105054817242.png)

## In reverse order of finishing time

![image-20211105055052827](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105055052827.png)

## Topological ordering

![image-20211105055104896](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105055104896.png)

![image-20211105055112251](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105055112251.png)

### Example

![image-20211105055134402](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105055134402.png)

![image-20211105055127357](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105055127357.png)

![image-20211105060958201](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105060958201.png)

![image-20211105061003923](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105061003923.png)

![image-20211105061010571](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105061010571.png)

![image-20211105061018009](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105061018009.png)

![image-20211105061025420](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105061025420.png)

![image-20211105061032723](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105061032723.png)

## Breadth-First search

## How do we explore a graph?

![image-20211105150655153](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105150655153.png)

## Breadth-First Search

![image-20211105150708822](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105150708822.png)

![image-20211105150716159](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105150716159.png)

![image-20211105150723432](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105150723432.png)

![image-20211105150730916](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105150730916.png)

![image-20211105150738747](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105150738747.png)

![image-20211105151041469](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105151041469.png)

![image-20211105151047735](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105151047735.png)

![image-20211105151052997](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105151052997.png)

## BFS also finds all the nodes reachable from the starting point

![image-20211105151108917](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105151108917.png)

## Running time

![image-20211105152247090](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105152247090.png)

n = number of nodes

m = number of edges

## Why is it called breadth-first?

![image-20211105152303847](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105152303847.png)

## Application: shortest path

![image-20211105152506769](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105152506769.png)

![image-20211105152513773](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105152513773.png)

## To find the distance between w and all other vertices v

![image-20211105152530953](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105152530953.png)

## Recap

![image-20211105152716299](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105152716299.png)

## What if the graphs are weighted?

![image-20211105153154271](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153154271.png)

## Dijkstra's algorithm

![image-20211105153212068](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153212068.png)

![image-20211105153221946](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153221946.png)

![image-20211105153232021](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153232021.png)

## Shortest path problem

![image-20211105153244399](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153244399.png)

![image-20211105153256183](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153256183.png)

## A sub-path of a shortest path is also a shortest path

![image-20211105153822565](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105153822565.png)

## Single-source shortest-path problem

![image-20211105154306535](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105154306535.png)

## Example

![image-20211105154332820](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105154332820.png)

![image-20211105154523140](/Kevin_Min/images/2021-11-05-algorithms-week-9/image-20211105154523140.png)

