# customer-churn-modeling
A machine learning project to predict customer churn using classification models. Includes EDA, model building, and performance evaluation.
# 📂 RBC Customer Churn Modeling – SAS Enterprise Miner

## 📝 Overview  
This project was completed as part of the BA706 course and aimed to predict customer churn for RBC using data-driven techniques in **SAS Enterprise Miner**. The analysis used a structured approach to build predictive models that help understand the key factors influencing churn.

## 📊 Dataset  
- **Source:** [Kaggle - RBC Churn Dataset](https://www.kaggle.com/datasets/saadsalim997/rbcchurndataset)  
- **Records:** 160,000  
- **Variables:** Customer demographics, behavioral metrics, and account details  
- **Target Variable:** `Exited` (1 = customer churned, 0 = retained)

## 🔍 Techniques Used  
- **Data Preparation:**  
  - Handling skewness using log and cap-floor transformations  
  - Feature engineering (e.g., HasBalance, HasProducts)  
  - Partitioning into 50% training and 50% validation sets  

- **Model Development:**  
  - **Decision Tree Models** (Assessment, Maximal, ASE Tree)  
  - **Regression Models** (Full, Backward, Forward, Stepwise)  
  - **Neural Networks** with tuning across hidden units (2H–8H)  

## 📈 Best Model Performance  
- **Neural Network (Cap & Floor, 4 Hidden Units):**  
  - **ASE:** 0.115123  
  - **ROC:** 0.833  
  - Best balance of complexity and accuracy

## ✅ Key Findings  
- **Top Predictors:**  
  - Age  
  - IsActiveMember  
  - HasProducts  
  - Geography (Germany had higher churn)  
  - Gender (Females were more likely to churn)

- **Overall Churn Rate:** 20.37%  
- Inactive members, customers with fewer products, and those in certain regions showed higher churn likelihood.

## 📌 Tools & Environment  
- **Tool:** SAS Enterprise Miner  
- **Environment:** Academic Lab  
- **Team Project:** Completed with 3 group members; this file summarizes my personal contributions and model evaluations.

## 💡 Business Recommendations  
- Launch gender-specific and age-based retention strategies  
- Use product bundling to reduce churn among single-product users  
- Integrate neural network scoring into real-time CRM systems for proactive retention

