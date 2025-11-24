# Machine Learning Regression Analysis Project

This repository contains a Machine Learning project focused on **linear and multiple regression analysis** using the `Auto.csv` dataset. The project includes simulations, model fitting, visualization, and interpretation of results for both simple and multiple linear regression scenarios.

## Dataset

* **File:** `Auto.csv`
* **Description:** Automobile dataset containing variables such as `mpg`, `horsepower`, `cylinders`, `displacement`, `weight`, `acceleration`, `year`, `origin`, and `name`.
* **Usage:** Used for regression modeling, correlation analysis, diagnostic plots, and exploration of interaction and polynomial effects.

## Project Structure

1. **Simple Linear Regression**

   * Fitted a simple linear regression model with `mpg` as the response and `horsepower` as the predictor.
   * Evaluated the relationship between predictor and response, including coefficient interpretation and statistical significance.
   * Predicted `horsepower` for given `mpg` values using numerical methods (`fsolve` from `scipy`).
   * Visualized results with scatterplots and regression lines using `seaborn.lmplot()`.
   * Diagnostic plots were created with `statsmodels.plot_fit()` to identify model issues or outliers.

2. **Multiple Linear Regression**

   * Performed regression with `mpg` as the response and all other variables (except `name`) as predictors.
   * Explored variable associations via pairplots and correlation heatmaps.
   * Evaluated significant predictors and fitted models with interaction effects.
   * Tested alternative variable transformations (log, square root, squared) and compared results.
   * Diagnostic plots were used to detect high-leverage points and unusual residual patterns.

3. **Simulated Data Analysis**

   * Generated synthetic datasets with controlled noise using normal distributions.
   * Created response variables using predefined linear relationships.
   * Fitted simple, polynomial, and multiple regression models.
   * Assessed the impact of noise variation on coefficient estimates and confidence intervals.
   * Demonstrated the equivalence of (R^2) and squared correlation for simple linear regression.

4. **Specific Analyses**

   * Explored regression with multiple predictors individually and jointly to understand coefficient interpretation.
   * Assessed the effect of outliers and high-leverage points on model stability.
   * Compared estimated coefficients to true values in simulated data for model validation.

## Visualizations

* Scatterplots showing relationships between predictors and response.
* Regression lines overlaid on scatterplots.
* Pairplots and heatmaps for multivariate exploration.
* Diagnostic plots to evaluate residuals, leverage, and model fit.

## Tools & Libraries

* Python: `pandas`, `numpy`, `scipy`, `seaborn`, `matplotlib`, `statsmodels`
* Techniques: Simple linear regression, multiple linear regression, polynomial regression, interaction terms, model diagnostics, transformations, numerical root finding

## Key Learnings

* Understanding the relationship between predictors and response variables.
* Assessing statistical significance of regression coefficients.
* Evaluating model fit and diagnosing potential issues (outliers, leverage points).
* Observing the effect of noise and transformations on regression models.
* Linking theoretical concepts (e.g., (R^2)) to empirical results using simulated data.
