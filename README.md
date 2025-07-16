#  IBM HR Analytics – Employee Attrition Prediction

---

##  Project Overview

This project analyzes employee attrition using IBM’s HR dataset to uncover key factors driving turnover and predict which employees are at risk of leaving. It includes detailed EDA, multiple feature selection techniques, machine learning models, and an interactive Power BI dashboard.

---

##  Key Features

- Exploratory Data Analysis (EDA) of employee demographics and job factors  
- Multiple feature selection methods (**SelectKBest**, **RFECV**)  
- Comparison of **Logistic Regression**, **Decision Tree**, **Random Forest**, and **Gradient Boosting**  
- Prediction of individual attrition risk scores  
- Interactive **Power BI dashboard** for clear visualization and storytelling

---

##  Dataset

The dataset contains **35 features** for **1,470 employees**, covering:

- **Demographics:** Age, Gender, Marital Status  
- **Job Factors:** Job Level, Role, Satisfaction  
- **Financial Metrics:** Monthly Income, Salary Hike  
- **Work-Life Balance:** Overtime, Work-Life Balance indicators

---

##  Models Evaluated

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------|-----------|--------|----------|
| Logistic Regression (SelectKBest) | 0.874 | 0.75 | 0.08 | 0.14 |
| Decision Tree (SelectKBest) | 0.792 | 0.18 | 0.15 | 0.16 |
| Decision Tree (RFECV) | 0.772 | 0.18 | 0.21 | 0.19 |
| Random Forest (SelectKBest) | 0.837 | 0.20 | 0.08 | 0.11 |
| Random Forest (RFECV) | 0.878 | 0.80 | 0.10 | 0.18 |
| **Gradient Boosting (RFECV)** | **0.878** | **0.58** | **0.28** | **0.38** |

 **Gradient Boosting with RFECV features delivered the best performance.**

---

##  Files Included

- `ibm_hr_dataset.py` – Main Python analysis script  
- `WA_Fn-UseC_-HR-Employee-Attrition.csv` – Original dataset  
- `model_summary.csv` – Model evaluation metrics  
- `all_employee_risks.csv` – Attrition risk scores for all employees  
- `top10_risk_new.csv` – Top 10 high-risk employees  
- `dashboard.pbix` – Power BI dashboard

---

##  Key Insights

- **Overtime**, **distance from home**, and **job satisfaction** are major drivers of attrition  
- **Younger employees** and those with **shorter tenure** are more likely to leave  
- The final model successfully identifies **high-risk employees** for proactive retention planning

---
