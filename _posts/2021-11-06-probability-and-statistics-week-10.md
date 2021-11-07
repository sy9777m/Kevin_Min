---
toc: true
layout: post
description: Soongsil University 2-2 Probability and Statistics week 10.
categories: [markdown]
title: Probability and Statistics week 10
---
# Probability and Statistics week 10

## point estimation (점 추정)

모르는 분포에 대해서 가장 근사(best guess / best estimate)적인 단일 값을 구하는 것

![image-20211106124712947](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106124712947.png)

## Statistic (통계량)

![image-20211106124816375](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106124816375.png)

### examples of statistic

![image-20211106124922303](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106124922303.png)

## Estimation

![image-20211106125010623](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125010623.png)

![image-20211106125047631](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125047631.png)

1.   데이터를 보고 가능한 분포의 후보를 정함
2.   각 분포를 estimation
3.   best fit distiburion을 찾음 - 보통 한 데이터를 설명할 수 있는 분포에는 여러 종류가 있음

## Example: sample mean vs. population mean

![image-20211106125455695](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125455695.png)

Central Limit Theorem

![image-20211106125538055](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125538055.png)

sample mean의 probability density function을 그려보고 비슷한 distribution을 찾아서 statistical inference

### Example: 기계 고장

![image-20211106125613063](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125613063.png)

## Unbiased estimators (불/비편향 추정량)

![image-20211106125650805](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125650805.png)

### Example: 기계고장

![image-20211106125804710](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125804710.png)

![image-20211106125926479](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106125926479.png)

## Unbiased estimator of variance

![image-20211106130035063](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130035063.png)

## Variance estimator

![image-20211106130045055](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130045055.png)

만약 분포가 n -1이 아니라 n이라면

![image-20211106130306310](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130306310.png)

항상 작게 측정되는 문제가 발생함

## 더 좋은 estimator를 찾는 방법

![image-20211106130342325](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130342325.png)

## Maximum variance unbiased estimator (MVUE)

![image-20211106130448998](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130448998.png)

## Relative efficiency

![image-20211106130541142](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130541142.png)

![image-20211106130556872](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130556872.png)

biased estimator라서 bias가 존재할 경우 서로 bias가 다르고, variance도 다른데 이 경우에는 어떻게 비교해야 할까? 어떤 estimator가 더 좋은 estimator일까?

## Mean Squared Error (MSE)

![image-20211106130647262](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130647262.png)

## Example: 두 개의 estimate의 합

![image-20211106130827670](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130827670.png)

![image-20211106130904671](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130904671.png)

![image-20211106130958085](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106130958085.png)

## Generalization

![image-20211106131027623](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131027623.png)

## Sampling distribution

![image-20211106131102623](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131102623.png)

![image-20211106131218366](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131218366.png)

## Proof

![image-20211106131251192](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131251192.png)

## Parameter를 추정하는 방법

![image-20211106131419878](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131419878.png)

### Example: Uniform distribution

![image-20211106131717037](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131717037.png)

## Example: Gaussian distribution

![image-20211106131835104](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131835104.png)

## Maximum likelihood estimation

![image-20211106131857096](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106131857096.png)

Unbiased estimator임을 보장하지 않음

### Example: Gaussian distribution

![image-20211106132011655](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106132011655.png)

![image-20211106132053382](/Kevin_Min/images/2021-11-06-probability-and-statistics-week-10/image-20211106132053382.png)

