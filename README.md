# E-commerce Customer Churn Analysis

End-to-end churn prediction project on 5,630 e-commerce customers — from raw data to a deployable model and a live case-study site.

**[View the live site →](https://sanyagusain19.github.io/ecommerce-churn-analysis/)**

## Overview

This project identifies which customers are likely to churn on an e-commerce platform, and why — combining exploratory data analysis with a predictive model to turn raw transaction data into actionable retention strategy.

## Dataset

[Ecommerce Customer Churn Analysis and Prediction](https://www.kaggle.com/datasets/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction) by Ankit Verma, via Kaggle — 5,630 customers, 20 features including tenure, city tier, complaints, satisfaction score, and payment behavior.

## Approach

1. **Data cleaning** — handled missing values across 8 columns (4–5% missingness each)
2. **Exploratory analysis** — tested 8 variables against churn rate; identified tenure, complaints, city tier, and satisfaction score as meaningful signals
3. **Feature engineering** — one-hot encoded categorical variables, scaled numeric features
4. **Modeling** — compared 4 classifiers (Logistic Regression, SVM, Random Forest, XGBoost), optimized for recall
5. **Business recommendations** — translated findings into 5 testable retention interventions

## Key findings

- Customers in their first 3 months churn at **41.9%** — nearly 7x the rate of long-tenure customers
- A filed complaint nearly **triples** churn risk (31.7% vs 10.9%)
- Tier 3 cities churn more than Tier 1 (21.4% vs 14.5%), suggesting service/delivery gaps
- Counter-intuitively, the highest satisfaction score (5/5) had the **highest** churn rate of any group

## Model results

| Model | Accuracy | Recall | Precision |
|---|---|---|---|
| Logistic Regression | 86% | 30% | 73% |
| SVM | 85% | 59% | 59% |
| Random Forest | 95.7% | 75% | 100% |
| **XGBoost (selected)** | **97.5%** | **90%** | **95%** |

Recall was prioritized over raw accuracy — missing a churning customer is costlier to the business than a false alarm.

## Tools

Python · Pandas · Scikit-learn · XGBoost · Matplotlib · Seaborn

## Project structure

```
├── index.html          # site markup
├── style.css            # styling
├── charts.js             # Chart.js visualizations
├── reveal.js              # scroll animations
└── churn_analysis.ipynb   # full notebook: cleaning, EDA, modeling
```
---

**Sanya Gusain**
[LinkedIn]https://www.linkedin.com/in/saniya-gusain-493a2b415?utm_source=share_via&utm_content=profile&utm_medium=member_android

[GitHub](https://github.com/sanyagusain19)
