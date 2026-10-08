# ProHR – AI-Based Employee Attrition Prediction

ProHR is an AI/ML-powered HR analytics dashboard designed to predict employee attrition risk and provide interpretable insights into the factors contributing to employee turnover.

The system combines machine learning-based prediction, employee risk classification, HR analytics, and explainable AI to support data-driven employee retention decisions.

## 🚀 Live Demo

🔗 **[View ProHR Live](https://hr-ml-prediction-1rsm.vercel.app/)**

## 📌 Overview

Employee attrition can increase recruitment costs, reduce productivity, and affect team stability.

ProHR helps HR teams identify employees who may be at higher risk of leaving and understand the key factors associated with that risk.

The system categorizes employees into:

- 🔴 High Risk
- 🟡 Medium Risk
- 🟢 Low Risk

and provides corresponding HR insights to support retention planning.

## ✨ Key Features

- 📊 Interactive HR analytics dashboard
- 🧠 Employee attrition prediction
- 🤖 Multiple machine learning models
- ⚖️ Class imbalance handling using SMOTE
- 🔍 Explainable AI using SHAP
- 🚦 High / Medium / Low employee risk classification
- 📈 Interactive data visualizations
- 👥 Employee-level analysis
- 📋 Department and workforce analytics
- 💡 HR action recommendations based on risk factors

## 🧠 Machine Learning

Multiple classification models are evaluated for employee attrition prediction:

- Logistic Regression
- Random Forest
- XGBoost

The models are evaluated using classification metrics including:

- F1-Score
- ROC-AUC

### Handling Class Imbalance

Employee attrition datasets can contain significantly fewer attrition cases compared to non-attrition cases.

**SMOTE (Synthetic Minority Over-sampling Technique)** is used to address class imbalance and improve the model's ability to identify employees at risk of attrition.

## 🔍 Explainable AI with SHAP

ProHR uses **SHAP (SHapley Additive exPlanations)** to interpret machine learning predictions.

This helps identify the factors that have the greatest influence on employee attrition risk.

Examples include:

- Overtime
- Salary
- Job Satisfaction
- Job-related factors
- Employee characteristics

Instead of only providing a prediction, ProHR helps explain **why an employee may be at risk**.

## 🏗️ Project Structure

```text
HR-ML-Prediction/
│
├── backend/
│   ├── ML models
│   ├── API services
│   └── backend logic
│
├── public/
│
├── src/
│   ├── components/
│   │   ├── AnalyticsTab.js
│   │   ├── DashboardTab.js
│   │   ├── PredictionsTab.js
│   │   └── Toast.js
│   │
│   ├── App.js
│   └── application logic
│
├── employee1.ods
├── employee12.csv
├── package.json
├── package-lock.json
└── README.md
