# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to create a model tha could predict the creditworthiness of loan borrowers. This was predicted based on the loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks and total debt. The dataset contained 75,036 borrowers with healthy loans and 2,500 borrowers with high risk of defaulting. In summary, the process consisted on: separating the data into labels ( y = loan status) and features (rest of the data), spliting the data into training and testing datasets, fiting a logistic regression model by using the training data, making predictions using the testing data, evalutaing the model by calculating the accuracy, generating a confusion matrix and analysing the classification report. Then, I did the same thing again with resampled training data and compared both models.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1 (Logistic Regression with original data):
  * Accuracy: 99%. This was a really high accuracy percentage.
  * Precision: 100% for 0 (healthy loan) and 85% for 1 (high-risk loan). The model was better at calculating healthy loans than high-risk loans. 
  * Recall: The model was able to catch 99% of healthy loans and 91% of high-risk loans.



* Machine Learning Model 2 (Logistic Regression with resampled data):
  * Accuracy: 99%. This was a really high accuracy percentage.
  * Precision: 100% for 0 (healthy loan) and 84% for 1 (high-risk loan). The model was better at calculating healthy loans than high-risk loans.
  * Recall: The model was able to catch 99% of healthy loans and 99% of high-risk loans.

## Summary

The model that seems to be better suited for this case is model two, with higher recall for high-risk loans, which aligns with the goal of identifying loans with a high risk of defaulting. The model that suits best does depend on the problem we are trying to solve and what is most important to us. Model one has higher precision for the high-risk class, but in this case, we want to focus on a higher recall since we want to make sure the model can identify high-risk loans better. The 84% precision for high-risk loan on model two might be concerning, and knowing more context about the business and the specific impact of the different types of predictions would be needed to decide if the model is recommended to use or not.
