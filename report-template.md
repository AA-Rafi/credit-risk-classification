# Module 12 Report Template

## Overview of the Analysis


The objective of this analysis is to map models on top of data containing loan information to understand the risk associated with them. The models used different types of techniques to ultimalty deploy a Logistic Regression Model that would predict if the loan was either 0, a healthy loan, or 1, a high-risk loan. 

The analysis involved the following:
* From the original dataset, features were established through splitting which were used to creating training and testing sets to create the models

* Machine Learning Model 1 (Model1 in the file) was created by developing a logistic regression model, training it using the initial training sets (x_train, y_train), fitting it to the training sets, and utilizing it for predictions.

* Another logistic regression model was instantiated (Model2 in the data) by resampling the initial training data using the RandomOverSampler module. This resampled model was then fitted to the resampled training sets (x_resample, y_resample), and predictions were made.

The performance of each model was evaluated based on metrics such as balance accuracy score, confusion matrix, precision, recall, and f1-score, as presented in the classification report.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Overall the model is accurate, with a precision of 94%. With it being able to tell healthy loans 100% of the time but high risk loans 87% of the time. Although, paired with the recall rate (that is the correct identification of type of loan) for high risk loans is 89% the model is overal satisfactory on its high risk loan side of things but a better model should still be considered.

* Machine Learning Model 2:
  * There is a slight improvment from the original regression model. Notably in the accuracy score, going from around 94% to 99%. There is now 100% in the recall ability for both healthy and high risk loans, where that wasnt the case with the original model. Overall this model scores greater than the previous model, making it the better model for use. 

## Summary

Based on the analysis, Model 2 demonstrates higher overall accuracy and outperforms Model 1 in predicting high-risk loans. Specifically, Model 2 successfully identifies all high-risk loans in the dataset and achieves a relatively strong precision in high-risk loan prediction. This performance is considered commendable in this context. To accurately identify high-risk loans and improve overall label predictions, I recommend utilizing Model 2 over Model 1. In real life deployment, there are much more factors that should also be considered in this model, such as a further examination of the degrees of high risk associated with each loan. 
 