# Programming Assignment 2

## Normalization Problem
### Step 1: Importing the NumPy Library
Firstly, I have imported numpy as np in order to gain access to the NumPy library. 

### Step 2: Generating the 5 by 5 Array
In the given problem, it was asked to create a 5 by 5 array and store it to variable "X". At first, when I try to use the syntax (np.random.random((m,n,p)), it generates an array with float values with more than six decimal places. It would be difficult for me to check the accuracy of the calculations, that's why I considered using a function that would only generate integers with no decimals. The (np.random.randint(low,high, size) syntax had provided me random values that are all positive integers and are only limited to being 1 to 100.

### Step 3: Solving for the Mean and Standard Deviation
In order to compute for the normalized values, the formula is (X - mean) divided by the standard deviation. To calculate for the mean, I have utilized the syntax (np.mean(X)) and stored the result to "mean". Likewise with the computation for the standard deviation, syntax (np.std(x)) was used, then the result is stored to "stddev". 

### Step 4: Calculating the Normalized Values
For the next step, I did not directly input the derived mean and standard deviation to solve for the normalized value. Instead, I created variable "n" that contains the value of the numerator of the formula which can be calculated by subtracting the mean from the X. After that, I divided the "n" by the "stddev" and its quotient is now the normalized values of ndArray X.
