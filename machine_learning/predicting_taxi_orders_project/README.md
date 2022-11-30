# Project: **Predicting Number of Taxi Orders**

## Description and Purpose of Project:

Sweet Lift is a taxi company that has collected historical data on taxi orders at airports. The purpose of this project is to attract more drivers during peak hours and predict the amount of taxi orders for the next hour by building a machine learning model for such a prediction. To create such machine learning model, we had to analyze the rolling mean and standard deviation of DateTime data with different window sizes to obtain smooth rolling and observe trends and seasonality in daily, and monthly periods. After analyzing and determining the window sizes that provided a smooth rolling for mean and standard deviation, we created lags of DateTime data as features to train and test Machine Learning modes including RandomForestRegressor, DecisionTreeRegressor, CatboostRegressor, and XGBRegressor models. The company’s RMSE threshold specifications were the folllwing: The RMSE metric on the test set should not be more than 48.

Below is a description of the structure of the project: 

1. Downloading  the data and resample it by one hour.
2. Analyzing the data.
3. Training different models with different hyperparameters. The test sample was 10% of the initial dataset.
4. Testing the data using the test sample and provide a conclusion.


## Business value:

The business value from this project was to attract more drivers during peak hours and predict the amount of taxi orders for the next hour with the use of a machine learning model. 

## Tools and concepts used in project:
- Time Series
- pandas
- numpy
- statsmodels.tsa.seasonal.seasonal_decompose
- matplotlib.pyplot
- LinearRegression
- sklearn.model_selection (train_test_split, RandomizedSearchCV, GridSearchCV, cross_val_score)
- sklearn.metrics(mean_squared_error, make_scorer)
- RandomForestRegressor 
- DecisionTreeRegressor
- CatBoostRegressor
- XGBRegressor 
- TimeSeriesSplit

## Table of contents:
```
1  Project instructions/Specifications
2  Libraries Used for Anlysis
3  Data description
4  Preparation and Analysis
5  Training
  5.1  RadomForestRegressor Model
  5.2  DecisionTreeRegressor
  5.3  CatBoostRegressor
  5.4  XGBRegressor Model
  5.5  Conclusion from Training
6  Testing
7  Conclusion
```


