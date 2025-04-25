# Credit Card Fraud Detection using Gradient Boosting Machine (GBM)

## Overview
This project focuses on detecting fraudulent credit card transactions using a Gradient Boosting Machine (GBM) model. The goal was to accurately identify fraud within a highly imbalanced financial dataset, demonstrating the effectiveness of ensemble methods in binary classification problems.

The project covers:
- Data acquisition and preprocessing
- Exploratory Data Analysis (EDA)
- Model training and evaluation
- Benchmark comparison against a Kaggle baseline Random Forest model

## Dataset
The dataset used for this project was sourced from Kaggle's "Credit Card Fraud Detection 2023" dataset, featuring anonymized transaction information including principal components (V1-V28), transaction amount, and class labels (0 = legitimate, 1 = fraud).

## Key Steps
- Scaled the `Amount` feature and dropped the `Time` feature.
- Split the data into an 80/20 stratified train-test split.
- Trained a `GradientBoostingClassifier` with 100 estimators and a learning rate of 0.1.
- Evaluated the model using precision, recall, F1-score, and ROC-AUC metrics.
- Benchmarked model performance against an established Kaggle Random Forest notebook.

## Results
- Precision (Fraud): **1.00**
- Recall (Fraud): **1.00**
- F1-Score (Fraud): **1.00**
- ROC-AUC: **0.9999**
- Slightly outperformed the benchmark Random Forest model, achieving higher accuracy and ROC-AUC under balanced and clean dataset conditions.

## Conclusion
The GBM model demonstrated excellent performance on the balanced dataset. However, real-world fraud detection would involve additional complexities such as class imbalance, feature noise, and dynamic fraud patterns. Future work could explore SMOTE, anomaly detection, and deployment strategies for production environments.

## Project Highlights
- Full data preprocessing pipeline
- Clear EDA visualizations
- ROC and Precision-Recall curve analysis
- Benchmark comparison and visual ROC-AUC comparison
- Kaggle notebook showcasing all results and code

## Technologies Used
- Python
- Pandas, NumPy
- scikit-learn
- Matplotlib, Seaborn
- Kaggle Kernels

---

> *This project demonstrates a strong understanding of machine learning workflows, model evaluation, and fraud detection challenges.* 🚀
