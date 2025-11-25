# Credit Card Fraud Detection using Gradient Boosting (GBM)

This project explores how transaction patterns can be used to highlight activity that looks unusual, helping fraud teams focus their time on the transactions that matter most. The goal is to demonstrate a clear, repeatable framework for fraud detection while showcasing strong modeling performance using Gradient Boosting.

---

## Problem

Fraud analysts review thousands of transactions, but only a small percentage actually require intervention. Without support, analysts can spend too much time on routine cases while truly suspicious activity becomes harder to prioritize.

---

## Approach

I explored transaction behavior to understand what “typical” card activity looks like, then trained a Gradient Boosting Machine (GBM) model to highlight transactions that differ from those patterns. The focus was on building a practical scoring approach that helps analysts direct their attention where it matters.

Key components of this approach include:

- Data preprocessing, scaling, and feature handling  
- Exploratory Data Analysis (EDA) on spending patterns  
- Model training using a GBM classifier  
- Evaluation using precision, recall, F1-score, ROC-AUC  
- Benchmark comparison against a Kaggle Random Forest model  

---

## Outcome

The GBM model delivered excellent performance, correctly identifying all fraudulent transactions in the test set. While the dataset used was balanced and clean, the project demonstrates how a model like this could support real fraud operations by:

- Prioritizing transactions for manual review  
- Reducing analyst workload  
- Improving detection consistency  

Future enhancements could include SMOTE, anomaly detection, and real-world deployment considerations.

---

## Dataset

The dataset comes from Kaggle’s *Credit Card Fraud Detection 2023* collection, which includes anonymized features (`V1–V28`), transaction amount, and class labels (0 = legitimate, 1 = fraud).

Because the original dataset is imbalanced, this project uses a balanced variant to focus on modeling methodology and interpretability.

---

## Project Steps

### 1. Data Preprocessing
- Scaled `Amount` feature  
- Dropped `Time` feature  
- Created an 80/20 **stratified split**

### 2. Model Training
- `GradientBoostingClassifier`  
- 100 estimators  
- Learning rate = 0.1  

### 3. Evaluation
- Precision (fraud): **1.00**  
- Recall (fraud): **1.00**  
- F1-Score: **1.00**  
- ROC-AUC: **0.9999**

### 4. Benchmark Comparison
The GBM model outperformed a widely referenced Kaggle Random Forest benchmark.

---

## Visuals

