# Programming Assignment #2 (Numerical Python) #
This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

## No. 1: Normalization Problem ##
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

In this problem, we are tasked to create a 5x5 square array and save it to variable X. Once stored in the variable X; it should then be saved to a .npy file. To create the normalized array, I used random floats as my data. Using the .mean() and the .std() functions, each row's mean and standard deviation are calculated and stored in their own separate variables. Using these variables, the mean is subtracted from the element-wise data and then divided by the standard deviation to calculate the normalized data. This is then repeated for all the data given, and this new, normalized array is then stored in variable X_Normalized and saved in a .npy file.

## CODE ##
![image](https://github.com/user-attachments/assets/6423382f-3cad-49af-84c8-5071e255c2a6)

## OUTPUT ##
![carbon (1)](https://github.com/user-attachments/assets/8bc83976-437e-4452-8412-b792ab8bb855)

