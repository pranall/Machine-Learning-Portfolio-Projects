# Resampling Methods

This repository contains a Machine Learning project focused on **resampling methods** and regression modeling using the `data.csv` dataset. The project demonstrates the application of bootstrap, cross-validation, and regularized regression techniques to estimate model parameters and evaluate predictive performance.

## Dataset

* **File:** `data.csv`
* **Description:** Dataset containing information about colleges, including variables such as number of applications, acceptance rates, and other institutional characteristics.
* **Usage:** Used for resampling-based parameter estimation and regression modeling to predict the number of applications received.

## Project Structure

1. **Bootstrap Analysis**

   * Performed bootstrap sampling (`n = 1000`) to estimate the **median** and **95% confidence intervals** for the slope and intercept of the regression between `x` and `y_measured`.
   * Compared the parameter estimates obtained when using `y` instead of `y_measured`.

2. **Polynomial Regression and Resampling**

   * Improved the structure, clarity, and reproducibility of polynomial regression code.
   * Examined multiple replicates to ensure robust results.
   * Generated two plots to summarize model selection:

     1. Mean Squared Error (MSE) versus polynomial order.
     2. Scatterplot of `x` versus `y` with the best-fitting polynomial regression line overlaid.

3. **Predictive Modeling on College Dataset**

   * Fitted a **least squares linear regression** model on the training set to predict the number of applications received, and reported the test error.
   * Fitted a **ridge regression** model using cross-validation to select the optimal (\lambda) and reported the test error.
   * Fitted a **lasso regression** model using cross-validation to select the optimal (\lambda), reported the test error, and recorded the number of non-zero coefficients.

## Visualizations

* Mean Squared Error versus polynomial order to identify optimal model complexity.
* Scatterplots showing observed versus predicted relationships.
* Fitted regression lines illustrating model predictions.

## Tools & Libraries

* Python: `pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`, `statsmodels`, `sklearn`
* Techniques: Bootstrap sampling, cross-validation, polynomial regression, ridge regression, lasso regression

## Key Learnings

* Understanding the impact of resampling on parameter estimation and confidence intervals.
* Selecting polynomial model complexity based on resampling metrics (MSE).
* Evaluating predictive performance of different regression methods on training and test data.
* Observing the effect of regularization on coefficient estimates and model sparsity.
