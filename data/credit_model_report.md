# 📘 Credit Risk Model Explanation Report

Generated on: **2025-11-18 16:43:21**


## 1. 📊 Dataset Summary

- Total training samples: **400**

- Total test samples: **100**

- Total features: **10**


### Feature List:

- loan_amnt

- annual_income

- dti

- credit_score

- employment_length

- num_open_accounts

- recent_missed_payments

- purpose_debt_consolidation

- purpose_home

- purpose_small_business


---

## 2. 🎯 Model Performance

- Accuracy: **0.7700**

- ROC-AUC: **0.5100**


### Classification Report:

```

              precision    recall  f1-score   support

           0       0.79      0.96      0.87        80
           1       0.00      0.00      0.00        20

    accuracy                           0.77       100
   macro avg       0.40      0.48      0.44       100
weighted avg       0.64      0.77      0.70       100

```


---

## 3. 🔍 SHAP Global Feature Importance

Top important features:

- **dti** → 0.62984

- **employment_length** → 0.51796

- **credit_score** → 0.42778

- **num_open_accounts** → 0.38722

- **loan_amnt** → 0.38648

- **annual_income** → 0.34900

- **recent_missed_payments** → 0.19246

- **purpose_home** → 0.11001

- **purpose_small_business** → 0.10024

- **purpose_debt_consolidation** → 0.06596


(See shap_importance.csv for full ranking.)


---

## 4. ⚠️ Borderline Risk Cases (Closest to 0.5 Probability)

### Case 456

- Probability: **0.4952**

- True Label: **0**

- Distance from 0.5: **0.00478**


### Case 228

- Probability: **0.5054**

- True Label: **0**

- Distance from 0.5: **0.00544**


### Case 342

- Probability: **0.4908**

- True Label: **1**

- Distance from 0.5: **0.00915**


### Case 70

- Probability: **0.4099**

- True Label: **1**

- Distance from 0.5: **0.09015**


### Case 317

- Probability: **0.3643**

- True Label: **0**

- Distance from 0.5: **0.13570**



---

## 5. 📌 SHAP Feature Stability (Bootstrap)

Top features across bootstrap runs:

### Run 1

- dti

- annual_income

- credit_score

- loan_amnt

- employment_length

- num_open_accounts

- recent_missed_payments

- purpose_home

- purpose_small_business

- purpose_debt_consolidation



### Run 2

- dti

- annual_income

- loan_amnt

- num_open_accounts

- credit_score

- employment_length

- recent_missed_payments

- purpose_home

- purpose_debt_consolidation

- purpose_small_business



### Run 3

- employment_length

- credit_score

- num_open_accounts

- dti

- loan_amnt

- annual_income

- recent_missed_payments

- purpose_home

- purpose_small_business

- purpose_debt_consolidation



### Run 4

- dti

- annual_income

- num_open_accounts

- loan_amnt

- employment_length

- credit_score

- recent_missed_payments

- purpose_home

- purpose_small_business

- purpose_debt_consolidation



### Run 5

- dti

- loan_amnt

- credit_score

- annual_income

- employment_length

- num_open_accounts

- recent_missed_payments

- purpose_small_business

- purpose_home

- purpose_debt_consolidation




---

## 6. 💡 LIME Explanation Summary

LIME was executed for the 5 borderline cases.

Refer to notebook output for detailed local explanations.


---
