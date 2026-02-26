# 💰 Bitcoin Fraud Detection System (TDSP-Based ML Project)

## 🚀 Overview

This project presents an end-to-end **Bitcoin Fraud Detection System** built using machine learning and aligned with the **Team Data Science Process (TDSP)** methodology. The system identifies fraudulent transactions from blockchain data using advanced modeling, feature engineering, and evaluation techniques.

It also includes an interactive **Streamlit web application** for real-time fraud prediction.

---

## 🎯 Problem Statement

Detect whether a Bitcoin transaction is:

- ✅ Legitimate  
- 🚨 Fraudulent  

This is a **highly imbalanced classification problem**, where missing fraudulent transactions can lead to significant financial loss.

---

## 🧭 Methodology: TDSP (Team Data Science Process)

### 1. Business Understanding

- Objective: Detect fraudulent Bitcoin transactions accurately  
- Key Challenge: Severe class imbalance  
- Success Metric: F1-score, Recall, PR-AUC  

---

### 2. Data Acquisition & Understanding

- Dataset: Elliptic Bitcoin Dataset  
- Contains transaction features and labels:
  - `1` → Fraud  
  - `2` → Legitimate  
  - `unknown` → Removed  

#### Key Insights:

- Highly imbalanced dataset  
- Multiple numerical transaction features  
- Requires careful preprocessing and evaluation  

---

### 3. Data Preparation

- Removed unknown class labels  
- Converted target labels to binary (Fraud = 1, Legit = 0)  
- Handled missing values  
- Performed **train-test split with stratification**  

#### Imbalance Handling:

- Applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance classes  

---

### 4. Exploratory Data Analysis (EDA)

- Class distribution visualization  
- Summary statistics  
- Feature correlation heatmap  

#### Observations:

- Strong class imbalance  
- Some correlated features  
- Need for dimensionality reduction  

---

### 5. Feature Engineering

- **SelectKBest** for selecting top important features  
- **PCA (Principal Component Analysis)** for dimensionality reduction  
- Standardization using **StandardScaler**  

---

### 6. Modeling

Implemented and compared multiple models:

- Logistic Regression  
- Random Forest  
- XGBoost  

#### Approach:

- Used **Pipeline** for clean preprocessing + modeling  
- Applied **GridSearchCV** for hyperparameter tuning  
- Cross-validation used for robust model selection  

---

### 7. Evaluation

Since fraud detection is imbalanced, multiple metrics were used:

- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- PR-AUC (Primary metric for imbalance)  

#### Additional Enhancements:

- Threshold tuning (instead of default 0.5)  
- Model comparison across multiple metrics  

---

### 8. Model Explainability

- Used **SHAP (SHapley Additive Explanations)**  
- Provided feature-level interpretation of predictions  
- Enabled transparency and trust in model decisions  

---
