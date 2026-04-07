# binary-classification-loan-prediction

## Project Overview
Automating the home loan eligibility process for **XYZ Company**. This classification model predicts if a loan will be approved ('Y') or rejected ('N') based on user-provided demographics and financial data.

## Dataset
- **Training Data**: 614 observations across 13 features.
- **Target Variable**: `Loan_Status` (approx. 69% approved).
- **Key Features**: Gender, Marital Status, Education, Dependents, Income, Loan Amount, and Credit History.

## Technical Approach
1. **Data Preprocessing**: 
   - Handled missing values using **Median** (numerical) and **Mode** (categorical).
   - Normalized skewed data (Income/Loan Amount) using **Log Transformations**.
2. **Feature Engineering**: Created `Total_Income`, `EMI`, and `Balance_Income` to better reflect repayment capacity.
3. **Model Selection**: 
   - **Logistic Regression**: Baseline model for binary outcomes.
   - **Random Forest**: Ensemble method to improve predictive power.
4. **Evaluation**: Assessed via **Accuracy**, **Precision**, **Recall (Sensitivity)**, and **ROC/AUC** curves.

## Results
- **Logistic Regression Accuracy**: ~80.8%
- **Random Forest Accuracy**: ~78.6%
