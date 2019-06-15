# Implementing-Linear-Regression-1
Implementation of Linear Regression on USA Housing Dataset .
## What is Regression ?
Regression is basically a statistical approach of finding a relationship between the variables. Linear regression is one type of regression we use in Machine Learning.
## Basics of Linear Regression
* y = ax+b <br>
       y = Target<br>
       x = Feature<br>
       a,b = Parameter of the model
* How do we choose a and b ?
* Define an error function for any given line, choose the line that minimize the error function. Such an error function is also called     loss or cost function.

## What is our goal ??

Our goal is to minimize the vertical distance between all the data points and our line.
So, in determining the best line we are trying to minimize the distance between all the points and their distance to our line(Red Line).
There are lots of different ways to minimize this ,Sum of Squared Errors, Sum of absolute errors, etc., but all these methods have general goal of minimizing the distance.
For Example, one of the popular methods is the Least Square Methods.
## Least Squares Method :

Here, we have blue data points along X and Y axis. Now, we want to fit a linear regression line. How we decide which line is the best fitting line ?<br>
We will use the least squares method, which is fitted by Minimizing the sum of squares of the residuals(Red Line).
The residuals for an observation is the difference between the observation(the y-value) and the fitted line.
## Regression Evaluation Metrics
Here are three common evaluation metrics for regression problems:<br>
<b>Mean Absolute Error (MAE)</b> is the mean of the absolute value of the errors:<br>

<b>Mean Squared Error (MSE)</b> is the mean of the squared errors:<br>

<b>Root Mean Squared Error (RMSE)</b> is the square root of the mean of the squared errors:<br>

Comparing these metrics:
* <b>MAE</b> is the easiest to understand, because it's the average error.
* <b>MSE</b> is more popular than MAE, because MSE "punishes" larger errors, which tends to be useful in the real world.
* <b>RMSE</b> is even more popular than MSE, because RMSE is interpretable in the "y" units.<br>
All of these are loss functions, because we want to minimize them.
## Linear Regression in higher dimensions 
* y = a1 x1 + a2 x2 + b
* To fit a linear regression model here :<br>
      Need to specify 3 variables(a1,a2,b)
* In higher dimensions<br>
      y = a1 x1 +a2 x2 + --— +an xn+b <br>
      We must specify coefficients for each feature and the variable b.
* Sklearn api works exactly the same way <br>
      Pass two arrays : Feature and the target
