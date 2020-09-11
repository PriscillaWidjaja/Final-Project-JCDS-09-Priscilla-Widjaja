# Final Project JCDS 09 - Priscilla Widjaja

## Deposit Term Subscription Prediction Machine Learning

A prediction machine learning project using classification algorithm that predicts whether the client will subscribe a term deposit or not.

Datasets: http://archive.ics.uci.edu/ml/datasets/Bank+Marketing#

The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution.
The classification goal is to predict if the client will subscribe a term deposit (variable y).

Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

### Cleaning and Pre-Processing

1. Drop rows containing 'unknown' values and age outliers.
2. Encoded string datas to numerical.

#### Dataframe After Cleaning and Pre-Processing

#### Dataframe After Cleaning and Pre-Processing

(gambar)

### Feature Selection


### Modelling
1. Handling Imbalance Target : SMOTE oversampling.
2. Modelling: Decision Tree Classifier, KNN Classifier, Random Forest Classifier, and Logistic Regression.
3. Hyperparameter Tuning : GridSearchCV.

Based on F1 Score evaluation, the best model is Decision Tree Classifier.

#### Before Tuning

| Recall Default   |      F1-score      |  Returned Value |
|----------|:-------------:|------:|
| 0.28 |  0.64 | 0.983 |

#### After Tuning

| Recall Default   |      F1-score      |  Returned Value |
|----------|:-------------:|------:|
| 0.28 |  0.64 | 0.983 |



### Conclusion
This machine learning helps company to reduce telemarketing costs.
The results can be improve by having more data with target = 1.
This project helps get better understanding at prediction machine learning using classification algorithms.

### Business Insights:

- The company should add interest about 2%.
- The company needs to upgrade the loan market in Province D, F, L because they produce a high amount of loan.
- The company also needs to expand the market to Province G because there are almost no default customer provinces and a big ratio of no default customers.
- On Province J, they need to campaign to people who older than 45 and/or has typical for contract type A or history type A
- Start Massive Campaign on Province N

### Dashboard
Credits: Colorlib.com

#### Home
This page is to fill features for predicting Loan status. There is 9 features which is, family size, contract type, gender, province, age, group history type, monthly expense, and loan amount.

(gambar)

#### Prediction
This page tells the result of the input that we give at the Home page.

(gambar)

#### Data
This page shows some datas that I have cleaned and prepared for modelling.

(gambar)

#### Plot
This page shows some plots. There are barplot for user status in each Province, heatmap of loan amount of each Province, histogram of customer's age and loan amounts.

(gambar)

#### Author
This page tells you more about me.

(gambar)

##### Thank you for reading.

