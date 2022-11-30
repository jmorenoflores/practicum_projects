# Project: **Machine Learning Model to Pick the Right Mobile Plan**

## Description and Purpose of Project:

Mobile carrier Megaline has found out that many of their subscribers use legacy plans. The purpose of this project was to develop a machine learning model that would analyze subscribers' behavior and recommend their customers one of Megaline's newer plans: Smart or Ultra. In this project, we analyzed the behavior data about subscribers who have already switched to the new plans. For this classification task, we developed a model that will pick the right plan and picked the model with the highest possible accuracy score. Megaline specified that the threshold for accuracy was 0.75.

The structure of the project is decribed below: 

1. Downloading the dataset
2. Spliting the source data into a training set, a validation set, and a test set.
3. Investigating the quality of different models by changing hyperparameters. Briefly describing the findings of the study.
4. Checking the quality of the model using the test set.
5. Sanity check the model.

## Business value:
The business value from this project was to provide Megaline a machine learning model that would recommend their customers one of Megaline's newer plans: Smart or Ultra, based on the model's predictions. 

## Tools and concepts used in project:

- pandas
- DecisionTreeClassifier
- RandomForestClassifier
- sklearn.metrics (accuracy_score)
- sklearn.model_selection (train_test_split)
 
## Table of contents:
```
1. Project: Creating a Model to Pick the Right Mobile Plan
2. Description of users' behavior data
3. Model 1: Decision tree
  3.1 1  Model 1: sanity check
4. Model 2: Random Forest
  4.1 2  Model 2: sanity check
5. General Conclusion
```
