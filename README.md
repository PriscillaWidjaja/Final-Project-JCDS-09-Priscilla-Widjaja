# Final Project JCDS 09 - Priscilla Widjaja

### Deposit Term Subscription Prediction Machine Learning




A prediction machine learning project using classification algorithm that predicts whether the client will subscribe a term deposit or not.

### Datasets

http://archive.ics.uci.edu/ml/datasets/Bank+Marketing#

The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution.

The classification goal is to predict if the client will subscribe a term deposit (variable y).


### Cleaning and Pre-Processing

1. Drop rows containing 'unknown' values and age outliers.
2. Encoded string datas to numerical.

#### Dataframe Before Cleaning and Pre-Processing

#### Dataframe After Cleaning and Pre-Processing

(gambar)

### Feature Selection


### Modeling
1. Handling Imbalance Target : SMOTE oversampling.
2. Modeling: Decision Tree Classifier, KNN Classifier, Random Forest Classifier, and Logistic Regression.

|      Before Hyperparameter Tuning     |  After Hyperparameter Tuning  |
|:-:|:--:|
|  0.64 | 0.983 |

Based on F1 Score evaluation, the best model is Decision Tree Classifier.

3. Hyperparameter Tuning : GridSearchCV.

|      Before Hyperparameter Tuning     |  After Hyperparameter Tuning  |
|:-:|:--:|
|  0.64 | 0.983 |

### Conclusion
This machine learning helps company to reduce telemarketing costs by eliminating customers who aren't going to subscribe.

The results can be improve by having more data with target = 1.

This project helps get better understanding at prediction machine learning using classification algorithms.


### Business Insights:

- The company should create marketing campaign targeted to bank clients who are older than 38 years old.
- The company needs to create products which will attract bank clients who are self-employed, unemployed, entrepreneurs dan housemaids.

### Dashboard
Credits: Colorlib.com

#### Home

(gambar)

#### Data

(gambar)

#### Plot

(gambar)

#### Prediction

(gambar)

#### Results

(gambar)

##### Thank you for reading.
