Loan Default Prediction Project:
- This project aims to build a machine learning model for predicting whether a customer will default on a loan based on historical data.
- The project follows a structured approach, including data exploration, visualization, and the application of various machine learning models.
- The ultimate goal is to create a publishable and reproducible project that showcases the process of developing a predictive model for loan default prediction.


Project Organization - The project is organized into the following main steps:

Step 1) Data Understanding and Cleaning:
- Read and understand the dataset's contents and column descriptions.
- Perform summary statistics analysis for numerical and categorical columns.
- Check for missing values and duplicates.
- Impute missing data where necessary.

Step 2) Data Visualization:
- Visualize the distribution of numerical features using histograms, density plots, and boxplots.
- Explore correlations between numerical features using a pairplot and heatmap.
- Analyze categorical features using count plots with and without 'default' as the hue.

Syep 3) Machine Learning Models:
- Identify the target variable ('default') and predictor variables (numerical and categorical).
- Encode nominal columns using one-hot encoding and ordinal columns using ordered ranking.
- Apply standard scaling to numerical features using the Standard Scaler.
- Split the data into training and testing sets with stratification.
- Hyperparameter tune machine learning models using GridSearch and cross-validation.
- Fit all the models on the training set and evaluate performance on testing set.
- Compare models using AUC-PR and ROC curves along with AUC values from different values of thresholds.
- Finalize the model with the help of AUC-PR values and find a custom threshold to achieve optimal recall performance.


Repository Structure:

1) Dataset/: Contains the dataset files used in the project.
- credit.csv (Original dataset)
- Germanbankstep1output.csv (Cleaned dataset obtained after performing Step 1)

2.) ipynb files/: Contains Google Colab files. It contains all the three major steps as follows in one Google colab file.
- Step1) Well documented Python code to read, explore and clean data (automated processes and no hand edit on raw data).
- Step2) Well documented Python code to manipulate, wrangle and visualize data.
- Step3) Well documented Python code to run ML models and make publication-worthy figures or tables.

3.) Readme file/: Contains the project README file.
- README.txt: Detailed project overview and instructions.

Loan_Default_Prediction_Project/
│
├── CSV datafiles
│   ├── credit.csv (Original dataset)
│   ├── Germanbankstep1output.csv (Clean dataset after data cleaning in Step 1)
│
├── Google Colab Notebook
│   ├── Pranal'sMLFinalProject.ipynb (Contains all three steps:Python code to read, explore and clean data, manipulate,wrangle and visualize data and code to run ML models and make publication-worthy figures/tables.
│   
├── Images (Tables and graph plots)
│
└── README file (Project README file)

Necessary Python Libraries - The project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter
- xgboost


Conclusion:
- The project demonstrates a comprehensive approach to building and evaluating machine learning models for loan default prediction.
- Following the provided steps and exploring the notebooks, one can gain insights into the data, model performance, and strategies for improving recall in imbalanced classification scenarios.
