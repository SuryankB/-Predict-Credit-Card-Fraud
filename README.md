# 💳 Predict Credit Card Fraud Using Machine Learning

This project is focused on identifying fraudulent credit card transactions using advanced machine learning techniques. With the growing number of online transactions, credit card fraud is becoming increasingly prevalent, making fraud detection systems crucial for financial institutions. This project uses a highly imbalanced dataset to develop and evaluate various classification models to effectively detect fraud with minimal false alarms.

---

## 🧠 Project Objective

The main goals of this project are:

- To build a machine learning model that can accurately classify transactions as fraudulent or legitimate.
- To tackle **class imbalance**, which is a major challenge in fraud detection.
- To compare the performance of different classification algorithms.
- To apply data visualization and feature engineering techniques for improved accuracy.
- To reduce **false negatives** (missed frauds) while keeping **false positives** (legit transactions flagged as fraud) low.

---

## 📦 Dataset Overview

- **Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Records:** 284,807 transactions
- **Fraudulent Cases:** 492 (approx. 0.17% of data)
- **Features:**
  - V1 to V28: PCA-transformed numerical variables (confidential for security)
  - Time: Seconds elapsed between transactions
  - Amount: Transaction amount
  - Class: Target variable (0 = legitimate, 1 = fraud)

---

## 🧰 Tools & Technologies

- **Languages:** Python 3.x
- **Libraries:**
  - Data Analysis: `pandas`, `numpy`
  - Visualization: `matplotlib`, `seaborn`, `plotly`
  - Modeling: `scikit-learn`, `xgboost`, `lightgbm`
  - Imbalanced Data: `imbalanced-learn` (SMOTE, RandomUnderSampler)
  - Evaluation: `classification_report`, `roc_auc_score`, `confusion_matrix`

---

## 🔍 Workflow & Methodology

### 1️⃣ Data Preprocessing
- Normalization of `Time` and `Amount` features
- Splitting dataset into training and testing sets (stratified)
- Handling class imbalance using:
  - SMOTE (Synthetic Minority Over-sampling Technique)
  - Undersampling
- Visual inspection of fraud vs non-fraud patterns

### 2️⃣ Exploratory Data Analysis (EDA)
- Class distribution plot
- Correlation matrix
- Feature importance visualization
- Boxplots and density plots for fraud vs non-fraud

### 3️⃣ Model Training
- Models implemented:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
- Hyperparameter tuning using GridSearchCV
- Pipeline integration for reproducibility

### 4️⃣ Evaluation Metrics
Due to class imbalance, **accuracy** is not a sufficient metric. Instead, the following are used:
- Precision
- Recall (most critical)
- F1-Score
- ROC-AUC Curve
- Confusion Matrix

---


---


