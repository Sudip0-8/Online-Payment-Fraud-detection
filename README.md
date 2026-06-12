# Online Payment Fraud Detection using Machine Learning
A Machine Learning project that detects whether an online payment transaction is fraudulent or legitmate.

## Problem Statement 
Online payments are growing rapidly due to their convenience, but this has also led to a rise in fraudulent transactions. Detecting fraud automatically is critical to protect users from financial loss.

## Approach
- Performed EDA to understand transaction and class imbalance
- Applied SMOTE on training patterns and class imbalance (6.3 M non-fraud vs 8 K fraud cases)
- Trained three models - Logistic Regression, Random Forest , XGBoost
- Evaluated using Precision-Recall curve instead of just accuracy , since missing a fraud transaction is more costly than a false alarm
- Plotted feature importance to understand key fraud indicators


## Results
| Model | ROC-AUC |
|----|----|
| Logistic Regression | ~ 88% |
| Random Forest | ~ 96% |
| XGBoost | ~ 99% |

XGBoost performed best. Top features : newbalanceOrig, oldbalanceOrg , Payment

## Dataset
Download from : https://drive.google.com/file/d/133E0TDrfIjnhwRoGTw9OEozwBXUL38D8/view?usp=sharing
