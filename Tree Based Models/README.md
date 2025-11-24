# Tree Based Models

This repository contains a Machine Learning project focused on **tree-based methods** using datasets from the ISLR repository. The project demonstrates the use of **random forests** and **boosting** to model complex relationships and evaluate predictive performance compared to simpler models.

## Dataset

* **Source:** ISLR datasets ([https://book.huihoo.com/introduction-to-statistical-learning/data.html](https://book.huihoo.com/introduction-to-statistical-learning/data.html))
* **Description:** Dataset(s) selected for regression or classification tasks, including features relevant to the target variable.
* **Usage:** Used for training tree-based models and comparing predictive accuracy against simpler methods such as linear or logistic regression.

## Project Structure

1. **Data Loading and Preprocessing**

   * Read the dataset using `pandas.read_csv()` and performed preprocessing, including handling missing values and ensuring data quality.

2. **Train-Test Split**

   * Split the dataset into training and test sets using a chosen proportion to evaluate model performance.

3. **Tree-Based Modeling**

   * Applied **Random Forests** on the training set and predicted outcomes on the test set.
   * Applied **Boosting** (e.g., gradient boosting) on the training set and predicted outcomes on the test set.
   * Compared predictive accuracy of tree-based methods to simpler linear or logistic regression models.
   * Determined which method achieved the best performance for the given task.

4. **Model Evaluation**

   * Evaluated models using metrics appropriate to the task (accuracy, test error, or other performance metrics).
   * Compared results of tree-based models with simpler regression methods.

## Tools & Libraries

* Python: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
* Techniques: Random Forest, Boosting, Train-Test Split, Model Evaluation, Preprocessing

## Key Learnings

* Understanding the advantages of tree-based models over simpler linear or logistic regression in capturing non-linear patterns and interactions.
* Comparing performance of Random Forest and Boosting for prediction tasks.
* Preprocessing and splitting data appropriately to ensure fair evaluation.
* Interpreting tree-based models and evaluating their predictive accuracy on unseen data.
