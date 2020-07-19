---
title: "Day3"
lastmod: 2020-07-19
date: 2020-07-19
draft: false
---

#### Day 3 - Pandas - Series 

These upcoming blogs is regarding Pandas which is an library in python which helps to load, cleanse and pre-process the data which will be passed in to Machine learning algorithm.

My main resource will be Pandas - Udemy course. Also I have reffered some offical website of Pandas.

**Series:**

Series is one Dimesion where else pandas as two dimensions.

**Importing Series**

Series=pd.read_csv("filename.csv",squeeze=True,usecols={colname}) 

Squeeze should be set as true for Series,

We can convert list, tuples, Dict to Series by using pd.Series(list/tuple/dict)

**Attributes of Series**

Eg: Series.values,
Other examples are: index,dtype,isunique,ndim,shape,size,name

Above mentioned are self expalantory.

**Important Methods of Series**

1. Common function: sum(),product(),mean(),std(),min(),max(),median(),mode()
2. describe(),idxmax(),idmin(),value_counts()
3. apply(function)-> helps to apply a function you can apply lambada func too
4. map (series2)->mapping  returns the values matched (we can also use dic for map parameter)
5. Sorting -> sort_values(inplace=True,ascending=True)
6. Sortingindex -> sort_index(inplace=True,ascending=True)
7. reindex(index=['a','b']) if any of mentioned index has no values it will assign as NAN
8. rest_index
9. Series.get('index',default="There is nothing in it") -> get the mentioned values if no value is there it will print the default value

**in Operator**

1. 100 in series.index -> Returns Boolean
2. "NAME" in series.values -> Returns Boolean

**Extracting Data**
1. series[10] -> 10 th Row
2. series[1:20] -> 1 to 20 Rows
3. series[1:-3] 1 to 7
4. series[-5:-1] 5 to 7
5. series[[10,20,30]]
6. series['a':'b':2] -> 2 skips