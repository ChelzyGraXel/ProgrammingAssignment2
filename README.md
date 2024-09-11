# Programming Assignment 2

## Normalization Problem
#### Step 1: Importing the NumPy Library
Firstly, I have imported numpy as np in order to gain access to the NumPy library. 

#### Step 2: Generating the 5 by 5 Array
In the given problem, it was asked to create a 5 by 5 array and store it to variable "X". At first, when I try to use the syntax "np.random.random((m,n,p)", it generates an array with float values with more than six decimal places. It would be difficult for me to check the accuracy of the calculations, that's why I considered using a function that would only generate integers with no decimals. The "np.random.randint(low,high, size)" syntax had provided me random values that are all positive integers and are only limited to being 1 to 100.

#### Step 3: Solving for the Mean and Standard Deviation
In order to compute for the normalized values, the formula is (X - mean) divided by the standard deviation. To calculate for the mean, I have utilized the syntax "X.mean()" and stored the result to "mean". Likewise with the computation for the standard deviation, syntax "X.std()" was used, then the result is stored to "stddev". 

#### Step 4: Calculating the Normalized Values
For the next step, I did not directly input the derived mean and standard deviation to solve for the normalized value. Instead, I created variable "n" that contains the value of the numerator of the formula which can be calculated by subtracting the mean from the X. After that, I divided the "n" by the "stddev" and its quotient is now the normalized values of ndArray X. The result is stored to X_normalized.

#### Step 5: Save the ndArray as X_normalized.npy
Last but not least, to save the ndArray to X_normalized.np, the "np.save('X_normalized.npy', X_normalized)". In order to print the results, the syntax "np.load('X_normalized.npy') was used.

## Divisible By 3 Problem
#### Step 1: Importing the NumPy Library
Firstly, I have imported numpy as np in order to gain access to the NumPy library.

#### Step 2: Generate the First 100 Positive Integers
The variable namely "num" contains all the positive integers from 1 to 100 and are all arranged in ascending order.

#### Step 3: Calculate for the Squares of each Integer
The variable namely "squaredNum" calculates for the squares of each integer in the array. The utilization of two asterisks indicates a exponential function. The "num**2" is num raised to the power of 2.

#### Step 4: Storing the Calculated Squares
The task was to store the computed values of squared integers into a 10 by 10 array. In order to do that, the syntax used was ".reshape((rows,columns))" and there are 10 rows and 10 columns.

#### Step 5: Check for Values Divisible by 3
Using a modulo %, it will solve for the remainder of each squared integer when divided by 3. If the remainder will be equal to zero, it will store the squared integer value to a variable named "multiplesOf3". In order to check all the values in the array A, another variable is named div_by_3 and it stores all the values of multipleof3 to a new array.

#### Step 6: Save the ndArray as div_by_3.npy
Last but not least, to save the ndArray to div_by_3.npy, the "np.save('div_by_3.npy', div_by_3)". In order to print the results, the syntax "np.load('div_by_3.npy') was used.

