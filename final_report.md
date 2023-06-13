# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

With the imbalanced dataset we used for this prediction exersice, the classification report has a high degree of precision and f1-score for 
health loans, but for the High-Risk loans the scores are much lower. Because of the lower recall value on the High-Risk loans, the model 
might predict false positives and false negatives.




* Machine Learning Model 2:

After performing adjustments for the imbalance of the data using the RandomOverSampler(), there is a significant 
improvement on the classification report. The precision score for the High-Risk loans did not change significantly, 
but the recall, accuracy and f1-score improved a lot. This adjustment will improve the performance of the model 
eliminating a lot of false positives and false negatives.


## Summary

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

The model, when trained with the original data presented a good accuracy on the predictions, but the accuracy and recall were noticebly low.
This situation was caused because there was a significant imbalance on the dataset, with 96% of Healthy Loans but ony 4% of High-Risk loans.

After performing an adjustment using the RandomOverResample() on the data, the results of the model, both on accuracy, precision, recall 
and f1-score improved significantly. 

Since it is import that the model perform with high precision on avoiding false negatives, so we do not underevaluate the 'High-Risk loans',
the adjustment for the dataset imbalance was appropriate.

After the rebalancing of the sample data and retraining the model, we finished with a good model that can be used to predict High-Risk 
loans satisfactorily.


If you do not recommend any of the models, please justify your reasoning.
