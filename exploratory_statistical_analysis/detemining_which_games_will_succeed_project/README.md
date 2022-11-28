# Project: **Will the game succeed?**

## Description and Purpose of Project:

The project **Will the game succeed?** used data from the online store *Ice*, which sells video games all over the world. The data had information about the user and expert reviews, genres, platforms, sales, and rating of videogames sold in 2016. The purpose of this project was to identify patterns that determined whether a video game was going to succeed in 2017, and also allow us to spot potential big winners to plan advertising campaigns.

For the analysis component of this project we looked at the number of games were that released in different years and also checked if the number of released games, for, every period was significant for our analysis. Similarly, we looked at patterns of how sales varied from platform to platform, and chose the platforms with the greatest total sales. From the list of platforms with greatest sales, we visualized distributions of sales based on data for each year. With the use of number of sales from each platform, we determined the platforms that used to be popular, but now have zero sales to answer the following business question:

*How long does it generally take for new platforms to appear and old ones to fade?.*

Consequently, we determined the period we should take data for to build a prognosis for 2017. In other words, we decided to work only with the data that we had decided is relevant and disregarded the data for previous years. With the use of relevant data, we analyzed the platforms that were leading in sales; the platforms that were growing or shrinking; and selected several potentially profitable platforms. From the list of chosen platforms, we studied how user and professional reviews affected sales for this popular platform and answer the following business questions:

1. *What can we say about the most profitable genres?*
2. *Can we generalize about genres with high and low sales?*

## Business value:

This business value that this project provided include an analysis of patterns that determine the video games that will succeed in 2017 to plan advertising campaigns. Similarly, this project provided patterns of video game platforms and genres of video games that were profitable, leading and gowing in sales to plan advertising campaigns accordingly. 
## Tools and concepts used in project:
- pandas
- numpy
- datetime
- matplotlib.pyplot
- seaborn 
- scipy.stats

## Table of contents:
```
1  Description of project:
  1.1  Dictionaries used for analysis
  1.2  Data used for analysis
2  Description of data
  2.1  General Information of data
  2.2  Description of missing values in columns
3  Head of data
4  Preparing the data
  4.1  name column
    4.1.1  Fixing data type
    4.1.2  Fixing values in column
    4.1.3  Replacing missing values in column
    4.1.4  Deleting duplicates
  4.2  platform column
    4.2.1  Fixing data type
    4.2.2  Fixing values in column
    4.2.3  Replacing missing values in column
  4.3  genre column
    4.3.1  Fixing data type
    4.3.2  Fixing values in column
  4.4  na_sales column
    4.4.1  Fixing values in column
  4.5  eu_sales column
    4.5.1  Fixing data types in column
  4.6  jp_sales column
    4.6.1  Fixing values in column
  4.7  other_sales column
    4.7.1  Fixing values in column
  4.8  year_of_release column
    4.8.1  Replacing missing values in column
    4.8.2  Fixing data type in column
    4.8.3  Removing duplicates in data
  4.9  critic_score column
    4.9.1  Fixing missing values in column
    4.9.2  Fixing data type in column
  4.10  user_score column
    4.10.1  Fixing values in column
    4.10.2  Fixing missing values in column
    4.10.3  Fixing data type in column
  4.11  rating column
    4.11.1  Fixing missing values in column
  4.12  Enriching data
5  Analyze the data
  5.1  Games released per year
  5.2  Pattern of sales per platform
    5.2.1  Platforms that used to be popular, and now have zero total sales.
    5.2.2  How long does it take for old platforms to fade?
    5.2.3  How long does it take for new platforms to appear?
  5.3  Selecting relevant games from data
  5.4  Platforms with growing and shrinking total sales
    5.4.1  Leading total sales platforms
    5.4.2  Growing and shrinking patterns
  5.5  Distribution of total sales per plaform
  5.6  How does professional and user reviews affect total sales for a platform?
  5.7  Comparing total sales of same games in other platforms.
  5.8  Distribution of total sales by video game genres
6  User profiles for each region
    6.0.1  Top 5 leading sales platform foe each region
    6.0.2  Top 5 leading sales genres for each region
    6.0.3  Do ESRB ratings affect sales in individual regions?
7  Testing statistical hypothesis
    7.0.1  XOne and PC user ratings
    7.0.2  Action and Sports user ratings
8  General Conclusion
```

