# Term Deposit Subscription: Project Overview
* Cleaned data, performed exploratory analysis and did some feature engineering
* Optimized Logistic Regression & K-Nearest Neighbours using GridSearchCV to reach the best model
* Built a classification model to predict whether or not clients will subscribe to a term deposit facilitated by a banking institution

## Code & Resources Used
* **Jupyter Notebooks**: Python 3  
* **Packages**: pandas, numpy, sklearn, matplotlib, seaborn  
* **Data Source**: https://www.kaggle.com/gowthamchowdry/bank-classifying-term-deposit-subscriptions/data  

## Data Cleaning
After fetching the data, I needed to clean it up so that it can be used for building the classification model.
The cleaning process involved the following tasks.  
* Dealt with the missing values
* Dealt with outliers
* Removed the column for month of last contact

## EDA
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights.    
![](https://github.com/pranavjoshi-hub/term-deposit-subscription/blob/main/visualizations/job_type_counts.png
)
![](https://github.com/pranavjoshi-hub/term-deposit-subscription/blob/main/visualizations/heat_map.png)
![](https://github.com/pranavjoshi-hub/term-deposit-subscription/blob/main/visualizations/prediction_by_education.png)

## Model Building
First, I transformed the categorical variables into dummy variables. I scaled the numeric features to a standard range. I also split the data into train and test sets with a test size of 20%.

I tried three different models and evaluated them using R2.

Following are the three models I tried:

1. Gaussian Naive Bayes  
2. Logistic Regression  
3. K-Nearest Neighbours 

## Model Performance
The Logistic Regression model outperformed the Gaussian Naive Bayes model by some distance and the KNN model only marginally. Therefore, I optimized the Logistic Regression and KNN models to get the following results.

1. Logistic Regression - **89.4%** 
2. K-Nearest Neighbours - **89.3%** 

## Project Results
* The model shall enable the bank during promotional campaigns to identify and focus on potential clients who are predicted to subscribe to the term deposit.
* The model could help the bank save at least 30% on promotional expenses.
