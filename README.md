# Linear Regression (Gradient Descent)

## Overview

This project implements **Linear Regression from scratch using Gradient
Descent** to predict a target value from a single feature. The goal is
to understand how linear regression works without using machine learning
libraries.

## Dataset

The dataset contains two columns:

-   **features** → input variable x
-   **labels** → target variable y

Example:

  features   labels
  ---------- --------
  0.58       4.09
  0.00       0.19
  -0.47      -3.95

## Model

The model learns a linear relationship between the feature and the
label:

y_hat = w\*x + b

To simplify calculations, the bias is added as a column of ones in the
feature matrix:

X = \[1, x\]

So the prediction becomes:

y_hat = Xw

## Cost Function

The model is trained by minimizing the Mean Squared Error:

J(w) = (1/(2m)) \* sum((y_hat - y)\^2)

where m is the number of training samples.

## Training (Gradient Descent)

Weights are updated using gradient descent:

w = w - alpha \* gradient

where:

-   alpha → learning rate
-   gradient → derivative of the cost function

Hyperparameters used:

alpha = 1.99 iterations = 10000

## Implementation Steps

1.  Load the dataset
2.  Convert values to numeric format
3.  Normalize the feature values
4.  Add a bias column to the feature matrix
5.  Initialize weights to zero
6.  Train the model using gradient descent
7.  Track cost and weights during training

## Output

The program prints:

-   initial cost
-   final cost after training
-   final learned weights

## Tools Used

-   Python
-   NumPy
-   Pandas
-   Matplotlib
