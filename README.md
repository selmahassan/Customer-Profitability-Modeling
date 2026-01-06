# Customer Profitability Segmentation Modeling

## Overview

This project explores how a financial institution could identify and understand **customer profitability** using demographic, credit, and transaction-level data. The goal is to simulate a real-world **finance data science workflow**—from messy raw data to modeling insights that could inform marketing, credit strategy, or customer segmentation decisions.

The analysis focuses on predicting whether a customer falls into a **Low, Medium, or High profitability class** based on their financial behavior and characteristics.

---

## Project Objectives

* Perform exploratory data analysis (EDA) on multi-source financial data
* Engineer meaningful features related to credit behavior and transactions
* Build and evaluate machine learning models to predict customer profitability
* Interpret model outputs in a **business-relevant, finance-focused** way

---

## Data Description

The data used in this project was sourced from the "Financial Transactions Dataset: Analytics" on Kaggle and can be found here: https://www.kaggle.com/datasets/computingvictor/transactions-fraud-datasets

The project uses multiple datasets that simulate realistic financial data commonly found at banks or credit card companies, including:

* **Customer Demographics**: Age, income, geographic location
* **Credit Information**: Credit score, debt, card type, card brand
* **Transaction Data**: Transaction amounts, usage frequency, chip usage

These datasets were merged and cleaned to create a unified modeling table.

---

## Exploratory Data Analysis (EDA)

Key EDA steps included:

* Distribution analysis of credit scores and income
* Geographic visualization of customers using latitude and longitude
* Comparison of transaction behavior across card brands (e.g., Visa, Amex)
* Analysis of transaction volume and usage patterns by profitability class

EDA was used not only to understand the data, but also to guide **feature engineering and modeling decisions**.

---

## Feature Engineering

Examples of engineered features include:

* Aggregated transaction behavior metrics
* Combined demographic and financial attributes
*  Encoded card brand and card type
* Indicators for chip usage


The final feature set reflects a mix of **behavioral, financial, and demographic signals**, similar to what would be available in a real finance analytics environment.

---

## Modeling Approach

The target variable is **Profitability Class** (Low, Medium, High), treated as a multi-class classification problem.

Models explored:

* **Decision Tree Classifier**
* **Random Forest Classifier**

Tree-based models were chosen for their:

* Interpretability
* Ability to handle non-linear relationships
* Suitability for tabular financial data

The dataset was split into training and validation sets to evaluate model performance.

---

## Model Evaluation

Models were evaluated using:

* Accuracy
* Confusion matrices
* Precision, recall, and F1-score (classification report)

Special attention was given to:

* Misclassification between Medium and High profitability customers
* The trade-off between identifying high-value customers and overall accuracy

---

## Key Findings

* Behavioral transaction metrics provide a strong signal for customer value segmentation.
* High-profit customers can be reliably identified with minimal false positives.
* Most classification uncertainty arises among mid-tier customers near profitability thresholds.
* The Random Forest model reduces severe misclassifications (e.g., Low predicted as High), making it more robust for real-world finance applications.

These insights align with real-world expectations in consumer finance and credit analytics.

---

## Future Improvements

Potential next steps to improve this analysis include:

* Treating profitability as an **ordinal** or regression-based target
* Trying gradient boosting models (XGBoost, LightGBM)
* Engineering time-based transaction features
* Addressing potential class imbalance
* Adding explainability tools such as SHAP values

---

## Tools & Technologies

* Python
* pandas, NumPy
* matplotlib, seaborn
* scikit-learn
* Jupyter Notebook

---

## Why This Project Matters

This project demonstrates:

* End-to-end data science thinking
* Experience with realistic financial datasets
* Ability to translate technical results into business insights
* Strong alignment with roles in **finance, fintech, and credit analytics**

---

## Author

**Selma Hassan**
Data Science graduate with a computer science concentration, interested in data science applications in finance and consumer analytics.
