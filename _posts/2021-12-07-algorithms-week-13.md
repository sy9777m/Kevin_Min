---
toc: true
layout: post
description: Soongsil University 2-2 Algorithms week 13.
categories: [markdown]
title: Algorithms week 13
---
# Algorithms week 13

## Outline

![image-20211207124410764](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207124410764.png)

## Greedy algorithms

![image-20211207125150921](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125150921.png)

## Non-example

![image-20211207125159135](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125159135.png)

![image-20211207125207413](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125207413.png)

## Activity selection

### Example where greedy works

![image-20211207125230959](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125230959.png)

## Activity selection

![image-20211207125243425](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125243425.png)

## Greedy algorithm

![image-20211207125255106](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125255106.png)

![image-20211207125643256](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125643256.png)

![image-20211207125650404](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125650404.png)

![image-20211207125659201](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125659201.png)

![image-20211207125707809](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125707809.png)

![image-20211207125714728](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125714728.png)

![image-20211207125723888](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125723888.png)

![image-20211207125731144](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125731144.png)

## At least it's fast

![image-20211207125743376](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125743376.png)

## What makes it greedy?

![image-20211207125758193](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207125758193.png)

## Three questions

![image-20211207130139784](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130139784.png)

## Answers

![image-20211207130150462](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130150462.png)

## Back to activity selection

![image-20211207130204867](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130204867.png)

## Why does it work?

![image-20211207130216147](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130216147.png)

## Assuming we can prove that

![image-20211207130228086](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130228086.png)

## We never rule out an optimal solution

![image-20211207130521888](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130521888.png)

![image-20211207130532927](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130532927.png)

![image-20211207130541551](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130541551.png)

![image-20211207130550915](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130550915.png)

![image-20211207130601278](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130601278.png)

![image-20211207130610059](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130610059.png)

![image-20211207130631355](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130631355.png)

## So the algorithm is correct

![image-20211207130650827](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207130650827.png)

## Sub-problem graph view

![image-20211207131200965](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131200965.png)

![image-20211207131207103](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131207103.png)

![image-20211207131214932](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131214932.png)

![image-20211207131223065](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131223065.png)

## Answers

![image-20211207131233461](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131233461.png)

## Another example: Huffman coding

![image-20211207131250435](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131250435.png)

![image-20211207131258723](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131258723.png)

## Suppose we have some distribution on characters

![image-20211207131316733](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131316733.png)

## Try 0

![image-20211207131323243](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131323243.png)

![image-20211207131328719](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131328719.png)

![image-20211207131805446](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131805446.png)

## Try 1

![image-20211207131828773](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131828773.png)

## Try 2: prefix-free coding

![image-20211207131851032](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131851032.png)

![image-20211207131907776](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131907776.png)

![image-20211207131916155](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131916155.png)

![image-20211207131924584](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131924584.png)

## A prefix-free code is a tree

![image-20211207131940349](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131940349.png)

## Some trees are better than others

![image-20211207131953121](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207131953121.png)

## Question

![image-20211207132002609](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132002609.png)

## Optimal sub-structure

![image-20211207132012989](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132012989.png)

## In order to design a greedy algorithm

![image-20211207132026488](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132026488.png)

## Solution

greedily build subtrees, starting with the infrequent letters

![image-20211207132045635](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132045635.png)

![image-20211207132054696](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132054696.png)

![image-20211207132100843](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132100843.png)

![image-20211207132107452](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132107452.png)

![image-20211207132116352](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132116352.png)

![image-20211207132125129](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132125129.png)

## What exactly was the algorithm?

![image-20211207132138686](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132138686.png)

## Does it work?

![image-20211207132717578](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132717578.png)

## What have we learned?

![image-20211207132729107](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132729107.png)

## Recap I

![image-20211207132738317](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132738317.png)

## Minimum spanning tree

![image-20211207132748707](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132748707.png)

## Minimum spanning tree

![image-20211207132800492](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207132800492.png)

![image-20211207133312410](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133312410.png)

![image-20211207133320125](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133320125.png)

![image-20211207133327857](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133327857.png)

![image-20211207133335355](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133335355.png)

## Why MSTs?

![image-20211207133352369](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133352369.png)

## Idea 1

![image-20211207133405724](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133405724.png)

![image-20211207133413229](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133413229.png)

![image-20211207133420158](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133420158.png)

![image-20211207133427278](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133427278.png)

![image-20211207133434180](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133434180.png)

![image-20211207133441720](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133441720.png)

![image-20211207133449792](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133449792.png)

![image-20211207133455751](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133455751.png)

## We've discovered Prim's algorithm!

![image-20211207133518905](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207133518905.png)

## Question

![image-20211207134032338](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134032338.png)

## How do we actually implement this?

![image-20211207134047136](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134047136.png)

![image-20211207134148373](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134148373.png)

![image-20211207134136742](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134136742.png)

## Efficient implementation

![image-20211207134430747](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134430747.png)

![image-20211207134445691](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134445691.png)

![image-20211207134453471](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134453471.png)

![image-20211207134502336](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134502336.png)

![image-20211207134511684](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134511684.png)

![image-20211207134519342](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134519342.png)

![image-20211207134527768](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134527768.png)

![image-20211207134535359](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134535359.png)

![image-20211207134543507](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134543507.png)

![image-20211207134552336](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134552336.png)

![image-20211207134601368](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134601368.png)

![image-20211207134609199](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134609199.png)

![image-20211207134618035](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134618035.png)

![image-20211207134625973](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134625973.png)

![image-20211207134632861](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134632861.png)

![image-20211207134640126](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134640126.png)

![image-20211207134646017](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134646017.png)

## This should look pretty familiar

![image-20211207134700872](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207134700872.png)

## One thing that is similar: running time

![image-20211207135209167](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135209167.png)

## Code

![image-20211207135217731](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135217731.png)

## That's not the only greedy algorithm

![image-20211207135232436](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135232436.png)

![image-20211207135240236](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135240236.png)

![image-20211207135257433](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135257433.png)

![image-20211207135303049](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135303049.png)

![image-20211207135308324](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135308324.png)

![image-20211207135312825](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135312825.png)

![image-20211207135321039](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135321039.png)

![image-20211207135329210](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135329210.png)

![image-20211207135334453](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135334453.png)

![image-20211207135339882](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135339882.png)

## We've discovered Kruskal's algorithm!

![image-20211207135355389](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207135355389.png)

## Question

![image-20211207140949415](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207140949415.png)

## At each step of Kruskal's, we are maintaining a forest

![image-20211207141009574](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141009574.png)

![image-20211207141015822](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141015822.png)

![image-20211207141022055](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141022055.png)

![image-20211207141028740](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141028740.png)

![image-20211207141034734](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141034734.png)

## Union-find data structure also called disjoint-set data structure

![image-20211207141052286](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141052286.png)

![image-20211207141058341](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141058341.png)

![image-20211207141104364](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141104364.png)

## Kruskal pseudo-code

![image-20211207141117012](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141117012.png)

## Once more...

![image-20211207141448215](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141448215.png)

![image-20211207141454494](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141454494.png)

![image-20211207141501260](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141501260.png)

![image-20211207141506607](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141506607.png)

![image-20211207141512251](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141512251.png)

![image-20211207141517618](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141517618.png)

![image-20211207141524970](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141524970.png)

![image-20211207141531540](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141531540.png)

![image-20211207141538068](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141538068.png)

![image-20211207141541742](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141541742.png)

## Running time

![image-20211207141551496](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141551496.png)

## Compare and contrast

![image-20211207141601905](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141601905.png)

## Both Prim and Kruskal

![image-20211207141612359](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141612359.png)

## Recap

![image-20211207141621642](/Kevin_Min/images/2021-12-07-algorithms-week-13/image-20211207141621642.png)
