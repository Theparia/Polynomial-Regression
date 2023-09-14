# Polynomial-Regression

This project implements Polynomial Regression with regularization, a machine learning technique used for modeling complex relationships between input features and output targets. 


## Introduction
Polynomial Regression is a regression technique that fits a polynomial equation to the data instead of a linear equation. It is particularly useful when the relationship between the input features and the output target is nonlinear. This implementation also includes regularization, which helps prevent overfitting and enhances the model's generalization.

## Features
- **Polynomial Transformation**: The `transform` method allows for the transformation of input features into polynomial features up to a specified degree. This enables capturing complex relationships in the data.
  
  - Input Features: $X = [x_1, x_2]$

  - Transformed Features: $f(X) = [x_1, x_2, x_1^2, x_1x_2, x_2^2, x_1^3, x_1^2x_2, x_1x_2^2, \ldots]$




- **Sigmoid Function**: The `sigmoid` method implements the sigmoid activation function, commonly used in logistic regression to model binary outcomes.
- **Hypothesis Function**: The `h_theta` method calculates the hypothesis function, which predicts output values based on input features and model parameters.
- **Feature Scaling**: The `scale_features` method standardizes input features by calculating their mean and standard deviation, ensuring consistent scales for polynomial features.
- **Batch Gradient Descent**: The `batch_gradient_descent` method optimizes the model parameters using batch gradient descent. It includes regularization to prevent overfitting and promote smoother polynomial fits.
- **Model Training**: The `fit` method trains the Polynomial Regression model on input data, transforming features, scaling them, and optimizing model parameters.
- **Prediction**: The `predict` method makes predictions on new data using the trained model, returning binary outcomes based on a specified threshold (0.5 by default).
