# credit-risk-classification
# Module 20 Report

## Loan Analysis

The data provided lists various loans given of varying sizes with their accompanying metadata; loan size, interest rate, borrower income, ratio of debt to income, the number of accounts held, derogatory marks, total debt held, and their loan status (0 indicates a healthy loan, 1 indicates high risk loan).

* The goal is to predict whether a loan will be healthy or high risk based on the other metadata.
* Used `value_counts` as a metric to check on data size.
* Split the data using the "loan status" as the label and the rest of the columns as the features.

Created Linear Regression Model using the original data.
* Used sklearn to fit the data.
* Used testing data feature of linear regression models to create testing predictions.
* Created balanced accuracy score.
* Created a classification report based on the findings.

Created Linear Regression Model using Resampled Training Data
* Used RandomOverSampler with a random state of 1 
* Fit the original training data to the random sampler model.
* Used the value counts to check on data size.
* Used a classifier to fit the data.
* Saved Predictions to a dataframe
* Calculated the accuract score, a confusion matrix and a classification report.

## Results


* Machine Learning Model 1: Linear Progression Model using Original Data
  * True Positive and True Negative scores were high, indicating accurate predictions.
  * Low numbers indicate few false positives and false negatives. 
  * Balanced accuracy score of .952 is excellent.


* Machine Learning Model 2: Linear Regression Model using Resampled Training Data
  * True Positive and True Negative scores were high, indicating accurate predictions.
  * Low numbers indicate few false positives and false negatives. 
  * Balanced accuracy score of .946 is not as good but still great.
  * Extended Classification report shows 100% precision for predicting healthy loans.
  

## Summary

Both models seem to be very good at predicting healthy and risky loans, but when using the Original Data from Model 1 it seems a bit better.  However since the datasets were very different in value count size, more information should be examined.

* Model 1 has higher true predictions for both healthy and risky.   
* Model 1 also minimizes false positives and negatives.

