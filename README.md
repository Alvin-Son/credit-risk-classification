# Module 12 Report

## Overview of the Analysis

* **Purpose of the Analysis**: The purpose of the analysis was to evaluate the performance of various machine learning models in predicting the risk level of loans, specifically identifying whether a loan is healthy (0) or high-risk (1).
* **Financial Information**: The data included financial information related to loans, with the goal of predicting the risk associated with each loan.
* **Variables**: The primary variable to predict was the loan risk classification (`0` for healthy loans and `1` for high-risk loans). Basic information such as `value_counts` showed the distribution of these classes.
* **Stages of Machine Learning Process**:
  * Data Preprocessing: Cleaning and preparing the data for modeling.
  * Model Training: Using algorithms such as `LogisticRegression` to train models on the dataset.
  * Model Evaluation: Assessing the models' performance using metrics like accuracy, precision, recall, and f1-score.
* **Methods Used**: The analysis involved the use of `LogisticRegression` among other potential algorithms to predict loan risk.

## Results

* **Machine Learning Model 1: Logistic Regression**:
  * **Accuracy**: 0.99
  * **Healthy Loan (Label 0)**:
    * Precision: 1.00
    * Recall: 0.99
    * F1-Score: 1.00
  * **High-Risk Loan (Label 1)**:
    * Precision: 0.84
    * Recall: 0.94
    * F1-Score: 0.89
  * **Macro Average**:
    * Precision: 0.92
    * Recall: 0.97
    * F1-Score: 0.94
  * **Weighted Average**:
    * Precision: 0.99
    * Recall: 0.99
    * F1-Score: 0.99

## Summary

* **Best Performing Model**: The logistic regression model performed best, with an overall accuracy of 99%. This is evident from the high precision and recall scores, especially for healthy loans.
* **Performance Dependence**: Performance depends on the problem's priorities. If predicting high-risk loans (`1`s) is more critical, the slightly lower precision of 0.84 should be considered. However, the high recall of 0.94 indicates that most high-risk loans are correctly identified.
* **Recommendation**: Given its high overall accuracy and balanced performance metrics, the logistic regression model is recommended. It is particularly strong in predicting healthy loans while still performing well in identifying high-risk loans.
