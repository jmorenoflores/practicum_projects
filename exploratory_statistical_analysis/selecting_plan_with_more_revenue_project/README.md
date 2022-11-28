# Project: **Which plan brings in more revenue?**

## Description and Purpose of Project:

Megaline is a company that offers its clients two prepaid plans, Surf and Ultimate. The commercial department wants to know which of the plans brings in more revenue in order to adjust the advertising budget.

The purpose of this project is to carry out a preliminary analysis of the plans based on a relatively small client selection. The data on 500 Megaline clients contains information about: who the clients are, where they're from, which plan they use, and the number of calls they made and text messages they sent in 2018. This project was conducted to analyze the clients' behavior and determine which prepaid plan brings in more revenue.

In this project, we proprocessed and removed errors in data. Consequently, we conducted analysis on each user to stydy the following:
- The number of calls made and minutes used per month
- The number of text messages sent per month
- The volume of data per month

The monthly revenue from each user (we subtracted the free package limit from the total number of calls, text messages, and data; and multiplied the result by the calling plan value; and added the monthly charge depending on the calling plan). We also analyzed and described the customers' behavior by finding the minutes, texts, and volume of data the users of each plan required per month. With this information, we calculated the mean, variance, and standard deviatiod and also plotted histograms to describe the distributions.

For this project, we tested the following hypotheses:
- if the average revenue from users of Ultimate and Surf calling plans differs.
- if the average revenue from users in NY-NJ area is different from that of the users from other regions.

## Business value:
Determine which mobile plan brings in more revenue to adjust the advertising budget accordingly. 

## Tools and concepts used in project:

- pandas 
- datetime
- relativedelta
- numpy
- math
- matplotlib.pyplot
- scipy.stats

## Table of contents:
```
1  Project: Which plan brings in more revenue?
  1.1  Initialization
    1.1.1  Libraries used for analysis.
  1.2  Load data
    1.2.1  calls_data DataFrame
    1.2.2  internet_data DataFrame
    1.2.3  messages_data DataFrame
    1.2.4  place_data DataFrame
    1.2.5  users_data DataFrame
  1.3  Prepare the data
    1.3.1  Plans_data
    1.3.2  Users_data
      1.3.2.1  Fix Data
      1.3.2.2  Enrich Data
    1.3.3  calls_data
      1.3.3.1  Fix data
      1.3.3.2  Enrich data
    1.3.4  Messages_data
      1.3.4.1  Fix data
      1.3.4.2  Enrich data
    1.3.5  Internet_data
      1.3.5.1  Fix data
      1.3.5.2  Enrich data
  1.4  Study plan conditions
  1.5  Aggregate data per user
    1.5.1  Total Revenue of each user per each month
  1.6  Study user behaviour
    1.6.1  Calls
    1.6.2  Messages
    1.6.3  Internet
  1.7  Revenue
  1.8  Test statistical hypotheses
  1.9  General conclusion
```
