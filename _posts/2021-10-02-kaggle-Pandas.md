---
toc: true
layout: post
description: Kaggle course Pandas for Find-A.
categories: [markdown]
title: Kaggle Pandas
---
# kaggle Pandas

## Creating, Reading and Writing

![image-20211002094657783](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002094657783.png)

![image-20211002094819228](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002094819228.png)

## Indexing, Selecting & Assigning

### Indexing in pandas

![image-20211002095402026](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002095402026.png)

![image-20211002095420960](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002095420960.png)

## Summary Functions and Maps

![image-20211002100732122](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002100732122.png)

### Maps

A **map** is a term, borrowed from mathematics, for a function that takes one set of values and "maps" them to another set of values.

![image-20211002100817452](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002100817452.png)

The function you pass to `map()` should expect a single value from the Series (a point value, in the above example), and return a transformed version of that value. `map()` returns a new Series where all the values have been transformed by your function.

![image-20211002100913583](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002100913583.png)

![image-20211002101001344](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002101001344.png)

### Exercise

```python
descriptor_counts = pd.Series([reviews['description'].map(lambda x: 'tropical' in x).sum(), reviews['description'].map(lambda x: 'fruity' in x).sum()], index=['tropical', 'fruity'])
# descriptor_counts

# Check your answer
q6.check()
```

## Grouping and Sorting

### Groupwise analysis

`groupby()` created a group of reviews which allotted the same point values to the given wines. Then, for each of these groups, we grabbed the `points()` column and counted how many times it appeared. `value_counts()` is just a shortcut to this `groupby()` operation.

![image-20211002145008983](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145008983.png)

![image-20211002145105647](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145105647.png)

![image-20211002145157713](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145157713.png)

Another `groupby()` method worth mentioning is `agg()`, which lets you run a bunch of different functions on your DataFrame simultaneously. For example, we can generate a simple statistical summary of the dataset as follows:

![image-20211002145227678](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145227678.png)

### Multi-indexes

![image-20211002145549134](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145549134.png)

Multi-indices have several methods for dealing with their tiered structure which are absent for single-level indices. They also require two levels of labels to retrieve a value.

![image-20211002145648037](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145648037.png)

### Sorting

`sort_values()` defaults to an ascending sort, where the lowest values go first. However, most of the time we want a descending sort, where the higher numbers go first.

![image-20211002145731562](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145731562.png)

![image-20211002145742868](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002145742868.png)

## Data Types and Missing Values

### Dtypes

The data type for a column in a DataFrame or a Series is known as the **dtype**.

![image-20211002152246617](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002152246617.png)

`float64` means that it's using a 64-bit floating point number; `int64` means a similarly sized integer instead, and so on.

One peculiarity to keep in mind (and on display very clearly here) is that columns consisting entirely of strings do not get their own type; they are instead given the `object` type.

It's possible to convert a column of one type into another wherever such a conversion makes sense by using the `astype()` function.

![image-20211002152325928](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002152325928.png)

### Missing data

Entries missing values are given the value `NaN`, short for "Not a Number". For technical reasons these `NaN` values are always of the `float64` dtype.

Pandas provides some methods specific to missing data. To select `NaN` entries you can use `pd.isnull()` (or its companion `pd.notnull()`). This is meant to be used thusly:

![image-20211002152400996](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002152400996.png)

Replacing missing values is a common operation. Pandas provides a really handy method for this problem: `fillna()`. `fillna()` provides a few different strategies for mitigating such data.

![image-20211002152429049](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002152429049.png)

Or we could fill each missing value with the first non-null value that appears sometime after the given record in the database. This is known as the backfill strategy.

![image-20211002152459962](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002152459962.png)

## Renaming and Combining

### Renaming

![image-20211002153750555](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002153750555.png)

![image-20211002153803885](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002153803885.png)

![image-20211002153827767](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002153827767.png)

### Combining

![image-20211002153859890](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002153859890.png)

![image-20211002153919768](/Kevin_Min/images/2021-10-02-kaggle-Pandas/image-20211002153919768.png)

