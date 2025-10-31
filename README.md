This repository contains analysis on detecting Parkinson's disease using structured voice-related data from UCI Machine Learning Repository. It focuses on building, comparing and evaluating machine learning models for accurate and efficient screening.

**OVERVIEW:**

The CSV dataset included 195 samples and 24 voice related features such as jitter, shimmer, HNR, MFCCs and Delta coefficients. The goal was to determine how effectively these features can distinguish between healthy individuals and Parkinson’s patients, and to identify the most deployable model for real-world use.

**WorkFlow:**

Data Preparation:
Data was already clean and split into 60% training, 20% validation, and 20% test sets using grouped patient IDs to prevent data leakage.

Feature Selection:
Random Forest feature importance was applied to select the top 20 most influential acoustic features.

Modeling:
Multiple algorithms were compared — LightGBM, Support Vector Machine (RBF), Logistic Regression, and TabPFN.

Evaluation Metrics:
Accuracy, F1-Score, and Confusion Matrix were used to assess model performance and generalization.

Deployment:
LightGBM was selected for deployment due to its balance between accuracy, speed, and ease of integration with APIs.

**Performance Summary**

| Model | Train Accuracy | Test Accuracy | F1-Score |
|--------|----------------|----------------|-----------|
| LightGBM | 85% | 81% | 81% |
| SVM (RBF) | 83% | 83% | 83% |
| Logistic Regression | 85% | 79% | 79% |
| TabPFN | 84% | 73% | 73% |





