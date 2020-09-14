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

![Corr](/Images/Corr.png)

2. Choosing Top 10 features to use.

![FeatureSelection](/Images/FeatureSelection.png)

### Handling Imbalance Target

| y | Data (%) |
|:-|:-:|
| No | 87.75 |
| Yes | 12.25 |

The target was imbalance. So SMOTE Oversampling technique was used to balance the target.

### Modelling & Hyperparameter Tuning

Using GridSearchCV to choose the best parameters.

#### F1 Score Before & After Hyperparameter Tuning

|           |  Before  | After |
|:-|:-:|:-:|
| Logistic Regression | 41.909023 | 40.391335 |
| Decision Tree | 32.446134 | 46.787879 |
| Random Forest | 40.638607 | 42.477876 |
| KNN Classifier | 37.958533 | 46.511628 |

Based on F1 Score, the best model is Decision Tree Classifier.

#### Confusion Matrix Decision Tree Classifier

##### Before Hyperparameter Tuning

![Before](/Images/Before.png)

##### After Hyperparameter Tuning

![After](/Images/After.png)

### Conclusions:
- This machine learning helps company to reduce telemarketing costs by eliminating customers who aren't going to subscribe.
- The results can be improved by having more datas of bank clients who susbcribed.


### Business Insights:

- The company should create marketing campaign targeted to bank clients who are older than 38 years old.
- The company needs to create products which will attract bank clients who are self-employed, unemployed, entrepreneurs dan housemaids.

### Dashboard

#### Home

![Home](/Images/Home.png)

#### Dataset

![Dataset](/Images/Dataset.png)

#### Plot

![Plot](/Images/Visualization.png)

#### Prediction

![Prediction](/Images/Prediction.png)

#### Result

![Result](/Images/Result.png)

##### Thank you for reading.
