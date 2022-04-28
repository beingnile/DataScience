# NumPy

NumPy, or Numerical Python, is a python library used for working with arrays. It also has functions for working in domain of linear algebra, fourier transform, and matrices.

## Installation


```sh

pip3 install numpy

```

## Usage

```py

# To use numpy, you have to import the package in your python scripts
import numpy as np

```

## NumPy arrays

Python lists are inbuilt powerful data structures.  
They can store values of different types and they are easy to use.  
Moreover, lists support operations like deletion and addition of elements.
Lists however do not support mathematical operations over collections besides being slow to process.  
An elegant solution for the lists short-comings, is the NumPy arrays.  
NumPy arrays are more or less like lists. They are however faster than the traditional Python lists.  
They also support mathematical operations over collections.  
Suppose that we have two different lists that contain the height in meters and weight in kilograms of a group of people.  

```py

height = [1.53, 1.62, 1.74, 1.65]

weight = [55.03, 60.11, 85.78, 60.22]

```

To calculate the BMI of each person, you would assume that `weight / height ** 2` would work, right?  
The calculation throws an error: `TypeError: unsupported operand type(s) for ** or pow(): 'list' and 'int'`  

### Using NumPy arrays

```py

np.array(weight) / np.array(height) ** 2

# Output
array([23.50805246, 22.90428288, 28.33267274, 22.11937557])

```

Converting both weight and height to numpy arrays enables us to perform element-wise mathematical operations.
