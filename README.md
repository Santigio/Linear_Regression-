# Linear Regression

# This project is designed to explain how the concept of Statistics can be applied in machine learning to make inferences or predictions. In the end, I aim at providing you with a clear and straightforward understanding of how one can use the concept of statistics and linear regression to make prediction. You can use this example to make predictions using linear regression. 

# Problem definition
To start with, Brewery Rwanda, a business that makes and sells beer, wants an ideal model that separates beer from wine. So as data engineer, you have been asked to design a machine learning model that answers the question of whether a drink is a beer or wine. 

In this project, our goal is to create a model that answers whether the drink is wine or beer.
In designing a machine learning model, statistics is an important prerequisite to consider, and it’s so much important to not only visualize data, but also to perform data analysis. 

Statistics as a subfield of mathematics focuses on the collection of methods for working with data and using data to answer questions.


# Regression 
Regression for machine learning (Mathematical Aspect)

To start with, let's talk a little bit about regression in general, but let's start off with Supervised learning since it’s the core of regression and machine learning in general.

Supervised Learning looks at a collected dataset containing numeric value (height, weight), label(yes/no), or classification and makes predictions of data that we don’t know. It requires the need of a coder or engineer to oversee the algorithm. For instance, dogs do certain activities based on past supervised learning.

# Types of supervised learning
  Linear regression for regression problems
 Support vector machine learning for classification problems
 

    Regression: Relationship between two or more variables, where the change in one variable is associated with the change in another. It deals with data that are numerical (or continuous) e.g., salary based on work experience, weight based on height etc. types of regression are linear, logistic, lasso regression, stepwise, ridge, polynomial elastic Net regression.
How much salary raise will I get? 

·   Classification: deals with data that are categorical or discrete. I.e with two or more values. Eg yes/no, true/false, spam/not spam email
For instance will I get a salary raise or not? 
 Some Algorithms used in supervised learning
      	
Nearest Neighbor
Support Vector Machines
Decision Trees
Boosted Trees
Random Forest
Neural Networks
Linear Regression
Logistic regression 

Real life use of supervised learning- risk assessment, image classification, fraud detection, speech recognition, 


# And now let’s take a look at Linear regression since it’s our focus .
Linear regression is one of the most well known and well understood algorithms in statistics and machine learning. It makes expectations for continuous/real or numeric factors such as deals, compensation, age, item cost, etc. Linear regression tends to establish a relationship between them by formulating an equation that describes the outcome (y) as a linear combination of the input variables. It is also known as multiple regression, multivariate regression, and ordinarily least squares. The linear regression model provides a sloped straight line representing the relationship between the variables. Consider the below image:
(Linear Regression in Machine learning - Javatpoint, 2020)
 
 
# Types of linear regression
Simple linear regression is a regression model that estimates the relationship between one independent variable and one dependent variable using a straight line. Both variables should be quantitative. 



Multiple linear regression attempts to model the relationship between two or more explanatory variables and a response variable by fitting a linear equation to observed data. Every value of the independent variable x is associated with a value of the dependent variable y. 


Cost function
The cost function helps us to find the best possible values for a 0 and a 1 that would provide the best line for the data points. Since we want the best values for a 0 and a 1, we convert this search problem into a minimization problem where we want to minimize the error between the predicted value and the actual value.



To minimize, we choose the above function. The difference between the predicted values and the ground truth is a measure of the error difference. We calculate the error difference and sum over all data points and divide that value by the total number of data points. This results in an average squared error over all data points.


Gradient Descent

The next big term needed to understand linear regression is gradient descent. Gradient Descent is a tool for modifying a 0 and a 1 to reduce the cost function (MSE). The idea is that we start with certain values for a 0 and a 1, and then adjust these values iteratively to minimize costs. Gradient descent allows one to change the values.




 # Technology ( Linear Regression)

To start off,  I collected sample data to train our model as shown below. I take record of rainfall in two years and the umbrellas sold in those years. The idea is to check for a relationship between our independent variables(rainfall) which is one factor that can affect sales,  and our dependent variable(umbrella sold) in a list of months. 
 



Interpret regression analysis output.

R Square
In the data, R2 is 0.15, which is fairly poor. It means that 15% of our values fit the regression analysis model. In other words, 15% of the dependent variables (y-values) are explained by the independent variables (x-values). Generally, our model doesn't fit well.

Multiple R
The data has a strong negative relationship. Since it draws closer to -1. The model explains 39% of the variance in the dependent variable.



Another aspect to also consider is analysis of variance(ANOVA). Which basically splits the sum of squares into individual components that gives information about the levels of variability within our regression model. 

Whereas, 
Df is the number of the degrees of freedom associated with the sources of variance. 
SS is the sum of squares. The smaller the Residual SS compared with the total SS, the better the model fits the data. 
MS is the mean square.
F is the statistic, or F-test for null hypothesis. Which is used to test the overall significance of the model. 
Significance F is the p value of F. 

And we can tell that our model is reliable since the Significance F is not above 0.05(5%). In other words, we chose the right independent variable. 



# To get our linear regression formulae, we need to know the rainfall coefficient and intercept. 

Given that the formulae of a line is; 

Y = bx + a

Y = Rainfall Coefficient * x + Intercept

# From our output, our formulae is now 

Y = 0.415*x-9.57 rounded to three decimal places. For instance, with the average rainfall equal to 116 mm, the umbrella sales would be 39.148.

 0.42*116-9.57= 39.148


# To compare our estimated vs our actual number of sold umbrellas. 

Estimated: 39.15
Actual: 34

 The reason why we have these differences is because independent variables are never perfect predictors of dependent variables. 



# Conclusion

In conclusion, linear regression as one of the most commonly used predictive modelling techniques, I have been able to perform analyzes and identify the relationship between two variables; rainfall, and umbrella solds in specific months in Rwanda. Normally you need large dataset to get an accurate result.



