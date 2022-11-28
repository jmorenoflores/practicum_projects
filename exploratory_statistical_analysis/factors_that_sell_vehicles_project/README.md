# Project: **What sells a car?**

## Description and Purpose of Project:

At Crankshaft List, hundreds of free advertisements for vehicles are published on site every day. We studied the data collected over the last few years to determine which factors influenced the price of a vehicle. The purpuse of **the What sells a car?** project is to analyze data from vehicles, such as model, model year, condition of the vehicle, number of cylinders, type of fuel, type of transmission, and other characteristic of vehicles; and determine which of these vehicle attributes influence the pricing of a vehicle.

For this project, we studied the following parameters: price, vehicle's age when the ad was placed, mileage, number of cylinders, and condition and plotted histograms for each of these parameters. Similarly, we analyzed how outliers affected the form and readability of the histograms. For these plots, we determined the upper limits of outliers, removed the outliers and stored them in a separate DataFrame, and continued working with the filtered data without outliers.

With the filtered data, we used it to plot new histograms, compared them with the earlier histograms (the ones that included outliers) and drew conclusions for the distributions. Similarly, we studied how many days advertisements were displayed (days_listed), plotted a histogram, and calculated the mean and median values for the distributions to describe the typical lifetime of an ad. With the distribution descriptive values, we determined when ads were removed quickly, and when they were listed for an abnormally long time.

Finally, we analyzed the number of ads and the average price for each type of vehicle. Furthermore, we plotted a graph showing the dependence of the number of ads on the vehicle type. With this in mind, we selected the two types with the greatest number of ads. The last business question we answered was the following:
- *What factors impact the price most?*

For this, we took each of the popular types we detected at the previous stage and studied whether the price depends on age, mileage, condition, transmission type, and color. For categorical variables (transmission type and color), we plotted box-and-whisker charts, and created scatterplots for the rest. When analyzing categorical variables, note that we selected categories thad had at least 50 ads; otherwise, their parameters wouldn't been valid for our analysis.

## Business value:

The business value from this project incude an analysis of the factors that influence the pricing of a vehicle to plan advertising campaigns accordingly. 
## Tools and concepts used in project:

- pandas
- datetime
- numpy
- matplotlib.pyplot 
- seaborn
## Table of contents: 
```
1  Project: What sells a car?
  1.1  Initialization
  1.2  Load data
  1.3  Explore initial data
    1.3.1  Description of data
    1.3.2  Fixing innapropriate data types in columns
    1.3.3  Conclusions and further steps for initial data
  1.4  Treating missing values
    1.4.1  odometer
    1.4.2  model_year column
    1.4.3  cylinders column
    1.4.4  paint_color column
    1.4.5  is_4w column
  1.5  Fix data types
    1.5.1  model_year column
    1.5.2  cylinders column
    1.5.3  odometer column
    1.5.4  is_4wd column
    1.5.5  date_posted column
  1.6  Enrich data
    1.6.1  weekday_posted, month_posted, year_posted, and vehicle_age columns
    1.6.2  avg_miles_per_year
  1.7  Check and clean data
    1.7.1  avg_miles_per_year column
  1.8  Study core parameters
    1.8.1  price parameter
    1.8.2  age parameter
    1.8.3  avg_miles_per_year parameter
    1.8.4  cylinders parameter
    1.8.5  condition parameter
  1.9  Study and treat outliers
  1.10  Study core parameters without outliers
    1.10.1  core parameter: price
    1.10.2  core parameter: vehicle_age
    1.10.3  core parameter: avg_miles_per_year
    1.10.4  core parameter: cylinders
    1.10.5  core parameter: condition
  1.11  Ads lifetime
  1.12  Average price per each type of vehicle
  1.13  Price factors
    1.13.1  Condition factor
    1.13.2  paint color factor
    1.13.3  transmission factor
  1.14  General conclusion
  ```
