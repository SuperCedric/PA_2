# Programming Assignment #2 (Numerical Python) #
This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

## No. 1: Normalization Problem ##
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

In this problem, we are tasked to create a 5x5 array containing numbers. I used the ".random.rand()" function in order to create the array so that the user won't have to input 25 numbers in succession. I stored this array into a variable named "X," as tasked by the problem. I then used the .mean and .std functions to find each row's mean and standard deviation, hence why the parameters are "axis=0". I then used these variables along with each data in X to calculate the normalized version of the X array and stored the normalized array in the variable "X_Normalized". This was then saved to a file named "X_Normalized.npy". Lastly, i printed the normalized array so i can verify any syntax errors or logical errors.

## CODE ##
![carbon (7)](https://github.com/user-attachments/assets/270d218b-e3ac-4bd9-a7e9-a7cde5bf8d63)

## OUTPUT ##
![carbon (6)](https://github.com/user-attachments/assets/1a9dd15e-852e-438e-b030-ef27b8ae6179)

## No. 2: Divisble by 3 Problem ##
The Divisible by 3 Problem, in my opinion, was an easier task compared to the Normalization problem.

In this problem, we are tasked to create a 10x10 array that includes the squares of the first 100 integers. In the 10x10 array, we are then tasked to find the numbers divisible by 3, save it in another array, and save it in a .npy file. 
To code this problem, we need to create the 10x10 array first and store it in variable "A". For efficiency, I made sure that the function to create the 10x10 array is created in just 1 line. We can then proceed to check the array for the numbers divisible by 3. These numbers can now be inputted in a separate array, stored in the variable "div". I reshaped the div array to a 3x11 array to make it more pleasant and readable for the user. I then saved this in the .npy file. Additionally, I made sure to print the two arrays so we can check if the arrays generated are logically correct.

## CODE ##
![carbon (5)](https://github.com/user-attachments/assets/71b062ed-ff40-49d9-b802-0674cba723c1)

## OUTPUT ##
![carbon (4)](https://github.com/user-attachments/assets/5db3990c-926b-4662-8e7d-2aa5ae3b276f)
