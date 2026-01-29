🏦 Bank Customer Churn Prediction

A mini ML project to predict bank customer churn using Logistic Regression. This project uses a custom CSV dataset where age is the main factor influencing churn.

Project Overview

Customer churn is when a customer stops using a company’s services. Predicting churn helps banks take proactive actions to retain valuable customers.

In this project, I:

Created a synthetic bank dataset (bank_churn_age_based.csv)
Explored relationships between customer features and churn
Built a Logistic Regression model to predict churn
Evaluated model performance

Dataset

File: bank_churn_age_based.csv

Column Name	Description
CustomerID	Unique ID for each customer
Age	Customer’s age (main factor affecting churn)
Balance	Customer’s bank balance
Tenure_Years	Number of years with the bank
IsActiveMember	1 = Active customer, 0 = Not active
Churn	Target variable: 1 = Customer left the bank, 0 = Customer stayed

Age–Churn relation logic:
Age < 30 → low churn probability
Age 30–44 → medium churn probability
Age ≥ 45 → high churn probability

Features Used

Age

Balance

Tenure_Years

IsActiveMember

Target: Churn

Machine Learning Model

Algorithm: Logistic Regression
Reason: Logistic Regression is suitable for binary classification problems like predicting churn (Yes/No).

Steps implemented:

Load and explore dataset (pandas)
Preprocess data (handle missing values, if any)
Split data into training and testing sets
Train Logistic Regression model
Predict churn on test set
Evaluate performance using accuracy, confusion matrix, and classification report

Results

Accuracy: ~X% (replace with your result)
Confusion Matrix shows good prediction of churn for higher age groups
Logistic Regression captures age dependency effectively

Future Improvements

Include more features like transaction history, credit score, or customer complaints
Experiment with Random Forest, XGBoost or other advanced models
Deploy the model in a web app to predict churn in real-time

Files in Repo

data_bank.csv → Synthetic dataset
Bank_Customer_Churn_Prediction.py → Logistic Regression model
README.md → Project description

📌 References

Logistic Regression Documentation - scikit-learn

Synthetic dataset created for educational purposes
