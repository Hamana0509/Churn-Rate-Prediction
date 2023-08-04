# Churn Rate Prediction
## Introduction
Churn rate is the percentage of subscribers to a service that discontinue their subscription to that service in a given time period. It is a possible indicator of customer dissatisfaction, cheaper and/or better offers from the competition, more successful sales and/or marketing by the competition, or reasons having to do with the customer life cycle. In this project, we will use the data from a telecom company to predict the churn rate of its customers.
## Data Description
- The data is from Kaggle: https://www.kaggle.com/datasets/imsparsh/churn-risk-rate-hackerearth-ml
- The data includes 36992 rows, 21 columns, and 1 target variable. The target variable is `churn_risk_score`, which is a categorical variable with 5 levels. The other 20 columns are features, including 3 numerical variables and 17 categorical variables.
- The data is imbalanced. The churn rate is 4.2%.
## Data Preprocessing
### Missing Values
- There are 3 numerical variables and 17 categorical variables. The missing values are filled with the mode of the categorical variables and the mean of the numerical variables.
### Outliers
- The outliers are removed by using the Robust Scaler.
### Imbalanced Data
- The imbalanced data is handled by using the SMOTE method.
### Feature Engineering
The feature engineering includes:
    - Feature extraction
    - Encoding the categorical variables
    - Feature selection
    - Feature scaling
## Model Building
### Model Selection
- The models used in this project are:
    - SVM
    - Decision Tree
    - Random Forest
    - XGBoost
    - CatBoost
- The model selection is based on the recall score.
### Model Evaluation
The evaluation metrics are:
    - Accuracy
    - Precision
    - Recall
    - F1 score
    - Confusion Matrix
### Model Tuning
- The hyperparameter are tuned by using the GridSearchCV method.