📉 Gradient Descent Visualization for Linear Regression

📌 Project Overview

This project demonstrates how Gradient Descent updates the intercept (b) in Simple Linear Regression.

The objective is to understand how the cost function derivative adjusts the regression line step-by-step until it approaches the Optimal Least Squares (OLS) solution.

Instead of directly using the final model, this project visually shows how the regression line moves during each iteration.

📁 Dataset

The dataset is generated using:

from sklearn.datasets import make_regression

Parameters used:

n_samples = 4

n_features = 1

noise = 80

random_state = 13

This creates a simple synthetic regression dataset with noise.

🧠 Algorithm Concept
🔹 Model Equation

y = mx + b

Where:

m = slope

b = intercept

🔹 Gradient Descent Update Rule

To update intercept (b), we compute the derivative of the cost function:

∂J/∂b = -2 Σ (y - mx - b)

Update rule:

b = b - α * ∂J/∂b

Where:

α = learning rate

∂J/∂b = gradient

b = updated intercept

⚙️ Implementation Details

Slope (m) is initialized from OLS result (~78.35)

Intercept (b) starts from 0

Learning rate (lr) = 0.1

Multiple iterations are performed

Regression line is plotted after each update

The model gradually moves toward the optimal OLS solution.

📊 Visualization

The graph contains:

🔴 Red Line → OLS solution (from sklearn)

🔵 Blue Line → Initial line (b = 0)

🟢 Green/Black/Yellow Lines → Updated lines after each iteration

This clearly shows how Gradient Descent shifts the line upward until it matches OLS.

📈 Results

From sklearn OLS:

Slope (m):
78.3506

Intercept (b):
26.1596

After multiple Gradient Descent updates, the intercept converges close to:

b ≈ 26.11

This confirms that Gradient Descent successfully approaches the optimal solution.
