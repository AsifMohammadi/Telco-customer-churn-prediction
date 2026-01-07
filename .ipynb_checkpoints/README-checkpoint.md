# Telco Customer Churn Prediction

## Overview
This project develops supervised machine learning models to predict customer churn. Churn indicates whether a customer left the telecom service or stayed.

## Dataset
- Source: Kaggle blastchar Telco dataset  
- File: Telco-Customer-Churn-Data.csv  
- Records: 7,043 customers  
- Target variable: Churn (1 = left, 0 = stayed)

## Workflow
- Loaded and inspected raw customer data using pandas  
- Cleaned hidden blanks and converted TotalCharges to numeric  
- Dropped customerID as an identifier column  
- One-hot encoded categorical features  
- Split data into training and test sets  
- Trained and evaluated:
  - Logistic Regression
  - Random Forest
  - Tuned Random Forest

## Results
- Logistic Regression ROC-AUC: 0.837  
- Basic Random Forest ROC-AUC: 0.821  
- Tuned Random Forest ROC-AUC: 0.838  
- Mean cross-validated ROC-AUC: 0.847 ± 0.012

Feature importance analysis showed that tenure, MonthlyCharges, TotalCharges, contract type, internet service type, and payment method were most associated with churn.

## How to Run
1. Clone the repository  
2. Place `Telco-Customer-Churn-Data.csv` inside the `data/` folder  
3. Open `notebooks/data-exploration.ipynb`  
4. Restart the kernel and run all cells sequentially

## Repository
URL: https://github.com/AsifMohammadi/Telco-customer-churn-prediction
