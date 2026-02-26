📉 Gradient Descent from Scratch & Comparison with Scikit-Learn

📌 Project Overview

This repository demonstrates the implementation of Gradient Descent for Linear Regression in two different ways:

📘 Manual Gradient Descent (Intercept update step-by-step visualization)

🛠 Custom Gradient Descent Class (Updating both slope and intercept)

📊 Comparison with Scikit-learn’s LinearRegression

The goal of this project is to deeply understand how Gradient Descent optimizes parameters (m and b) and how it compares to the closed-form solution used in OLS.

🧠 Concepts Covered

What is Gradient Descent?

Cost Function (Mean Squared Error)

Partial Derivatives

Updating parameters iteratively

Learning Rate

Epochs

Convergence behavior

Comparison with Ordinary Least Squares (OLS)

📁 Notebooks Included:

1️⃣ Notebook 1 – Step-by-Step Gradient Descent (Intercept Update)

Dataset generated using make_regression

Manual update of intercept (b) while keeping slope (m) fixed

Visualization of regression line after each iteration

Comparison with Scikit-learn OLS line

What This Notebook Shows:

How b changes after each gradient step

How regression line moves toward optimal solution

Visual understanding of convergence

2️⃣ Notebook 2 – Full Gradient Descent Implementation

Larger synthetic dataset

Train/Test split

Cross-validation using cross_val_score

Custom GDRegressor class created from scratch

Simultaneous update of:

Slope (m)

Intercept (b)

⚙️ Technologies Used:

Python

NumPy

Pandas

Matplotlib

Scikit-learn

📊 Model Comparison:

🔴 Scikit-Learn Linear Regression

Uses closed-form Ordinary Least Squares solution.

Example Output:

m = 28.12
b = -2.27
R² ≈ 0.63

🔵 Custom Gradient Descent

Initial values:

m = 100
b = -120

After 50 epochs:

m ≈ 28.15
b ≈ -2.30

R² Score:

0.634

✅ Very close to Scikit-learn result.

📈 Results

Gradient Descent successfully converged to near-optimal parameters.

Custom implementation achieved nearly the same R² score as Scikit-learn.

Demonstrated importance of:

Learning rate

Proper initialization

Number of epochs

