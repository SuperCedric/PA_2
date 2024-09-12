<a name="top"></a>

# PA 2: NUMERICAL PYTHON # 
This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

### GIVEN PROBLEMS ###
#### 1. Normalization Problem ####
  - In this problem, we are tasked to create a 5x5 array, `X`, containing random numbers and normalize it by subtracting the mean and dividing by the standard deviation. Use `.mean()` and `.std()` for element-wise calculations, and save the normalized array as `X_normalized.npy`.
#### 2. Divisible by 3 Problem ####
   - Create a 10x10 array with the squares of the first 100 positive integers. Identify all elements divisible by 3 and save the result as `div_by_3.npy`.

## 1️⃣ Normalization Problem ##
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

### Documentation ###
In this task, a 5x5 array, stored in variable `X`, was generated using the `.random.rand()` function to avoid manual input. The array was normalized by calculating the mean and standard deviation for each row using `.mean()` and `.std()` with `axis=0`. The normalized array was stored in `X_Normalized` and saved as `X_Normalized.npy`. Finally, the normalized array was printed to verify correctness

## CODE ##
```python
#import the numpy library to use its functions
import numpy as np

#assign a random float between 1 and 0 in a 5x5 array
X = np.random.rand(5,5)
#find the mean
mean = X.mean(axis=0)
#find the standard deviation
sd = X.std(axis=0)
#normalize the array using the given formula
X_Normalized =  ((X - mean) / (sd))
#save the array in the properly named file
np.save("X_Normalized.npy", X_Normalized)
#Print the normalized array to check for errors
X_Normalized
```

## OUTPUT ##
```
array([[ 1.37056571,  0.92442838,  1.04155734, -0.90441686,  0.72807555],
       [ 0.69595613, -0.42394752, -0.35225163, -0.67510097,  0.4520398 ],
       [-1.17290787, -1.10154428, -1.04611764, -0.84101816,  1.1971176 ],
       [-1.10339242, -0.83341324, -0.96899493,  0.99877331, -1.13006215],
       [ 0.20977845,  1.43447665,  1.32580686,  1.42176269, -1.2471708 ]])
```

## 2️⃣ Divisible by 3 Problem ##
The Divisible by 3 Problem, in my opinion, was an easier task compared to the Normalization problem.

### Documentation ###

To code this problem, a 10x10 array, `A` was created in one line for efficiency. Next, elements divisible by 3 were extracted and stored in a new array, `div`, which was reshaped to a 3x11 array for better readability. The result was saved as a `.npy` file, and both arrays were printed to verify their correctness.

## CODE ##
```python
#import the NumPy library to use its functions
import numpy as np
#assign the squared numbers into a 10x10 array
A = np.arange(1,101).reshape(10,10) ** 2
#find the numbers that are divisible by 3 element-wise and assign it to a variable
div = A[A % 3 == 0].reshape(3,11)
#Print the two arrays so we can check for any logic errors
print("The 10x10 array is given as: \n", A)
print("The elements divisible by 3 are: \n", div)
#save the divisible by 3 array into the properly named file
np.save("div_by_3.npy", div)
```
## OUTPUT ##
```
The 10x10 array is given as: 
 [[    1     4     9    16    25    36    49    64    81   100]
 [  121   144   169   196   225   256   289   324   361   400]
 [  441   484   529   576   625   676   729   784   841   900]
 [  961  1024  1089  1156  1225  1296  1369  1444  1521  1600]
 [ 1681  1764  1849  1936  2025  2116  2209  2304  2401  2500]
 [ 2601  2704  2809  2916  3025  3136  3249  3364  3481  3600]
 [ 3721  3844  3969  4096  4225  4356  4489  4624  4761  4900]
 [ 5041  5184  5329  5476  5625  5776  5929  6084  6241  6400]
 [ 6561  6724  6889  7056  7225  7396  7569  7744  7921  8100]
 [ 8281  8464  8649  8836  9025  9216  9409  9604  9801 10000]]
The elements divisible by 3 are: 
 [[   9   36   81  144  225  324  441  576  729  900 1089]
 [1296 1521 1764 2025 2304 2601 2916 3249 3600 3969 4356]
 [4761 5184 5625 6084 6561 7056 7569 8100 8649 9216 9801]]
```

### BUILT WITH ###
 - Jupyter Notebook

### LIBRARIES USED ###
 - PYTHON
    - Numpy

### AUTHOR ###
 - Cedric Kurt Taguba - [@SuperCedric](https://github.com/SuperCedric)


<p align="right">(<a href="#top">[🔼GO TO TOP]</a>)</p>
