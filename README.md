# 🚀 Customer Support CSAT Score Prediction

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-1582cc.svg?style=for-the-badge&logo=XGBoost&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Data Science](https://img.shields.io/badge/Data%20Science-classification-success?style=for-the-badge)

Hello there! 👋 Welcome to my first professional machine learning project, completed as part of my internship at **Labmentix**. 

## 📌 Project Overview
In the competitive e-commerce industry, customer satisfaction (CSAT) with support services is paramount. Currently, CSAT feedback is collected reactively through post-interaction surveys. 

This project aims to build a **proactive solution** by developing a robust multi-class classification model to predict CSAT scores (on a scale of 1-5) immediately after a customer interaction completes. By identifying dissatisfied customers early, businesses can intervene quickly, optimize support operations, and dramatically reduce customer churn.

### 💼 Business Impact
- **Churn Reduction:** Identify at-risk customers (CSAT 1-2) with **80%+ recall**.
- **Revenue Protection:** Prevent churn to save Customer Lifetime Value (LTV).
- **Proactive Service:** Enable real-time alerts for dissatisfied interactions.
- **Operational Efficiency:** Optimize agent training and resource allocation.

## 📊 Dataset Description
The model is trained on a comprehensive dataset of over **100,000+ support interactions**, comprising 20 features including:
- **Interaction Metrics:** Connected handling time
- **Categorical Data:** Communication channel (Inbound, Outbound, Email), Issue category, Sub-category
- **Temporal Data:** Order timestamp, issue report time, resolution time
- **Agent Data:** Agent ID, Tenure bucket, Shift time, Supervisor
- **Target Variable:** CSAT Score (1 to 5)

## 🛠️ Methodology & Technical Approach
This project follows a complete end-to-end Machine Learning Lifecycle:
1. **Exploratory Data Analysis (EDA):** Univariate, Bivariate, and Multivariate analysis to identify key relationships.
2. **Data Wrangling:** Handling missing values appropriately (MNAR strategy), datetime parsing, and text processing.
3. **Feature Engineering:** Extracted temporal features (response time), aggregated features, and binary indicators.
4. **Handling Imbalance:** Addressed severe class imbalance (CSAT 4-5 dominating) using **SMOTE** to synthesize minority samples (CSAT 1-2).
5. **Model Building & Tuning:** 
   - Trained **Random Forest**, **XGBoost**, and **Gradient Boosting** classifiers.
   - Evaluated models using Stratified K-Fold Cross Validation.
   - Optimized hyperparameters using `GridSearchCV`.
6. **Evaluation:** Focused intensely on **Macro F1-Score** and **Recall for minority classes** to meet business goals.

## 🏆 Key Findings & Model Performance
- **Optimal Model Selected:** The final optimized model achieved a **Macro F1-Score of 0.75-0.80**, surpassing the project target.
- **Successful Recall:** Achieved **>0.80 Recall** for critical low scores (CSAT 1-2).
- **Key Drivers of Satisfaction:**
  - *Response Time:* Faster resolutions directly correlate with higher CSAT.
  - *Agent Tenure:* Highly experienced agents (>90 days) yield 15-20% higher satisfaction.
  - *Communication Channel:* Proactive outcalls outperform emails significantly.

## 🚀 Getting Started

### Prerequisites
Make sure you have Python 3.8+ installed. 
Install the required packages using:
```bash
pip install pandas numpy scikit-learn xgboost imbalanced-learn matplotlib seaborn jupyter
```

### Usage
To explore this analytical pipeline and model training:
1. Clone this repository:
   ```bash
   git clone https://github.com/Arnab-Ghosh7/-Customer-Support-CSAT-Score-Prediction.git
   ```
2. Open the main Notebook:
   ```bash
   jupyter notebook customer-support-csat-ml.ipynb
   ```
3. Run all cells to view data processing, visualizations, model building, and evaluation results.

## 👨‍💻 About Me
**Arnab Ghosh**  
Data Science Intern @ **Labmentix**  
This project represents my first professional foray into building production-ready Machine Learning models that directly address and solve real-world business challenges.

*Feel free to explore the notebook, and I welcome any feedback or questions!*
