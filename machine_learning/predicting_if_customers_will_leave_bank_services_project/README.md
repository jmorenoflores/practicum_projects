# Project: **Will Costumers leave soon?**

## Description and Purpose of Project:

Beta Bank customers are leaving: little by little, chipping away every month. The bankers figured out it’s cheaper to save the existing customers rather than to attract new ones. This project was used to create a machine learning model that predicts whether a customer will leave the bank soon based on the data of clients’ past behavior and termination of contracts with the bank.

The project consisted of creating a DecissionTreeClassifier and a RandomForestClassifier model from the data; tuning each of the models' hyperparameters to obtain the highest F1 score, accuracy score, and AUC value from the ROC curve; The best model with the highest F1, accuracy, and AUC values was picked for the findings of task research. The threshold for the F1 score was a score of at least 0.59.

The structure of the project and instructions were the following: 
```
- Downloading and preparing the data. (Explaining the procedure)
- Examining the balance of classes. Training the model without taking into account the imbalance. Briefly describing the findings.
- Improving the quality of the model by using at least two approaches to fixing class imbalance. 
- Using the training set to pick the best parameters. 
- Using different models on training and validation sets and finding the best one. Briefly describing the findings.
- Performing the final testing.
```
## Business value:

The Business value from this project was provide a machine model that would preduct whether a client would leave the bank's services, so the bankers can try to retain these clients at risk of leaving. 

## Tools and concepts used in project:

- pandas
- numpy
- DecisionTreeClassifier
- RandomForestClassifier
- sklearn.model_selection
- matplotlib.pyplot
- OrdinalEncoder
- StandardScaler
- sklearn.metrics (f1_score, roc_curve, accuracy_score, roc_auc_score)
- sklearn.utils.shuffle
- RandomizedSearchCV
- GridSearchCV
- linear_model

## Table of contents:
```
1  Libraries Used for Analysis
2  Description of Data
3  Preparing the data for Analysis
  3.1  column names in data
  3.2  rownumber column
  3.3  customerid column
  3.4  surname column
  3.5  creditscore column
  3.6  geography column
  3.7  gender column
  3.8  age column
  3.9  tenure column
  3.10  balance column
  3.11  numofproducts column
  3.12  hascrcard column
  3.13  isactivemember column
  3.14  estimatedsalary column
4  Model 1: DecisionTreeClassifier
5  Model 2: RandomForest
6  Selecting Best model
7  Conclusion
```
