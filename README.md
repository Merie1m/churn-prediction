# Churn Prediction — Streaming Platform

A machine learning project to predict which streaming subscribers are likely 
to cancel, so the marketing team can reach out before they leave.

---

## The Problem

A streaming platform loses 26% of its subscribers every quarter.
Retaining an existing customer is far cheaper than acquiring a new one,
so we built a model to flag at-risk customers early.

---

## Dataset

IBM Telco Customer Churn — https://www.kaggle.com/datasets/blastchar/telco-customer-churn
7043 customers, 21 features, 26.5% churn rate.
Variables were renamed to fit a streaming context.

---

## Methodology

This project follows the CRISP-DM framework across 6 phases:
Business Understanding → Data Understanding → Data Preparation
→ Modeling → Evaluation → Deployment

---

## Stack

Python, pandas, matplotlib, seaborn, scikit-learn, XGBoost, SHAP, imbalanced-learn, Power BI

---

## Repo Structure

data/raw                         → original IBM Telco dataset
data/processed                   → cleaned data, train/test splits
notebooks/01_EDA.ipynb           → exploration and visualization
notebooks/02_Preprocessing.ipynb → cleaning, encoding, SMOTE
notebooks/03_Modeling.ipynb      → model training and evaluation
outputs/models                   → saved XGBoost model
outputs/predictions              → predictions_churn.csv
dashboard                        → Power BI files
report/rapport_crisp_dm.pdf      → full CRISP-DM report

---

## Quickstart

git clone https://github.com/Merie1m/churn-prediction.git
pip install pandas matplotlib seaborn scikit-learn xgboost imbalanced-learn shap jupyter
jupyter notebook

Run notebooks in order: 01 → 02 → 03

---

## Results

Logistic Regression  →  AUC-ROC: 0.8093
Random Forest        →  AUC-ROC: 0.8170
XGBoost (final)      →  AUC-ROC: 0.8177

Out of 1409 test customers:
High risk   → 283 customers
Medium risk → 282 customers
Low risk    → 844 customers

---

## Key Findings

Customers on month-to-month contracts churn at 42.7%
Fiber optic users churn at 41.9%
Most churners leave within the first 10 months
Monthly charges is the strongest predictor

---

## Team

Toumi Meriem      →  Data Scientist / Analyst / Engineer  →  EDA, Preprocessing, Modelisation, Git
Ben Chaaben Eya   →  Data Analyst / BI Developer          →  Dashboard Power BI, Visualisations
Bejaoui Hadil     →  Project Manager                      →  Rapport CRISP-DM, Backlog Jira
Khouili Ghofrane  →  Data Engineer                        →  Pipeline, README, Slides soutenance
