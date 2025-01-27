Numpy Tutorial

![Numpy Logo](https://upload.wikimedia.org/wikipedia/commons/2/20/Numpy_logo_2020.svg)

This tutorial covers **NumPy**, a fundamental package for scientific computing with Python. NumPy is used for handling large multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays. It is one of the core libraries in data science and machine learning.

## Table of Contents

- [Introduction to NumPy](#introduction-to-numpy)
- [Creating Arrays](#creating-arrays)
- [Array Operations](#array-operations)
- [Array Indexing and Slicing](#array-indexing-and-slicing)
- [Mathematical Functions](#mathematical-functions)
- [Linear Algebra with NumPy](#linear-algebra-with-numpy)
- [Random Module](#random-module)
- [Reshaping Arrays](#reshaping-arrays)
- [Broadcasting](#broadcasting)

---

## Introduction to NumPy

NumPy is one of the most important packages in Python for scientific computing, providing support for large multi-dimensional arrays and matrices. It also includes mathematical functions to perform operations on these arrays efficiently.

To install NumPy, use:
```bash
pip install numpy


---

Creating Arrays

The most important feature of NumPy is its ndarray, a multidimensional array object that allows us to store data efficiently. You can create a NumPy array from a list, tuple, or other sequences.

Example: Create a Simple Array

import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr)

Example: Create a 2D Array

arr2d = np.array([[1, 2, 3], [4, 5, 6]])
print(arr2d)


---

Array Operations

NumPy supports a wide range of operations, including element-wise arithmetic operations, matrix multiplication, and more.

Example: Element-Wise Addition

arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
result = arr1 + arr2
print(result)

Example: Scalar Operations

arr = np.array([1, 2, 3])
result = arr * 2
print(result)


---

Array Indexing and Slicing

NumPy arrays can be indexed and sliced similar to Python lists, but with added capabilities such as multi-dimensional indexing.

Example: Indexing a 2D Array

arr2d = np.array([[1, 2, 3], [4, 5, 6]])
print(arr2d[0, 2])  # Accessing element in first row and third column

Example: Slicing a 2D Array

arr2d = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print(arr2d[0:2, 1:3])  # Accessing a submatrix


---

Mathematical Functions

NumPy provides a vast collection of mathematical functions for performing calculations on arrays. These include functions for trigonometry, statistics, linear algebra, and more.

Example: Basic Mathematical Operations

arr = np.array([1, 2, 3])
print(np.sqrt(arr))  # Square root of each element
print(np.exp(arr))   # Exponential of each element

Example: Statistical Operations

arr = np.array([1, 2, 3, 4, 5])
print(np.mean(arr))  # Mean
print(np.std(arr))   # Standard Deviation


---

Linear Algebra with NumPy

NumPy provides functions for linear algebra operations, such as matrix multiplication, determinant calculation, eigenvalues, and more.

Example: Matrix Multiplication

arr1 = np.array([[1, 2], [3, 4]])
arr2 = np.array([[5, 6], [7, 8]])
result = np.dot(arr1, arr2)
print(result)

Example: Determinant

arr = np.array([[1, 2], [3, 4]])
print(np.linalg.det(arr))  # Determinant of the matrix


---

Random Module

The numpy.random module provides functions for generating random numbers and performing random sampling.

Example: Generate Random Numbers

rand_arr = np.random.rand(3, 2)  # Random numbers from a uniform distribution
print(rand_arr)

Example: Random Integer Generation

rand_ints = np.random.randint(1, 10, size=(3, 3))  # Random integers between 1 and 10
print(rand_ints)


---

Reshaping Arrays

You can reshape an array to fit your needs, turning it into a different shape without changing its data.

Example: Reshaping an Array

arr = np.array([1, 2, 3, 4, 5, 6])
reshaped_arr = arr.reshape(2, 3)
print(reshaped_arr)


---

Broadcasting

Broadcasting is a powerful feature that allows NumPy to perform arithmetic operations on arrays of different shapes. The smaller array is "broadcast" over the larger array so that they have compatible shapes.

Example: Broadcasting

arr1 = np.array([1, 2, 3])
arr2 = np.array([[1], [2], [3]])
result = arr1 + arr2
print(result)


---

Conclusion

This tutorial provided an in-depth exploration of NumPy, covering essential topics such as array creation, operations, slicing, linear algebra, and more. NumPy is the foundational library for numerical computing in Python, and mastering it will greatly enhance your ability to work with scientific data.

For more advanced topics and examples, visit the official NumPy documentation: https://numpy.org/

Feel free to modify and experiment with the code examples provided!

### How to Use:
1. **Installation**: Ensure you have NumPy installed with `pip install numpy`.
2. **Explore**: Use the provided code examples to explore and learn about various NumPy features.
3. **Practice**: Try modifying the code and running your own examples to gain a deeper understanding of how NumPy works.

Let me know if you need additional modifications or further clarifications!
