# Programming Assignment #2 (Numerical Python)
-This repository includes my solution to the two given problems involving the Numpy library. Respectively, the first and second problem are the *Normalization Problem* and the *Divisible by 3 Problem*.

## No. 1: Normalization Problem
Normalization, simply put, is a way to clean up a collection of data to make it **clearer** and **more machine-readable**.

In this problem, we are tasked to create a 5x5 square array and save it to variable X. Once stored in the variable X, it should then be saved to a .npy file.
To create the normalized array, I used random floats as my data. Using the .mean() and the .std() function, the mean and standard deviation of each row is then calculated and stored in their own separate variables.
Using these variables, the mean is subtracted from the element-wise data and then divided by the standard deviation to calculate the normalized data, this is then repeated for all the data given

-CODE
![carbon](https://github.com/user-attachments/assets/c22d0f75-f51f-4daf-b064-a6c4bc8d4b0e)

-OUTPUT
![carbon (1)](https://github.com/user-attachments/assets/8bc83976-437e-4452-8412-b792ab8bb855)

