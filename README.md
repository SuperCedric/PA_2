# Programming Assignment #2 (Numerical Python) #
This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

## No. 1: Normalization Problem ##
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

In this problem, we are tasked to create a 5x5 array containing numbers. I used the ".random.rand()" function in order to create the array so that the user won't have to input 25 numbers in succession. I stored this array into a variable named "X," as tasked by the problem. I then used the .mean and .std functions to find each row's mean and standard deviation, hence why the parameters are "axis=0". I then used these variables along with each data in X to calculate the normalized version of the X array and stored the normalized array in the variable "X_Normalized". This was then saved to a file named "X_Normalized.npy". Lastly, i printed the normalized array so i can verify any syntax errors or logical errors.

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
```python
array([[ 1.37056571,  0.92442838,  1.04155734, -0.90441686,  0.72807555],
       [ 0.69595613, -0.42394752, -0.35225163, -0.67510097,  0.4520398 ],
       [-1.17290787, -1.10154428, -1.04611764, -0.84101816,  1.1971176 ],
       [-1.10339242, -0.83341324, -0.96899493,  0.99877331, -1.13006215],
       [ 0.20977845,  1.43447665,  1.32580686,  1.42176269, -1.2471708 ]])
```

## No. 2: Divisble by 3 Problem ##
The Divisible by 3 Problem, in my opinion, was an easier task compared to the Normalization problem.

In this problem, we are tasked to create a 10x10 array that includes the squares of the first 100 integers. In the 10x10 array, we are then tasked to find the numbers divisible by 3, save it in another array, and save it in a .npy file. 
To code this problem, we need to create the 10x10 array first and store it in variable "A". For efficiency, I made sure that the function to create the 10x10 array is created in just 1 line. We can then proceed to check the array for the numbers divisible by 3. These numbers can now be inputted in a separate array, stored in the variable "div". I reshaped the div array to a 3x11 array to make it more pleasant and readable for the user. I then saved this in the .npy file. Additionally, I made sure to print the two arrays so we can check if the arrays generated are logically correct.

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
![carbon (4)](https://github.com/user-attachments/assets/5db3990c-926b-4662-8e7d-2aa5ae3b276f)
