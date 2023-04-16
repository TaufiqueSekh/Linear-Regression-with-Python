# Linear regression
Linear regression is a type of supervised learning algorithm, commonly used for predictive analysis. As the name suggests, linear regression performs regression tasks. Now, what is regression? Well, regression is nothing but a technique that displays the relationship between two variables.
We refer to dependent variables as responses and independent variables as features.
In order to provide a basic understanding of linear regression, we start with the most basic version, i.e., simple linear regression.

## Important assumptions of Linear regression?

Linear Regression is a useful statistical method one can use to understand the relationship between two variables, x and y 
Before conduct linear regression one must first make sure that four assumptions are met:

1. Linear relationship: There exists a linear relationship between the independent variable, x, and the dependent variable, y.
2. Independence: The residuals are independent. In particular, there is no correlation between consecutive residuals in time series data.
3. Homoscedasticity: The residuals have constant variance at every level of x.
4. Normality: The residuals of the model are normally distributed.

If one or more of these assumptions are violated, then the results of linear regression may be unreliable or even misleading

## What is Heteroscedasticity / Non-Constant Variance?

Also known as non-constant variance
Heteroscedasticity refers to data for which the variance of the dependent variable is unequal across the range of independent variables. Heteroscedasticity is the opposite of homoscedasticity. The heteroscedasticity of data is important in the context of regression analysis. A regression model assumes a consistent variance, or homoscedasticity, across the data. 
Heteroscedasticity in the data results in regression providing accurate outputs on one end of the data range but highly inaccurate outputs on the other end of the data. An easy way to visualize these concepts is to create a scatter plot of the data. A heteroscedastic data set will exhibit a conical shape across the range of independent variables. The wider the cone, the more heteroscedastic the data is and the less friendly for regression analysis. It is important to understand that a regression analysis on the data set is still possible but the results will prove unreliable outside of a specific range.

## What are the implications?

When heteroscedasticity is detected in the residuals from a model, it suggests that the model is misspecified (i.e., in some sense wrong). Possible causes of heteroscedasticity include:
--Incorrectly assuming linear relationships in models
--Incorrect distributional assumptions (e.g., using linear regression when Poisson regression would be appropriate)
--Models that perform better for some subgroups than others (e.g., a model that performs well for women but poorly for men will exhibit heteroscedasticity)
--The existence of autocorrelation means that the standard computations of standard errors, and consequently p-values, are misleading.

## Fixes for heteroscedasticity:

--The best solution for heteroscedasticity is to modify the model so that the problem disappears. For example:
--Transform some of the numeric variables by taking their natural logarithms
--Transform numeric predictor variables
--Build separate models for different subgroups
--Use models that explicitly model the difference in the variance (as opposed to just modeling the mean, which is what most models do)

### Simple Linear Regression:-

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

## Linear Regression Line of Best Fit

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

## How does multicollinearity affect the linear regression?

Multicollinearity occurs when some of the independent variables are highly correlated (positively or negatively) with each other. This causes a problem, as it is against the basic assumption of linear regression. The presence of multicollinearity does not affect the predictive capability of the model. So, if you just want predictions, the presence of multicollinearity does not affect your output. However, if you want to draw some insights from the model and apply them in, let’s say, some business model, it may cause problems.
One of the major problems caused by multicollinearity is that it leads to incorrect interpretations and offers wrong insights. The coefficients of linear regression suggest the mean change in the target value if a feature is changed by one unit. So, if multicollinearity exists, this does not hold true, as changing one feature will lead to changes in the correlated variable and consequent changes in the target variable. This leads to wrong insights and can produce hazardous results for a business.
**A highly effective way of dealing with multicollinearity is the use of VIF (variance inflation factor). The higher the value of VIF for a feature, the more linearly correlated that feature is. Simply remove the feature with a very high VIF value and retrain the model on the remaining data set.


Now, let us see how we can apply these concepts to build linear regression models. In the below given Python Linear Regression Examples, we will be building two machine learning models for simple and multiple linear regression. Let’s begin.


Hands-on: Linear Regression Using Python Scikit learn Hands-on-: USA Housing Prices Dataset

Environment: Python 3 and Jupyter Notebook
Library: Pandas
Module: Scikit-learn
