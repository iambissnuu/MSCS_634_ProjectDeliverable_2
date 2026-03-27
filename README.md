# Regression Modeling and Performance Evaluation

### MSCS 634 - Advanced Data Mining
### Name: Bishnu Sharma
### Deliverable 2

---

## Overview

This deliverable focuses on building and evaluating regression models to predict customer account balance using the Bank Marketing Dataset. The objective is to apply feature engineering techniques, develop multiple regression models, and compare their performance using appropriate evaluation metrics.

The analysis includes Linear Regression, Ridge Regression, and Lasso Regression models. Model performance is evaluated using R-squared (R²), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE). Cross-validation is also applied to assess the generalization ability of the models.

---

## Dataset Summary

* Dataset Name: Bank Marketing Dataset (UCI Machine Learning Repository)
* Number of Records: 45,000+
* Number of Features: 16+
* Target Variable: balance (customer account balance)

The dataset contains customer demographic information, financial attributes, and marketing campaign data, making it suitable for predictive modeling and regression analysis.

---

## Data Preprocessing and Feature Engineering

The following preprocessing and feature engineering steps were applied:

* Converted categorical variables into numerical format using one-hot encoding
* Scaled numerical features using StandardScaler to ensure consistent feature contribution
* Removed redundancy by dropping one category level to avoid multicollinearity

These steps improved model performance and ensured compatibility with regression algorithms.

---

## Regression Models Implemented

The following models were developed and evaluated:

* Linear Regression
  Serves as a baseline model for comparison

* Ridge Regression
  Applies L2 regularization to reduce overfitting and handle multicollinearity

* Lasso Regression
  Applies L1 regularization and performs feature selection

---

## Model Evaluation

Model performance was evaluated using:

* R-squared (R²): Measures how well the model explains variance in the target variable
* Mean Squared Error (MSE): Measures average squared prediction error
* Root Mean Squared Error (RMSE): Provides error magnitude in original units

Additionally, 5-fold cross-validation was used to assess model generalization and stability.

---

## Visualizations

The following visualizations were used to support model evaluation:

* Bar charts comparing R² and RMSE across models
* Residual plot to analyze prediction errors
* Feature importance plot based on Ridge regression coefficients

---

## Key Insights

* Ridge Regression achieved the best overall performance, with the highest R² and lowest RMSE, indicating improved predictive accuracy.

* The superior performance of Ridge Regression suggests the presence of multicollinearity among features, which was effectively handled through regularization.

* Lasso Regression simplified the model by reducing less important feature coefficients, highlighting key variables influencing customer balance.

* Cross-validation results confirmed that all models generalize well, with Ridge showing the most consistent performance across folds.

* Residual analysis indicated that prediction errors are reasonably distributed, suggesting minimal model bias, although some variability exists for higher balance values.

* Feature importance analysis revealed that only a subset of variables significantly influence the target variable, emphasizing the importance of feature selection.

---

## Challenges and Solutions

* High dimensionality after encoding
  Addressed by using regularization techniques such as Ridge and Lasso

* Multicollinearity among features
  Handled using Ridge Regression to stabilize model coefficients

* Model interpretability
  Improved through feature importance analysis and Lasso regression

---

## Repository Contents

The repository includes the following files:

* DataMining_Deliverable2.ipynb
  Contains the full implementation of regression models, feature engineering, evaluation, and visualizations

* README.md
  Provides an overview of the dataset, methodology, model evaluation, and key insights

* bank-full.csv
  Dataset used for analysis or a reference to its source

---

## Conclusion

This analysis demonstrates that Ridge Regression is the most effective model for predicting customer account balance in this dataset. Regularization techniques significantly improved model performance and stability.

While the models captured meaningful patterns, further improvements could be achieved through advanced feature engineering or non-linear modeling approaches.

---

## Future Improvements

* Explore polynomial or non-linear regression models
* Perform hyperparameter tuning for regularization strength
* Incorporate additional features or external data sources
* Evaluate alternative machine learning models

---
