---
title: "Day2"
lastmod: 2020-06-23
date: 2020-06-20
draft: false
---

**Difference between attributes and Methods**

**Attributes** - Returns the value eg arr.dtype
**Methods** - Performs actions/calculations eg.arr.min()

**Difference between series and and Dictionary**

Index can be duplicate in series but not in dictionary


**General points**

1. Sort_values uses quick_sort algorithm to sort the function.

2. Disadvantage of accessing the columns using Dataframe.columns we cannot access the columns which has space ex: column name Total price.

3. If CSV file has integers values with NA it will store the whole data in float data type.

4.  Float will have more memory than int so it is good practice to convert the float to int if it non -decimal number data

5. Converting data in to categorical data will also reduces the memory since data without categorical data type will store each data separately in each memory instead of sharing it.

6. On sorting the data frame the NA values will be by default at last if we want to move it first need to mention na_position='first'
