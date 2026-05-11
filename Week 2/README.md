# 📉 Linear Regression: Predictors of Anxiety (GAD-7)

## Dataset Used : Anxiety & Depression Mental Health Factors Dataset📝

## 📌 Project Context
This analysis is part of the **DS-1 Week 2** curriculum, focusing on **Ordinary Least Squares (OLS) Regression**. We are utilizing the **Anxiety & Depression Mental Health Factors Dataset📝** to investigate the relationship between individual circumstances and psychological outcomes.

## 🔍 Research Question
> *"Can demographic profiles and life stressors (Work & Finance) reliably predict a participant's score on the GAD-7 anxiety scale?"*

## 🛠 Model Specification
The model was constructed using the following parameters:
- **Dependent Variable:** `Anxiety_Score` (Continuous, 0-21)
- **Independent Variables:** - *Demographics:* Age, Gender, Education, Employment.
    - *Life Events:* Financial Stress (1-10), Work Stress (1-10).

## 📊 Methodology & Workflow
1. **Dummy Encoding:** Categorical data was transformed into indicator variables to allow for linear computation.
2. **OLS Fitting:** The model was fitted using the `statsmodels` library.
3. **Residual Diagnostics:** - Verified **Homoscedasticity** via Residuals vs. Fitted plots.
    - Verified **Normality** via Q-Q plots.
    - Checked **Multicollinearity** using Variance Inflation Factor (VIF).

## 💡 Results Summary
- **R-squared:** ~0.005 (The model explains 0.5% of the variance).
- **Key Finding:** Demographics and general life stressors were found to be weak predictors of GAD-7 scores in this sample.
- **Diagnostics:** The **Durbin-Watson** score of ~1.95 indicates that the residuals are independent and the model is not suffering from autocorrelation.

---
*Note: This folder contains the `anxiety_depression_data.csv` subset and the corresponding analysis scripts.*
