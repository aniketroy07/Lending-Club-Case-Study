# Load Data Analysis using Lending Club Dataset
- Lending Club is the largest online loan marketplace, offering products like 
       1. Personal Loans
       2. Business Loans
       3. Financing medical procedures
- Borrowers can apply and access these products through an online interface
- But lending loans to highly risky applicants can cause a very large credit loss
- Therefore, we must identify the driving factors that are strong indicators of a loan defaulter



## Table of Contents
* [Overall Approach](#general-information)
* [Missing Value Treatment](#technologies-used)
* [Outlier Treatment](#conclusions)
* [Feature Engineering](#acknowledgements)
* [Exploratory Data Analysis (EDA)](#acknowledgements)
* [Recommendations](#acknowledgements)

## Overall Approach
- We first load the dataset
- Perform missing value treatment
- Perform outlier treatment
- Perform feature engineering
- Perform Exploratory Data Analysis (EDA)
- Finally, we deliver our recommendations

## Missing Value Treatment
- Dropped all the columns that had at least 30% missing values as imputing these will result in bias/de-authentication of data
- Dropped all those rows whose respective columns had insignificant number of missing values. Dropping these will not result in data loss as the number is insignificant

## Outlier Treatment
- Removing the outliers by making sure we are not losing a significant amount of data
- We may still have some outliers in the data, which is fine.  Because, if we drop them, there will be a significant loss of data


## Feature Engineering
- Continuous features have values that are absolute numbers and trying to compare the absolute numbers with "Defaulters" and "Non-defaulters" will be difficult and make no sense. Hence, we can segment these data-points within features such that each segments have data-points that are homogenous to each other, and the  segments are heterogenous amongst each other

## Exploratory Data Analysis(EDA)
- Here we performed univariate, bivariate and multivariate analysis to ultimately draw inferences about the data and provide accurate recommendations

## Recommendations
- As observed in the EDA, interest rates, loan amount,  debt to salary ratio, salary, grade of debt and term of debt are the key drivers of loan defaulting. Following are our recommendations,
- To the applicants with low salary, high loan amount requirement, high debt to salary ratio, higher grade of debt and higher term requirement, we can approve a loan of an amount not to high but with a high interest as they are very high risky applicants
- To the applicants with medium salary, medium loan amount requirement, medium debt to salary ratio, medium grade of debt and medium to low term requirement, we can lend a slightly higher loan amount and a slightly lower interest rate than the highly risky applicants
- To the applicants with high salary, low loan requirement, low debt to salary ratio, low grade of debt and with a low term requirement, we can lend a higher amount as required with a standard or low interest rates as they are the least risky applicants


## Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn

## Contact
Created by [@aniketroy07] - feel free to contact me!
