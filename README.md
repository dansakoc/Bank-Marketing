# Bank Marketing Campaign Analysis
![](https://github.com/dansakoc/Image/blob/master/Bank%20image.jpg?raw=true)



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
The outcome variable shows 36548 clients responded no and 4640 responded yes which is respectively 89% negative answer and 11% positive answer.A low number of clients responded to a term deposit.

### 1 Categorical variable exploration

#### Age category variable
By grouping the respondents, I noticed that more seniors were interviewed during this campaign than other group.
![Age category](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Age_cateogry.png?raw=true)


#### Job title varaiable
Large number of subscribers of a term deposit where Admin followed by technician, Blue Colar and retired.Those with a job title of  Housemaid, unemployed, entrepreneur, self-employed responded more negatively to a term deposit
![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Job.png?raw=true)


#### Education variable
University degree holders responded more positively to the campaign
![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Education.png?raw=true)



#### Marital status
Married couples where more subscribers than single and divorced clients
![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Marital.png?raw=true)



#### Loan and default on loan
Clients with no loan, and no credit default subscribed more to a term deposit.
![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20default.png?raw=true)![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Loan.png?raw=true)




### 2 Numerical variable exploration


#### Deposit and Duration
 The average duration for a term deposit is 500 which can lead to a term deposit

![](https://github.com/dansakoc/Image/blob/master/Deposit%20vs%20Duration.png?raw=true)





## Fitting the model

1 Random Forest model

2 Glm model

3 Decision trees model 

To make a fair comparison of the three modes I created a control parameter.
I run these three models and I use the ROC metric to evaluate each model. To compare the models, I plotted a dotplot, boxplot and density plot. The Summary of the models shows that the ROC of the Random Forest was higher than the two other models.


#### Model comparison with boxplot 
![](https://github.com/dansakoc/Image/blob/master/Boxplot%20picture.png?raw=true)

### Model comparison with dotplot
![](https://github.com/dansakoc/Image/blob/master/Dotplot%20picture.png?raw=true)

### Model comparison with density plot
![](https://github.com/dansakoc/Image/blob/master/Density%20plot.png?raw=true)



# Conclusion
Random forest is the best model in this case to predict the client decision to make a term deposit. Many features like the clients age, bank account, loan ,the duration and nr.employed can be good predictors to build a model to understand the behaviors of a client to accept a Term deposit. 










