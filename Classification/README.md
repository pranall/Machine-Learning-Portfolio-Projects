# Classification

This repository contains a Machine Learning project focused on **classification methods** using the `Weekly` and `Auto.csv` datasets. The project demonstrates the application of logistic regression, LDA, QDA, and other classification approaches to predict categorical outcomes based on predictor variables.

## Datasets

* **`Weekly`** – Dataset from the `ISLR2` package, similar to the `Smarket` dataset, containing weekly stock market returns and trading volume.
* **`Auto.csv`** – Automobile dataset containing features such as `mpg`, `horsepower`, `weight`, `acceleration`, and other vehicle characteristics, used to predict high versus low gas mileage.

## Project Structure

1. **Exploration of Weekly Dataset**

   * Produced numerical and graphical summaries, including correlation analysis, to identify patterns in the predictors.
   * Fitted a logistic regression model with `Direction` as the response and five `Lag` variables plus `Volume` as predictors.
   * Computed the confusion matrix and overall accuracy, analyzing types of classification errors.
   * Trained a logistic regression model on 1990–2008 data with `Lag2` as the only predictor, and evaluated on 2009–2010 held-out data.

2. **Gas Mileage Classification on Auto Dataset**

   * Created a binary variable `mpg01` indicating high or low gas mileage based on the median `mpg`.
   * Explored relationships between `mpg01` and other features using scatterplots and boxplots to identify useful predictors.
   * Applied **Linear Discriminant Analysis (LDA)** to predict `mpg01` and reported test error.
   * Applied **Quadratic Discriminant Analysis (QDA)** to predict `mpg01` and reported test error.
   * Applied **Logistic Regression** to predict `mpg01` and reported test error.

3. **Model Evaluation**

   * Compared classification methods based on predictive accuracy and test error.
   * Analyzed which predictors were most influential for correctly classifying outcomes.

## Visualizations

* Scatterplots and boxplots to explore feature relationships with categorical outcomes.
* Confusion matrices to evaluate classification performance.

## Tools & Libraries

* Python: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `sklearn`
* Techniques: Logistic regression, Linear Discriminant Analysis (LDA), Quadratic Discriminant Analysis (QDA), exploratory data analysis

## Key Learnings

* Understanding predictor-response relationships in classification contexts.
* Evaluating and interpreting model performance using confusion matrices and test error.
* Comparing the performance of multiple classification methods on the same dataset.
* Identifying the most informative features for predicting categorical outcomes.
