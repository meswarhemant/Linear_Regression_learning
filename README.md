# Linear Regression

## What is Linear Regression?
Linear Regression is a supervised machine learning algorithm used for predicting a continuous output (dependent variable) based on one or more input features (independent variables). It assumes a linear relationship between the input features and the output.

The model tries to fit a straight line (or hyperplane in multiple dimensions) to the data that best explains the relationship between inputs and the output.

Mathematical Representation
The linear regression equation looks like this:

𝑦=𝛽0+𝛽1𝑥1+𝛽2𝑥2+⋯+𝛽𝑛𝑥𝑛+𝜖y

Where:

𝑦 is the predicted value,

𝛽0 is the intercept (the value of 𝑦 when all inputs are zero),

𝛽1,𝛽2,...,𝛽𝑛 are the coefficients (weights) assigned to each feature,

𝑥1,𝑥2,...,𝑥𝑛 are the feature values,

𝜖 is the error term capturing noise or variation in the data.

The algorithm learns the coefficients by minimizing the error between the predicted and actual values using the Least Squares method.

## How Linear Regression Works
You start with input data containing features and a continuous target variable.

The algorithm estimates the best-fitting line that minimizes the difference between actual and predicted values.

Once trained, you can predict the target for new data by plugging in feature values into the equation.

Example 1: Simple Linear Regression
Imagine you want to predict a student's exam score based on the number of hours they studied. If the model learns that the relationship is:

Score=45+6×(Hours Studied)

This means every additional hour studied increases the predicted exam score by 6 points. For example, a student who studied for 3 hours would have a predicted score of:

45+6×3=63

Example 2: Multiple Linear Regression
Suppose you want to predict the price of a house based on its size in square feet and the number of bedrooms. If the model learns:

Price=50000+100×(Size in sq ft)+20000×(Number of bedrooms)

Then, for a house with 2000 square feet and 4 bedrooms, the predicted price would be:

50000+100×2000+20000×4=330000

## Advantages
Simple to implement and understand.

Provides clear insight into how each feature affects the target.

Efficient for linearly related data.

Serves as a good baseline for regression problems.

## Limitations
Only captures linear relationships, which may be too simplistic for complex data.

Sensitive to outliers that can skew the model.

Assumes errors are normally distributed and have constant variance.

Can struggle with correlated features (multicollinearity).

