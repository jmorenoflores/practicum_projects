# Project: **Analyzing Borrowers’ Risk of Loan Defaulting**

## Description and Purpose of Project:

The loan division of a bank had provided data of their customers to find out if a customer's marital status and number of children have an inpact on whether they will default on a loan. The bank already has some data on customers’ credit worthiness. The purpose of this report was to analyze the relationship between default rate on loans and marital status and/or the number of children. This report was used to analyze if there is a increasing default rate on a loan as the number of children increase; as well as if being a widow, widower, divorced, or unmaried has a higher default rate compared to individuals who are married or in a civil partnership.

The following hypotheses were tested using the preprocessed data, after checking for errors and null values:

- Is there a correlation between having children and paying back on time?
- Is there a correlation between family status and paying back on time?
- Is there a correlation between income level and paying back on time?

## Business value:

This report will be considered when building a credit score for a potential customer. A credit score is used to evaluate the ability of a potential borrower to repay their loan.

## Tools and concepts used in project:
- pandas
- numpy
- math
- matplotlib.pyplot

## Table of contents: 
```
1  Data exploration
  1.1  Checking for Null Values in Columns
  1.2  Summary of Null Values in Columns
  1.3  Intermediate conclusion
  1.4  Distrubution of Missing values per categories of education, income type, and family status.
  1.5  Possible reasons for missing values in data
  1.6  Intermediate conclusion
  1.7  Conclusion
2  Data transformation
  2.1  education column
  2.2  children column
  2.3  days_employed column
  2.4  dob_years column
  2.5  family_status column
  2.6  gender column
  2.7  income_type column
  2.8  checking for duplicates
  2.9  Restoring missing values in total_income
    2.9.1  Distribution of values of factors that affect income
    2.9.2  intermediate conclusion
  2.10  Restoring values in days_employed
3  Categorization of data
4  Checking the Hypotheses
```
