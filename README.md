# Programming Assignment #2 (Numerical Python) #
-This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

## No. 1: Normalization Problem ##
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

In this problem, we are tasked to create a 5x5 square array and save it to variable X. Once stored in the variable X; it should then be saved to a .npy file. To create the normalized array, I used random floats as my data. Using the .mean() and the .std() functions, each row's mean and standard deviation are calculated and stored in their own separate variables. Using these variables, the mean is subtracted from the element-wise data and then divided by the standard deviation to calculate the normalized data. This is then repeated for all the data given, and this new, normalized array is then stored in variable X_Normalized and saved in a .npy file.

## CODE ##
'''python

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
np.save("X_Normalized_npy", X_Normalized)
#Print the normalized array to check for errors
X_Normalized

'''

## OUTPUT ##
![carbon (1)](https://github.com/user-attachments/assets/8bc83976-437e-4452-8412-b792ab8bb855)

