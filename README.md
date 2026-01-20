# Crypto Wallet Risk Prediction System

## Overview
This project explores the use of machine learning to identify high-risk cryptocurrency wallets based on transaction behavior. The task is framed as an imbalanced classification problem similar to fraud detection in financial systems.

## Dataset
Due to the lack of publicly available labeled wallet risk data, a synthetic dataset was generated to simulate realistic wallet behavior. The dataset includes transaction volume, interaction with exchanges and DeFi protocols, wallet age, and class imbalance typical of real-world risk scenarios.

## Methodology
- Exploratory Data Analysis (EDA) to understand feature distributions and risk patterns
- Stratified train-test split to preserve class imbalance
- Baseline models: Logistic Regression and Random Forest
- Evaluation using precision, recall, F1-score, and ROC-AUC
- Class imbalance handling using class weighting and SMOTE

## Key Findings
- Accuracy alone was misleading due to severe class imbalance
- Logistic Regression improved minority-class recall at the cost of accuracy
- Random Forest struggled to detect high-risk wallets despite class weighting
- Results highlight the need for alternative approaches such as anomaly detection

## Limitations
- Synthetic dataset may not fully capture real-world wallet behavior
- Risk labels are simulated rather than derived from actual security incidents
- Feature set lacks temporal and graph-based transaction patterns

## Future Work
- Incorporate temporal and network-based features
- Explore anomaly detection techniques such as Isolation Forest
- Extend analysis using real blockchain transaction data
