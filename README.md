# Final Project JCDS 09 - Priscilla Widjaja

### Deposit Term Subscription Prediction Machine Learning

A prediction machine learning project using classification algorithm that predicts whether the client will subscribe a term deposit or not.

### Datasets

http://archive.ics.uci.edu/ml/datasets/Bank+Marketing#

The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution.

The classification goal is to predict if the client will subscribe a term deposit (variable y).


### Cleaning and Pre-Processing

1. Drop rows containing 'unknown' values and age outliers.
2. Encode string datas to numerical.
3. Scale datas using RobustScaler.

### Feature Selection

1. Drop columns that has strong correlations with each other.

![Corr](Corr.png)

2. Choosing Top 10 features to use.

![FeatureSelection](FeatureSelection.png)

### Handling Imbalance Target

| y | Data (%) |
|:-|:-:|
| No | 87.75 |
| Yes | 12.25 |

The target was imbalance. So SMOTE Oversampling technique was used to balance the target.

### Modeling

|           |  F1 Score  |
|:-|:-:|
| Logistic Regression | 41.909023 |
| Decision Tree Classifier | 32.397959 |
| Random Forest Classifier | 41.319943 |
| KNeighborsClassifier | 37.958533 |

### Hyperparameter Tuning

Using GridSearchCV to choose the best parameters.

#### F1 Score Before & After Hyperparameter Tuning

|           |  Before  | After |
|:-|:-:|:-:|
| Logistic Regression | 41.909023 | 41.784387 |
| Decision Tree | 32.397959 | 46.731235 |
| Random Forest | 41.319943 | 40.419162 |
|  KNN Classifier | 37.958533 | 0.983 |

Based on F1 Score evaluation, the best model is Decision Tree Classifier.

### Conclusion
This machine learning helps company to reduce telemarketing costs by eliminating customers who aren't going to subscribe.

The results can be improve by having more data with target = 1.

This project helps get better understanding at prediction machine learning using classification algorithms.


### Business Insights:

- The company should create marketing campaign targeted to bank clients who are older than 38 years old.
- The company needs to create products which will attract bank clients who are self-employed, unemployed, entrepreneurs dan housemaids.

### Dashboard

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
