# Module 12 Report Template

## Overview of the Analysis

Could you describe the analysis you completed for the machine learning models used in this Challenge in this section? This might include:

* Explain the purpose of the analysis.
  The goal is to determine if the Logistic Regression model can be accurate in predicting healthy loans vs high-risk loans using original data vs resample data to increase the size of the minority class
  
* Explain what financial information the data was on, and what you needed to predict.
  loan_status is predictions
  
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
  original
  vaules_counts
  0   75036
  1    2500

  oversample
  0   56271
  1   56271
  
* Describe the stages of the machine learning process you went through as part of this analysis.
1. Prepare data
2. separate the data into features aka columns which X and Y are the outcomes or aka labels
3. train_test_split
4. pick the ml model for classification so LogisticRegression
5. Fit the model with training data
6. Use the Model to make predictions with the test data so 25% of default test data to be evaluated
7. Evaluate the predictions comparing metrics. confusion metric, classification report
   
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
  SKLearn LogisticRegression
  Train_test_split
  confusion_matrix
  Classification_report

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1
    * Accuracy: 0.99
    * Precision 0: 1.00, class: 0.85
    * Recall scores 0: 0.99, Class 1: 0.95

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
The logistic regression model performed well especially the prediction of the outcome of 0 healthy loans
for class 0 both the precision and recall were extremely high

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Given the info, it appears that logistic regression models do a great job at predicting both healthy and
high-risk loans given the features that used to train set data

Although the logistic regression model appears promising it would need to be evaluated against different
data sets to confirm that it should be put into use for the prediction health status of loans

If you do not recommend any of the models, please justify your reasoning.
