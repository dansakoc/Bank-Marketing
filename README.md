# Bank Marketing campaign Analysis

## Introduction
This project is a bank marketing campaign from Portuguese banking institution to determine if a client will subscribe to a bank term deposit. The data includes predictors which can influence the client decision and an outcome variable with a binary answer. I applied a machine learning technique in this case the classification method to find the best model to use for the data. 

## About the data

 1. Source: Bank Marketing uci repository
        https://archive.ics.uci.edu/dataset/222/bank+marketing
        
 2. Time Period: May 2008 to November 2010
   
 3. Variables: 21

## Data transformation and manipulation

The outcome variable was renamed deposit.

I Transformed the categorical variable to factors for R to process the data normally.

For a better view of the histograms, I added a log to some numerical variables.

I added a new variable Age_Category to group the age into 3 categories: senior, adults, youth.


## Data Exploration
The outcome variable shows 36548 clients responded no and 4640 responded yes which is respectively 89% negative answer and 11% positive answer.

#### Age category variable
By grouping the respondents, I noticed that more seniors were interviewed during this campaign.
![Age category](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Age_cateogry.png?raw=true)


#### Job title varaiable
![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Job.png?raw=true)

#### Education variable
![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Education.png?raw=true)







