# Report: Predict Bike Sharing Demand with AutoGluon Solution

## Project 1: AWS ML Nanodegree Course 1 Project 1

## **Initial Training**


## **Q1 **
What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?

## Ans:
All the values of the predictor must be greater than or equal to zero. Actualy, the results of the prediction are all positive values.

## **Q2**
What was the top ranked model that performed?

## Ans:
WeightedEnsemble_L3

# **Exploratory data analysis and feature creation**

## **Q3**
What did the exploratory analysis find and how did you add additional features?


## Ans:
The Exploratory Data Analysis helps to visualize the distribution of the data. Histogram is used to visualize the data distribution. During the EDA it is found that some of the features are continuous while others are discrete.

Additional features are added by employing the year, month, day and hour variables of the datetime data type.


## **Q4**
How much better did your model preform after adding additional features and why do you think that is?**

## Ans:
The addition of the Year, Month, Day and Hour features and the change of numeric data types to Categorical data type has improved the model performance. The Kaggle score is improved from 1.798 to 0.630. This is a great improvement.

# **Hyper parameter tuning**

## **Q5**
How much better did your model perform after trying different hyper parameters?**

## Ans:
The Kaggle score is improved from 0.630 to 0.510, after some hyperparameter tuning with the same data.

## **Q6**
If you were given more time with this dataset, where do you think you would spend more time?**

## Ans:
Feature selection and feature Engineering would add more value as shown in the model accuracy with raw data and with some feature processing.

## **Q7**
Create a table with the models you ran, the hyperparameters modified, and the kaggle score.**



| model  | initial | new_features | HPO | Kaggle Score |
-------- | -------- | ----------- | ------- | ---------------------|
| WeightedEnsemble_L3 |  Default  |   Default   | Default | 1.79854 |
| WeightedEnsemble_L3 | Default | Default | Default | 0.63043 |
| WeightedEnsemble_L2 | Default | Default | RF, CAT, XGB | 0.51037 |
| Best Performing(Score) |  0.8166  |   0.99256   | 0.99013 |

## **Create a line plot showing the top model score for the three (or more) training runs during the project.**

![model_test_score.png](attachment:model_test_score.png)

## **Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.**

![kaggle_score.png](attachment:kaggle_score.png)

## Create a graph showing changes of model evaluation metrics after each model iteration.

![model_score.png](attachment:model_score.png)

## **Summary**

## Feature engineering has great importance on the data modeling and accuracy of models. Also, finetuning hyperparameters would have a great impact on the final results but using the default parameters would be an intitial step to make comparison.

---


```python

```
