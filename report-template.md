# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of the analysis was to realize the importance of balanced data in machine learning and to learn the techniques that would help any data scientist remove imbalance from the dataset and improve it's performance resultantly.

* Explain what financial information the data was on, and what you needed to predict.
The dataset was about customers involved in taking loan from banks. It was a classification problem where using the 7 feature columns we had to predict whether the loan was healthy or risky.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
We were trying to predict the `loan_status` from the dataset. `loan_status` had two classes, `0` healthy loan, and `1` risky loan. Our objective was to predict the `loan_status` of customers based on dataset we were provided.

* Describe the stages of the machine learning process you went through as part of this analysis.
We went through the following machine learning statges:
1. Data Loading to load the data from csv into arrays.
2. Data Analysis to analyze the data and see if it's imbalanced.
3. Data Preparation to split the data into suitable training and testing sets.
4. Define the model that would make the predictions. 
5. Training the model on the training set.
6. Testing the model on the test set and making conclusions. 
7. We also went through an additional stage where we over sampled the data to improve performance of the model.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
We have used the following methods in our program:
1. LogisticRegression: A classification machine leanring algorithm that learns to classify classes based on the given training set. It comes with different methods to train, test, and predict the examples.
2. balanced_accuracy_score: It was used to get the balanced accuracy score of the predictions made by the model.
3. confusion_matrix: To draw the confusion matrix of the model predictions. It helps to evaluate the performance of a model.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. 

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  Accuracy:       0.95
  Precision:      0.99
  Recall:         0.99



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  Accuracy:       0.99 
  Precision:      0.99
  Recall:         0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Logistic Regression did a great job with the predictions as it was a simple problem. If we had used extreme gradient boosting, the results could have been even better. This is because gradient boosting is an ensemble model and makes use of other models to predict even better. 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Yes, the performance does depend on the problem we are trying to solve. For example, mis classifying someone as not having cancer is worse than mis classifying a person to have cancer. This is because the person mis classified to have cancer could be corrected by the further treatments and tests he would go through in the hospital, but the person who has cancer and has been classified to not have cancer, he won't even get to know about his disease and this would lead to serious troubles.

If you do not recommend any of the models, please justify your reasoning.
For simple datasets like this, Logisitc Regression works great but if we wanna increase the performance of our model we could use SVMs, they are large margin classifiers and could boost up the accuracy score even more.