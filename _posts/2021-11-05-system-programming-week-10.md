---
toc: true
layout: post
description: Soongsil University 2-2 System Programming week 10.
categories: [markdown]
title: System Programming week 10
---
# System Programming week 10

## Random-Access Memory (RAM)

![image-20211105044533457](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105044533457.png)

## SRAM vs. DRAM summary

![image-20211105044722848](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105044722848.png)

## Nonvolatile memories

![image-20211105044811282](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105044811282.png)

## Traditional bus structure connecting CPU and memory

![image-20211105045057795](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045057795.png)

## Memory read transaction

![image-20211105045208162](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045208162.png)

![image-20211105045212633](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045212633.png)

![image-20211105045222250](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045222250.png)

![image-20211105045228105](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045228105.png)

![image-20211105045233171](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045233171.png)

![image-20211105045237172](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045237172.png)

## What's inside a disk drive?

![image-20211105045349573](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045349573.png)

## Disk geometry

![image-20211105045402870](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045402870.png)

![image-20211105045523609](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045523609.png)

## Disk capacity

![image-20211105045534589](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045534589.png)

## Recording zones

![image-20211105045825242](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045825242.png)

## Computing disk capacity

![image-20211105045954225](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105045954225.png)

## Disk operation (single-platter view)

![image-20211105050057842](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050057842.png)

## Disk operation (multi-platter view)

![image-20211105050244248](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050244248.png)

## Disk structure - top view of single platter

![image-20211105050303081](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050303081.png)

## Disk access

![image-20211105050312625](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050312625.png)

![image-20211105050317570](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050317570.png)

![image-20211105050322008](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050322008.png)

![image-20211105050327362](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050327362.png)

![image-20211105050333026](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050333026.png)

![image-20211105050341107](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050341107.png)

![image-20211105050346698](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050346698.png)

![image-20211105050353387](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050353387.png)

![image-20211105050402110](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050402110.png)

## Disk access time

![image-20211105050412211](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050412211.png)

![image-20211105050619395](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050619395.png)

## Logical disk blocks

![image-20211105050750980](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105050750980.png)

## I/O bus

![image-20211105051056494](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051056494.png)

## Reading a disk sector

![image-20211105051108819](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051108819.png)

![image-20211105051239548](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051239548.png)

![image-20211105051248387](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051248387.png)

## Solid State Disks (SSDs)

![image-20211105051431580](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051431580.png)

## SSD tradeoffs vs. rotating disks

![image-20211105051715488](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051715488.png)

## The CPU-memory gap

![image-20211105051857954](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105051857954.png)

## Locality to the rescue!

![image-20211105052014751](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052014751.png)

## Example memory hierarchy

![image-20211105052109127](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052109127.png)

## Locality

![image-20211105052027082](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052027082.png)

![image-20211105052047171](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052047171.png)

## Qualitative estimates of locality

![image-20211105052421509](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052421509.png)

## Locality example

![image-20211105052507969](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052507969.png)

![image-20211105052519356](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052519356.png)

## Memory hierarchies

![image-20211105052533333](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052533333.png)

## Caches

![image-20211105052923955](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105052923955.png)

## General cache concepts

![image-20211105053032275](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105053032275.png)

![image-20211105053055659](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105053055659.png)

![image-20211105053103069](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105053103069.png)

## General caching concepts: types of cache misses

![image-20211105053123155](/Kevin_Min/images/2021-11-05-system-programming-week-10/image-20211105053123155.png)

