# Project: **Machine Learning Model to Find Best Location For Building a Well**

## Description and Purpose of Project:

In this project, we created a Linear Regression Machine Learning Model for the OilyGiant company. The company provided us with oil samples from 3 different regions, in which the parameters of each oil well in the region are already known. The purpose of this mahcine learning model was to pick the region with the highest profit margin. Similarly, we analyzed the potential profit and risks using the Boostrapping technique.

The steps to choose the location were the following:
- Collect the oil well parameters in the selected region: oil quality and volume of reserves
- Build a model for predicting the volume of reserves in the new wells
- Pick the oil wells with the highest estimated values
- Pick the region with the highest total profit for the selected oil wells.

For this project, we had into account the following conditions:
1. Only linear regression is suitable for model training (the rest are not sufficiently predictable).
2. When exploring the region, a study of 500 points is carried with picking the best 200 points for the profit calculation.
3. The budget for development of 200 oil wells is 100 USD million.
4. One barrel of raw materials brings 4.5 USD of revenue The revenue from one unit of product is 4,500 dollars (volume of reserves is in thousand barrels).
5. After the risk evaluation, keep only the regions with the risk of losses lower than 2.5%. From the ones that fit the criteria, the region with the highest average profit should be selected.
6. The data is synthetic: contract details and well characteristics are not disclosed.

With that said, below is the structure of the project: 
```
1. Downloading and preparing the data.
2. Training and testing the model for each region:
  2.1. Spliting the data into a training set and validation set at a ratio of 75:25.
  2.2. Training the model and making predictions for the validation set.
  2.3. Saving the predictions and correcting answers for the validation set.
  2.4. Printing the average volume of predicted reserves and model RMSE.
  2.5. Analyzing the results.
3. Preparing for profit calculation:
  3.1. Storing all key values for calculations in separate variables.
  3.2. Calculating the volume of reserves sufficient for developing a new well without losses. Compare the obtained value with the average volume of reserves in each region.
  3.3. Providing the findings about the preparation for profit calculation step.
4. Writing a function to calculate profit from a set of selected oil wells and model predictions:
  4.1. Picking the wells with the highest values of predictions.
  4.2. Summarizing the target volume of reserves in accordance with these predictions
  4.3. Providing findings: suggest a region for oil wells' development and justify the choice. Calculate the profit for the obtained volume of reserves.
5. Calculating risks and profit for each region:
  5.1. Using the bootstrapping technique with 1000 samples to find the distribution of profit.
  5.2. Finding average profit, 95% confidence interval and risk of losses. Loss is negative profit, calculate it as a probability and then express as a percentage.
  5.3. Providing findings: suggest a region for development of oil wells and justify the choice.
```

## Business value:
The business value from this project was to provide analysis by means of machine learning and bootsrapping to determing the region that would yield the highest profit margin for the OilyGiant Company. 

## Tools and concepts used in project:
- Boostrapping 
- pandas
- numpy
- sklearn.model_selection 
- LinearRegression
- sklearn.metrics (f1_score, roc_curve, accuracy_score, roc_auc_score, mean_squared_error, r2_score) 
- matplotlib.pyplot
- scipy.stats

## Table of contents:
```
1  Libraries used for Analysis
2  Data Used for Analysis
  2.1  data_geo_0 dataframe
  2.2  data_geo_1 dataframe
  2.3  data_geo_2 dataframe
3  Creating a Linear Regression Model for Each Region
  3.1  data_geo_0 Linear Regression Model
    3.1.1  Analyzing the Linear Regression Model Results for predicted validation set
  3.2  data_geo_1 Linear Regression Model
    3.2.1  Analyzing the Linear Regression Model Results for predicted validation set
  3.3  data_geo_2 Linear Regression Model
    3.3.1  Analyzing the Linear Regression Model Results for predicted validation set
4  Sufficient volume units of reserve for profit
5  Risk and Profit
  5.1  Region_0
  5.2  Region_1
  5.3  Region_2
6  General Conclusion
```
