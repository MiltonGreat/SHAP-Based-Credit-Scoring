# SHAP-Based Credit Scoring

![screenshot-localhost_8888-2025 04 03-09_27_06](https://github.com/user-attachments/assets/0233e718-b58a-43b5-ba2c-1dad654bf1f1)

### Project Overview

This project develops a machine learning model to predict the probability of loan default using the Home Credit dataset. It focuses on:

- Risk Prediction: Probability of Default (PD), Loss Given Default (LGD), and Exposure at Default (EAD).
- Explainability: Uses SHAP (SHapley Additive exPlanations) to interpret model decisions.
- Actionable Insights: Identifies key risk drivers for loan approvals/denials.

### Dataset

The dataset contains financial and demographic information related to credit applicants. The key features used in this model include:

- Credit History – Previous loan repayment behavior.
- Purpose – The reason for applying for credit.
- Savings – Amount of savings available.
- Amount – Loan amount requested.
- Duration – Loan repayment period.

The target variable is Credit Risk (Good/Bad Credit), where 1 represents bad credit and 0 represents good credit.

### Key Findings

**Top Risk Drivers**
1. EXT_SOURCE_3	(0.41) External credit score (most important)
2. EXT_SOURCE_2	(0.36) Secondary financial stability metric
3. AMT_GOODS_PRICE (0.26) Higher loan amounts increase risk
4. AMT_CREDIT	(0.19) Total credit granted

**Model Performance**

- PD Model (AUC-PR 0.78)
- LGD Model (R-squared -0.08)
- EAD Model (R-squared 0.59)
- 
### Conclusion

This project demonstrated that transparent, explainable credit risk modeling is achievable using SHAP values, with external data sources (EXT_SOURCE) being the strongest predictors.

### Source

![Home Credit Default Risk Dataset from Kaggle](https://www.kaggle.com/datasets/anggundwilestari/home-credit)
