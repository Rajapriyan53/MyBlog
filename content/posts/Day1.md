---
title: "Day1"
lastmod: 2020-06-23
date: 2020-06-20
draft: false
---

## Numpy

NumPy is a package in Python used for Scientific Computing. NumPy package is used to perform different operations. The ndarray (NumPy Array) is a multidimensional array used to store values of same datatype. These arrays are indexed just like Sequences, starts with zero.

Here some of the important numpy array functions and properties.

### Importing and Exporting Options(Np. will be used to call the function)

1. np.loadtxt('filename.txt') -> To load text file the path will be given in the parameter

2. np.genfromtxt('file.csv', delimiter=',') -> To load csv file the path will be given in the parameter along with that delimiter will be also provided

3. np.load(demp.npy) -> To load the saved numpy array
Allow pickle is optional in this parameter and it will restrict pickle data of the file if it set as true.

4. np.savetxt('filename', delimiter='') -> to save text file.

Note to save csv file delimter=','(comma) will be used.

### Scalar (Np. will be used to call the function)

1. np.add(arr,1) -> add 1 to all element

2. np.subract(arr,arr2) ->add arr and arr2

3. mulitply(), divide(), sqrt()

4. power(arr,2) or power(arr1, arr2)

5. array_equal(arr1,arr2)

6. sin(arr) ,log(arr), abs(arr), ceil(arr), floor(arr), round(arr)

Above are some of the functions which will perform actions according to the name of the functions.

### Statistics ( arr will be used to call the function, axis will be parameter to mention row/column)
0-> row and 1 -> column

1. arr.sum() , min(), max(), corrcoef()

2. np.var(arr), std(arr), mean(arr,axis=0/1)

### Combining/Splitting (NP)

1. np.concatenate((arr,arr2),axis=0/1)

2. np. split(arr,3) -> Splits arr to 3 subarray

3. np.hsplit(arr,5) -> Horizontal split to 5 subarray

### Adding/Removing Elements (NP)

1. np.append(arr,values,axis=0/1) -> Inserts at last

2. np.insert(arr,position,values,axis)

3. np.delete(arr,position,axis)

### Inspecting Properties (arr)

1. arr.size -> Size of array

2. arr.shape ->Shape of array

3. arr.dtype -> Returns datatype

Note: These are not functions they are called attributes

4. arr.astype(dtype) -> Convert to other data type

6. arr.tolist() -> Convert to Python list

### Generic functions (NP)

1. np.info(np.eye) -> Shows info about the nupy function

### Copying/sorting/Reshaping (arr)

2. np.copy(arr) -> Copies array

3. arr.view(dtype) -> creates view in specified data type.

4. arr.sort(axis=1)-> sort arrays

5. two_d_arr.flatten() - > flattens two d array to one dimension

6. arr.T - Transpose array

7. arr.reshape(3,4) -> reshapes array

8. arr.resize(5,6) -> changes shapes to 5X6 and fills values with 0)

Difference between reshape and resize is resize modifies the original data.

### Creating Array (NP)

1. np.array()

2. np.zeros(3)

3. np.ones((2,3))

4. np.eye(N,M,k,dtype,Order) -> Returns identical matrix (N-> row, M-> column,K=0 main diagonal, positive -> upper, negative -> lower, Order->{C/f}row/column wise store in memory)

5. np.linspace(1,10,4) -> Gives (1.0,3.0,5.0,7.0) Array of 5 evenly divided values from 0 to 10

6. np.arange(0,10,3) -> Gives (0,3,6,9) Array from 0 to 10 with step 3

7. np.full((2,3),8) 2X3 array with all values 8

8. np.random.rand(4,5) -> 4X5 array with random float values (0 -1)

9. np.random.rand(4,5)** 100  -> same but with random values (0 to 100)

10. np.random.randint(5,size=(2,3)) ->2X3 array with random value 0-4

### Indexing/Slicing/Subsetting

1. arr[0:3] Return the element from rows 0 to 2

2. arr[0:3,4] Return the element from 0 to 2 of the 4 th column

3. arr[:2] Return the element from beginning to 1 that is 0 and 1

4. arr[:,1] Return every row of column 1 elements

5. arr[arr<5] - Return elements which is less than 5

6. ~arr - inverts an boolean array


Note:
Mostly Every function will be called using np but Array will be used functions like converting,view,Reshape,resize,sort,min,max,sum,slicing/indexing,co relation, transpose. And also for attributes array will be used to call the attributes(Shapes,size,Dtype)


** Adding Some more functions used **
1. np.squeeze() -> Remove single-dimensional entries from the shape of an array.

Eg:x = np.array([[[0], [1], [2]]])

x.shape
(1, 3, 1)

np.squeeze(x).shape
(3,)

np.squeeze(x, axis=0).shape
(3, 1)

2. np.expand_dims() -> Insert a new axis that will appear at the axis position in the expanded array shape.

Eg: x = np.array([1, 2])

x.shape
(2,)

y = np.expand_dims(x, axis=1)

y
array([[1],
       [2]])

y.shape
(2, 1)
