# Programming Assignment #2 (Numerical Python) #
This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

## No. 1: Normalization Problem ##
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

In this problem, we are tasked to create a 5x5 array and store it in a variable. The first line of code should be importing the Numpy library to be able to use the necessary functions. Once stored in the variable X; it should then be saved in a .npy file. To create the normalized array, I used random floats as my data. Using the .mean() and the .std() functions, each row's mean and standard deviation are calculated and stored in their own separate variables. Using these variables, the mean is subtracted from the element-wise data and then divided by the standard deviation to calculate the normalized data. This is then repeated for all the data given, and this new, normalized array is then stored in variable X_Normalized and saved in a .npy file.

## CODE ##
![carbon](https://github.com/user-attachments/assets/2b72b1b0-8abe-469d-862c-942c66897690)

## OUTPUT ##
![carbon (6)](https://github.com/user-attachments/assets/1a9dd15e-852e-438e-b030-ef27b8ae6179)

## No. 2: Divisble by 3 Problem ##
In this problem, we are tasked to create a 10x10 array that includes the squares of the first 100 integers. In the 10x10 array, we are then tasked to find the numbers divisible by 3, save it in another array, and save it in a .npy file. 
To code this problem, we need to create the 10x10 array first and store it in variable "A". For efficiency, I made sure that the function to create the 10x10 array is created in just 1 line. We can then proceed to check the array for the numbers divisible by 3. These numbers can now be inputted in a separate array, stored in the variable "div". I reshaped the div array to a 3x11 array to make it more pleasant and readable for the viewer. I then saved this in the .npy file. Additionally, I made sure to print the two arrays so we can check if the arrays generated are logically correct.

## CODE ##
![carbon (5)](https://github.com/user-attachments/assets/71b062ed-ff40-49d9-b802-0674cba723c1)

## OUTPUT ##
![carbon (4)](https://github.com/user-attachments/assets/5db3990c-926b-4662-8e7d-2aa5ae3b276f)
