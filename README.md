Linear regression is a type of supervised learning algorithm, commonly used for predictive analysis. As the name suggests, linear regression performs regression tasks. Now, what is regression? Well, regression is nothing but a technique that displays the relationship between two variables.
We refer to dependent variables as responses and independent variables as features.
In order to provide a basic understanding of linear regression, we start with the most basic version, i.e., simple linear regression.

Simple Linear Regression:-

Simple linear regression is an approach for predicting a response using a single feature.
It is assumed that the two variables are linearly related. Hence, we try to find a linear function that predicts the response value (y) as accurately as possible as a function of the feature or independent variable (x).
The line of best fit is nothing but the line that best expresses the relationship between the data points. Let us see how to find the best-fit line in linear regression.

What Is Linear Regression?
linear regression is a predictive modeling technique. It is used whenever there is a linear relation between the dependent and the independent variables.

Y = b0 + b1* x
It is used in estimating exactly how much of y will change when x changes a certain amount.

Linear Regression
As we see in the picture, a flower’s sepal length is mapped onto the x-axis and the petal length is mapped on the y-axis. Let us try and understand how the petal length changes with respect to the sepal length with the help of linear regression. Let us have a better understanding of linear regression with another example given below.

Example:
Say, there is a telecom network called Neo. Its delivery manager wants to find out if there’s a relationship between the monthly charges of a customer and the tenure of the customer. So, he collects all customer data and implements linear regression by taking monthly charges as the dependent variable and tenure as the independent variable. After implementing the algorithm, what he understands is that there is a relationship between the monthly charges and the tenure of a customer. As the tenure of the customer increases, the monthly charges also increase. Now, the best-fit line helps the delivery manager find out more interesting insights from the data. With this, he can predict the values of y for every new value of x.

Example of Linear Regression
Let us say, the tenure of a customer is 45 months, and with the help of the best fit line, the delivery manager can predict that the customer’s monthly charges would be somewhere around $64.

Example of Linear Regression
Similarly, if the tenure of a customer is 69 months, then with the help of the best fit line the delivery manager can predict that the customer’s monthly charges would be somewhere around $110.

Example of Linear Regression
This is how linear regression works. Now, the question is how to find the best fit line?

Interested to learn Data Science? Check out this Data Science course in Chennai to get clear understanding.

Linear Regression Line of Best Fit
The line of best fit is nothing but the line that best expresses the relationship between the data points. Let us see how to find the best fit line in linear regression.

This is where the residual concept comes into the picture which is shown in the image below:

Linear Regression Line of Best Fit
Red lines in the above image denote residual values, which are the differences between the actual values and the predicted values. How does residual help in finding the best fit line?

To find out the best fit line, we have something called residual sum of squares (RSS). In RSS, we take the square of residuals and sum them up.

RSS
The line with the lowest value of RSS is the best fit line.


Now, let us see how the coefficient of x influences the relationship between the independent and the dependent variables.

Regression Coefficient
In simple linear regression, if the coefficient of x is positive, then we can conclude that the relationship between the independent and the dependent variables is positive.

Regression Coefficient Positive Relation
Here, if the value of x increases, the value of y also increases.

Now, if the coefficient of x is negative, then we can say that the relationship between the independent and the dependent variables is negative.

Regression Coefficient Negative Relation
Here, if the value of x increases, the value of y decreases.

Now, let us see how we can apply these concepts to build linear regression models. In the below given Python Linear Regression Examples, we will be building two machine learning models for simple and multiple linear regression. Let’s begin.


Hands-on: Linear Regression Using Python Scikit learn Hands-on-: USA Housing Prices Dataset

Environment: Python 3 and Jupyter Notebook
Library: Pandas
Module: Scikit-learn
