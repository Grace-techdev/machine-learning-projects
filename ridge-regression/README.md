# Ridge Regression: Closed-form vs SGD (Python)

This project explores **Ridge Regression** using two optimisation approaches:
a **closed-form solution** and **Stochastic Gradient Descent (SGD)**.

The focus is on how model behaviour changes with:
- polynomial model complexity  
- regularisation strength (L2 penalty)  
- optimisation strategy  
- dataset size and feature dimensionality  

Synthetic datasets with known ground-truth functions are used to enable controlled analysis of bias–variance trade-offs and scalability.

## What This Project Covers

- Synthetic polynomial data generation with Gaussian noise  
- Closed-form Ridge Regression implemented from scratch  
- Ridge Regression using `SGDRegressor`  
- Comparison of prediction accuracy, learned weights, and stability  
- Analysis of regularisation effects and model complexity  
- Empirical evaluation of training and prediction time  

## Key Observations

- When model complexity matches the true data-generating process, both methods perform similarly.  
- Strong regularisation can lead to underfitting even with correct model complexity.  
- The closed-form solution is stable for moderate feature dimensions.  
- SGD scales better to large datasets but is more sensitive to hyperparameters.  
- For very high polynomial degrees, regularisation alone is insufficient.

## How to Run

```bash
pip install -r requirements.txt
```

This project was originally developed for
University of Western Australia – CITS5508 Machine Learning (Assignment 1).