
## Overview

This project focuses on detecting fraudulent online payment transactions using Machine Learning algorithms. The model analyzes transaction details and predicts whether a transaction is fraudulent or legitimate. Multiple machine learning models are trained and evaluated to identify the best-performing fraud detection model.

## Features

- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- One-Hot Encoding for categorical features
- Fraud detection using Machine Learning
- Model comparison and evaluation
- ROC-AUC score analysis
- Confusion Matrix visualization
- Fraudulent transaction prediction

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost

## Dataset

The dataset contains transaction-related information such as:

- Transaction Type
- Transaction Amount
- Sender Balance
- Receiver Balance
- Transaction Time Step
- Fraud Label (`isFraud`)

### Target Variable

| Value | Meaning |
|---------|---------|
| 0 | Legitimate Transaction |
| 1 | Fraudulent Transaction |

## Project Workflow

### 1. Data Loading

The dataset is loaded using Pandas.

```python
data = pd.read_csv('new_file.csv')
```

### 2. Exploratory Data Analysis

- Dataset information
- Statistical summary
- Transaction type distribution
- Transaction amount analysis
- Fraud distribution analysis
- Correlation heatmap

### 3. Data Preprocessing

- One-Hot Encoding for transaction type
- Removal of unnecessary columns:
  - `nameOrig`
  - `nameDest`
  - `type`

### 4. Train-Test Split

The dataset is split into:

- Training Data: 70%
- Testing Data: 30%

### 5. Machine Learning Models

The following models are trained and compared:

- Logistic Regression
- Random Forest Classifier
- XGBoost Classifier

### 6. Model Evaluation

Models are evaluated using:

- ROC-AUC Score
- Confusion Matrix

## Results

The performance of all models is compared, and the model with the highest ROC-AUC score is selected as the final fraud detection model.

In this project, **XGBoost achieved the best performance** for detecting fraudulent transactions.

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/online-payment-fraud-detection.git
```

### Navigate to the Project Directory

```bash
cd online-payment-fraud-detection
```

### Install Required Packages

```bash
pip install -r requirements.txt
```

### Run the Project

```bash
python fraud_detection.py
```

## Project Structure

```text
Online-Payment-Fraud-Detection/
│
├── new_file.csv
├── fraud_detection.py
├── README.md
├── requirements.txt
│
└── outputs/
    ├── fraud_distribution.png
    ├── heatmap.png
    └── confusion_matrix.png
```

## Future Enhancements

- Real-time fraud detection
- Flask web application deployment
- Hyperparameter tuning
- Feature importance visualization
- Deep learning-based fraud detection
