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
                  precision    recall  f1-score   support

           0       1.00      0.99      1.00     56277
           1       0.85      0.89



Machine Learning Model 2 (with resampled data):
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
