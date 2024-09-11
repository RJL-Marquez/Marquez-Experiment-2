# Marquez Experiment #2
## 1. Normalization Problem

  In this problem, create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized ndarray as X_normalized.npy
  
  ### Importing numpy
```python
#Normalization Problem
#importing numpy
import numpy as np
```
  ### Initializing the random 5x5 ndarray
```python
#Creating a random 5 x 5 ndarray
X = np.random.random((5,5))
X
```
  ### Calculating for the Mean
```python
#Finding the Mean of the random elements
m = np.mean(X)
m
```
  ### Calculating for the Standard Deviation
```python
#Finding the Standard Dev. of the random elements
s = np.std(X)
s
```
  ### Calculating for the Z
```python
#Normalizing the random elements using the formula: Z=(X-m)/s
Z = ((X-m)/s)
Z
```
 ### Saving the result in a local .npy file
```python
#Saving the result as X_normalized.npy
np.save('X_normalized', Z)

#End of Code
```

## 2. Divisible By 3 Problem

Create a 10 x 10 ndarray, which includes squares of the first 100 positive integers. From this ndarray, determine all the elements that are divisible by 3. Save the result as div_by_3.npy
  
  ### Importing numpy
```python
#Divisible By 3 Problem
#importing numpy
import numpy as np
```
  ### Generating the given ndarray
```python
#Generating the ndarray
A = np.arange(1,101).reshape(10,10)
A = np.square(A)
A
```
  ### Filtering all values divisible by 3
```python
#Filtering the elements divisible by 3
B = A[A % 3 == 0]
B
```
  ### Saving the result in a local .npy file
```python
#Saving the result as div_by_3.npy
np.save('div_by_3', B)

#End of Code
  ```
