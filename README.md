`ECE2112: Advanced Computer Programming and Algorithms`
## EXPERIMENT 2: NUMERICAL PHYTON (NUMPY)

### I. Intended Learning Outcomes:

1. To identify the codes and functions inncorporated in the Numpy library.
3. To be able to apply and use different codes and functions in ceating a Python program using a Numpy library.

### II. Instructions:

Write a Python script/code in the Jupyter Notebook to do the given problems. You may submit your Jupyter Notebook in the dedicated submission bin.

### III. Problems:
## NORMALIZATION PROBLEM
Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data  from the mean and scaling means dividing with its standard deviation. Mathematically, normaliaztion can be expressed as:  

![Math](https://github.com/user-attachments/assets/d25aecb2-c49c-4521-bcf3-69d455347dc0)  

In Python, element-wise mean and element-wise standard deviation can be obtained by using .mean() and std() calls.

In this problem, create a random 5 x 5 ndarray and store it to variable X. Normalize X. Save your normalized ndarray as *X_normalized.npy*

  - A NumPy matrix of size 5×5 is created with random numbers, and its mean and standard deviation are computed using the functions. mean () and. std (), respectively. The normalized array will then be obtained as follows: each element will have the mean subtracted from it and divided by the standard deviation, giving data centered at zero with unit variance. In the end, *X_normalized.npy* should contain the normalized array.

```
Pseudocode:
1. Import NumPy.
2. Make a 5x5 array of random numbers assign to X.
3. Compute overall mean of X assign to mean.
4. Compute overall standard deviation of X assign to std
5. Compute normalized array assign to X_normalized = (X - m) / s
6. Save as X_normalized.npy
7. Print
```

## DIVISIBLE BY 3 PROBLEM
Create the following 10 x 10 ndarray.

![Table](https://github.com/user-attachments/assets/97eb706e-ba29-40a4-b7bb-c8637c074176)  

which are the squares of the firts 100 positive integers.  

From this ndarray, determine all the elements that are divisible by 3. Save the resuult as *div_by_3.npy*

   - In this problem: Let us first generate the first 100 positive integers: np.arange(1, 101), squaring them gives the sequence of perfect squares, reshaping it into a matrix of size 10×10, and thereafter applying a Boolean mask (A % 3 == 0) to select only those elements divisible by 3. Store that value over to a new array and save that as div_by_3.npy. Both of the above mentioned problems depend on the capability of NumPy to generate an array, make mathematical computations, and store them in an efficient manner with the minimum memory consumption.

```
Pseudocode:
1. Import NumPy.
2. Create integers from 1 to 100, assign to numbers = arange(1, 101).
3. Square them then assign to sq == numbers**2.
4. Reshape to 10x10 assign to A = reshape(sq, (10, 10)).
6. Extract the values assign to div_by_3 = A[A % 3 == 0].
7. Save div_by_3.npy
8. Print 
```

**Harvey Aaron E. Orzal**  
**2ECE - B**



