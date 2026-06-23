# Online Payment Fraud Detection using Machine Learning

## Overview

This project uses Machine Learning techniques to identify fraudulent online payment transactions. The system analyzes transaction details and predicts whether a transaction is fraudulent or legitimate. Multiple machine learning models were trained and evaluated to determine the most effective approach for fraud detection.

## Features

* Data preprocessing and cleaning
* Exploratory Data Analysis (EDA)
* One-Hot Encoding for categorical variables
* Fraud detection using Machine Learning
* Model comparison and evaluation
* ROC-AUC score analysis
* Confusion Matrix visualization

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

## Dataset

The dataset contains transaction information such as transaction type, amount, sender balance, receiver balance, transaction step, and fraud status.

Target Variable:

* 0 → Legitimate Transaction
* 1 → Fraudulent Transaction

## Project Workflow

### Data Loading

The dataset is loaded and inspected using Pandas.

### Exploratory Data Analysis

* Dataset information and statistics
* Transaction type analysis
* Fraud distribution analysis
* Correlation heatmap visualization

### Data Preprocessing

* One-Hot Encoding for transaction types
* Removal of unnecessary columns such as `nameOrig`, `nameDest`, and `type`

### Train-Test Split

The dataset is divided into training and testing sets with a 70:30 ratio.

### Machine Learning Models

The following models were trained and compared:

* Logistic Regression
* Random Forest Classifier
* XGBoost Classifier

### Model Evaluation

Models were evaluated using:

* ROC-AUC Score
* Confusion Matrix

## Results

Among the evaluated models, XGBoost achieved the best performance in detecting fraudulent transactions due to its ability to capture complex transaction patterns and reduce overfitting.

## Project Structure

Online-Payment-Fraud-Detection/

├── new_file.csv

├── fraud_detection.py

├── README.md

└── requirements.txt

## Future Enhancements

* Real-time fraud detection
* Flask web application deployment
* Hyperparameter tuning
* Feature importance analysis
* Deep learning-based fraud detection

