# Term Deposit Subscription: Project Overview
* Cleaned data, performed exploratory analysis and did some feature engineering
* Optimized Logistic Regression & K-Nearest Neighbors using GridSearchCV to reach the best model
* Built a classification model to predict whether or not clients will subscribe to a term deposit facilitated by a banking institution

## Code & Resources Used
Jupyter Notebooks: Python 3  
Packages: pandas, numpy, sklearn, matplotlib, seaborn  
Data Source: https://www.kaggle.com/gowthamchowdry/bank-classifying-term-deposit-subscriptions/data  

## Data Cleaning
After fetching the data, I needed to clean it up so that it can be used for building the classification model.
The cleaning process involved the following tasks.  
* Dealt with the missing values
* Changed data-type of columns
* Dealth with outliers
* Removed column for month of last contact

## EDA
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights.  

## Model Building
First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.

I tried three different models and evaluated them using R2.

I tried three different models:

Gaussian Naive Bayes  
Logistic Regression  
K-Nearest Neighbours 

## Model Performance
The Logistic Regression model outperformed the Gaussian Naive Bayes model by some distance and the KNN model only marginally.  
1. Baseline Model Performance:  
**Gaussian Naive-Bayes** - 85.9%    
**Logistic Regression** - 89.4%  
**K-Nearest Neighbors** - 89%    

2. Optimized Model Performance:  
**Logistic Regression** - 89.4%  
**K-Nearest Neighbors** - 89.3%  
