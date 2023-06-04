# Credit Risk Analysis Report

## Overview of the Analysis

The purpose of the analysis was to train a model to be able to identify healthy loans (0) and high-risk loan (1) requests. The financial information at hand contained data about:
* loan_size	
* interest_rate	
* borrower_income	
* debt_to_income	
* num_of_accounts	
* derogatory_marks	
* total_debt	

In the data set, for the objective value there were 75,036 values with (0) and 2500 with (1).

For the machine learning model the following stages were followed:
* Creation of the X and y (objective) data frames.
* Splitting the data between training and testing.
* Instantiation of the logistic regression model.
* Fitting the training data to the logistic regression model.
* Making the pertinent predictions and evaluating the model.
* In the end, the training data was resampled and a new logistic regression model wwas built.

## Results

Machine Learning Model 1 (with original data):
* Accuracy: 0.9924164259182832
*               precision    recall  f1-score   support

           0       1.00      0.99      1.00     56277
           1       0.85      0.89      0.87      1875



Machine Learning Model 2 (with resampled data):
* Accuracy: 0.9952022286421791
*               precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      1.00      0.93       625

## Summary

* With oversampled data the logistic regression model performs better overall, although it's still much better at predicting healthy loans (0) than high-risk loans (1) – as the model built using the original data. The accuracy is higher and performs better on precision and recall. I'd recommend using this model.
* Performance depends on whether it's more critical for us to find healthy loans (0) or high-risk loans (1) with higher accuracy.
