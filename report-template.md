
## Overview of the Analysis

* The purpose of this analysis is to compare to models for predicting healthy and high-risk loans
* The data consists of existing loans and their status as either healthy or high-risk
* The model was tring to predict loan status based on the rest of the data set.
* First, we imported the data into a pandas dataframe, then separated the x and y variables and created training and tsting data.
  After that, we used the training and testing data to create 2 models, one using a logistic regression on the training data and one that used a logistic regression on resampled data that would predict high-risk loans.

## Results

* Machine Learning Model 1:
This model fit a logistic regression model to some training data
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  * Healthy loans precision - 1.00
  * Healthy loans recall - 1.00
  * High-risk loans precision - 0.87
  * High-risk loans recall - 0.89


* Machine Learning Model 2:
This model used a logistic regression on resampled data.
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  * Healthy loans precision - 0.9
  * Healthy loans recall - 0.99
  * High-risk loans precision - 0.99
  * High-risk loans recall - 0.89

## Summary

Model performance depends on what we are looking for, ff we want to predict healthy loans, the first model is very good at identifying true positives for healthy loans, with a precision and recall of 1.00 for healthy loans. If we want to find high-risk loans, the second model is more precise but both have similar recall values, missing 11% of the true positives for high risk loans.
