# Credit_Card_fraud_detection

## 1. Background and Overview of the Dataset
In recent years, the prevalence of credit card fraud has increased significantly, necessitating the development of robust detection systems. This project utilizes the Credit Card Fraud Detection dataset obtained from Kaggle, which contains transactions made by European cardholders in September 2013. The dataset consists of 284,807 transactions, with only 492 being fraudulent, indicating a significant class imbalance. The dataset includes 30 anonymized features (V1 to V28, Time, and Amount) derived from PCA (Principal Component Analysis) transformation, ensuring the confidentiality of the cardholders' information.

You can find the data set [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## 2. Data Structure Overview
The dataset comprises:

Features (V1 to V28): These are numerical variables resulting from PCA transformation, capturing various attributes of the transactions.

Time: This represents the time elapsed since the first transaction, measured in seconds.

Amount: The monetary value of the transaction.

Class: The target variable where 1 represents fraudulent transactions and 0 indicates legitimate transactions.

#### Data Summary:

Total Transactions: 284,807

Legitimate Transactions: 284,315

Fraudulent Transactions: 492

## 3. Executive Summary
This project employs a Logistic Regression model to detect fraudulent transactions with a focus on achieving high accuracy despite the significant class imbalance in the dataset. The model was trained on a balanced dataset, created by undersampling legitimate transactions to match the number of fraudulent transactions. After training, the model achieved an accuracy score of approximately 92.39% on the test dataset, demonstrating its efficacy in detecting fraud.

## 4. Insights Deep Dive

#### Transaction Amount Analysis: 
The average amount for legitimate transactions is significantly lower (around $88.29) compared to fraudulent transactions (around $122.21). This discrepancy highlights that higher transaction amounts may be indicative of fraud.

#### Model Performance: 
The model achieved a precision of 0.94 for fraudulent transactions and a recall of 0.92, indicating that it effectively identifies fraud without misclassifying too many legitimate transactions.

#### Balanced Class Performance: 
Both precision and recall scores for legitimate and fraudulent transactions were high, suggesting that the model performs well across both classes.

## 5. Recommendations

#### Model Enhancement: 
Further experimentation with different algorithms (such as Random Forest, XGBoost, or neural networks) could improve detection rates and reduce false positives.

#### Feature Engineering: 
Investigate additional features or transformations that might help the model capture the characteristics of fraudulent transactions more effectively.

#### Real-Time Monitoring: 
Implementing this model in a real-time monitoring system could help organizations promptly identify and respond to potentially fraudulent activities.

#### Further Research: 
Explore advanced techniques like ensemble methods or anomaly detection approaches to enhance the detection capabilities in future iterations of this project.
