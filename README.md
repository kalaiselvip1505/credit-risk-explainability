# credit-risk-explainability
Credit Risk Model with SHAP, LIME, and XGBoost - Explainable AI Project
## 🎯 Objective

The primary objective of this project is to build a transparent, explainable,
and trustworthy Credit Risk Prediction model using advanced Explainable AI (XAI)
techniques. Traditional machine learning models such as XGBoost provide strong
predictive accuracy but function as “black-box” models. 

This project aims to:
- Build a high-performance XGBoost model for loan default prediction  
- Explain global feature importance using SHAP  
- Provide human-understandable, local explanations using LIME  
- Detect borderline (uncertain) applicants  
- Automatically generate a complete report for business stakeholders  
- Ensure the model is interpretable, fair, and deployment-ready  
## 📌 Summary

This project implements a complete end-to-end Machine Learning pipeline for 
Credit Risk Prediction using XGBoost combined with Explainable AI (XAI) methods.

### 🔄 1. Data Processing
The raw loan dataset undergoes thorough preprocessing:
- Handling missing values
- Encoding categorical features
- Normalizing and scaling numerical variables
- Balancing default vs non-default data (if required)
- Creating engineered features such as debt ratio, payment behaviour, etc.

This ensures the data is clean, structured, and model-ready.

### ⚙️ 2. Model Training (XGBoost)
A high-performance XGBoost classifier is trained to predict whether a loan 
applicant is likely to default. XGBoost is chosen because of:
- Excellent accuracy  
- Ability to handle nonlinear patterns  
- Robustness to noisy financial data  
- Fast training performance  

Hyperparameters are tuned for optimal model performance.

### 📊 3. Model Evaluation
The trained model is evaluated using:
- Accuracy  
- Precision, Recall  
- F1-Score  
- ROC–AUC score  
- Confusion Matrix  

This provides a clear understanding of model effectiveness in distinguishing
default vs non-default applicants.

### 🧠 4. Explainability & Interpretability
To avoid “black-box” predictions, modern XAI tools are used:

#### ✅ SHAP (Global + Local)
- SHAP Summary Plot shows overall feature importance  
- SHAP Bar Plot ranks top contributors  
- SHAP Force/Decision plots explain individual predictions  

#### ✅ LIME (Local Interpretation)
- Generates human-readable explanations for single loan applicants  
- Highlights what features pushed the model toward default / non-default  

#### ⚠️ Borderline Applicant Detection
Cases with prediction probability near **0.5** are identified as high-risk/uncertain 
loan applicants requiring manual review.

### 📝 5. Automated Reporting
A structured Markdown + PDF report is generated containing:
- Plots  
- Feature importance  
- SHAP & LIME explanations  
- Borderline analysis  
- Model summary  

---

This project is useful for:
- Banks / Financial Institutions  
- Credit Risk Analysts  
- Fraud & Risk Management Teams
- ## 📦 Requirements

This project requires the following Python libraries:

- python 3.9+
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- xgboost
- shap
- lime
- reportlab
- jinja2
- tqdm

Install everything using:

```bash
pip install -r requirements.txt
numpy
pandas
matplotlib
scikit-learn
seaborn
xgboost
shap
lime
reportlab
tqdm
jinja2

- Students and Researchers studying Explainable AI  
