# Non-Linear Regression Models

This repository contains a Machine Learning project focused on **non-linear regression modeling** using the `college.csv` and `regression.csv` datasets. The project demonstrates the use of Generalized Additive Models (GAMs) and Poisson GAMs to capture non-linear and interaction effects in data.

## Datasets

* **`college.csv`** – Contains information about colleges, including tuition, graduation rate, expenditures, alumni percentages, and other institutional features.
* **`regression.csv`** – Contains data used to model the response variable `richness` with temporal (`Year`) and spatial (`Longitude` and `Latitude`) predictors.

## Project Structure

1. **GAM on College Dataset**

   * Fitted a Generalized Additive Model (GAM) with `Out-of-State Tuition` as the response and a subset of predictors (`Private`, `Room.Board`, `PhD`, `perc.alumni`, `Expend`, `Grad.rate`).
   * Plotted the fitted smooth functions for each predictor.
   * Identified which predictors exhibited non-linear relationships with tuition.

2. **Poisson GAM on Regression Dataset**

   * Fitted a Poisson GAM (`M1`) modeling `E(richness) = exp(f(year)) * exp(g(Longitude, Latitude))`.
   * Plotted the model and summarized the results to assess effects of temporal and spatial variables.
   * Fitted an enhanced Poisson GAM (`M2`) including interaction terms between `Year`, `Longitude`, and `Latitude`.
   * Compared `M1` and `M2` using metrics such as (R^2), AIC, and test error to select the better-fitting model.

3. **Analysis and Visualization**

   * Visualized smooth functions of predictors for GAMs to detect non-linear trends.
   * Assessed temporal and spatial patterns in the response variable.
   * Evaluated model fit and compared competing models using statistical and predictive criteria.

## Tools & Libraries

* Python: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `pyGAM`
* Techniques: Generalized Additive Models (GAM), Poisson GAM, interaction effects, non-linear regression, model comparison

## Key Learnings

* Capturing non-linear relationships using GAMs to better model complex predictors.
* Assessing temporal and spatial effects on a response variable.
* Using interaction terms in Poisson GAMs to model combined effects of multiple predictors.
* Evaluating and comparing models using statistical metrics and predictive performance.
