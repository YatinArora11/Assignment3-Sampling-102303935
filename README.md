# Sampling-Technique-Performance-Analysis

**Submitted by:** [Your Name]  
**Roll Number:** [Your Roll Number]

---

## Overview

This project explores the impact of various sampling techniques on machine learning model accuracy when dealing with highly imbalanced datasets.  

Using a **Credit Card Fraud dataset**, we evaluate how different sampling strategies — from simple random sampling to SMOTE — influence the predictive performance of five distinct machine learning classifiers.

---

## Dataset Description

The analysis is performed on the **Credit Card Fraud Dataset**:

- **Source:**  
- **Characteristics:**  
  The dataset is highly imbalanced, a common trait in real-world fraud detection where fraudulent transactions (minority class) are significantly fewer than legitimate ones (majority class).
- **Features:**  
  Includes anonymized numerical features and a **Class** label  
  - `0` → Legitimate  
  - `1` → Fraud  

---

## Methodology

The assignment follows a structured pipeline to compare sampling effectiveness:

### 1. Data Preparation
The initial imbalanced dataset is converted into a **balanced class dataset** to provide a baseline for fair sampling.

### 2️. Sampling Techniques
Five different sampling strategies are applied to generate subsets of the balanced data:

- **Sampling1:** Simple Random Sampling  
- **Sampling2:** Systematic Sampling  
- **Sampling3:** Stratified Sampling  
- **Sampling4:** Cluster Sampling  
- **Sampling5:** Bootstrap Sampling / Random Over-sampling  

### 3️. Machine Learning Models
Each sample is tested against five different models (M1 to M5):

- **M1:** Logistic Regression  
- **M2:** Random Forest  
- **M3:** Support Vector Machine (SVM)  
- **M4:** Decision Tree  
- **M5:** K-Nearest Neighbors (KNN)  

### 4️. Evaluation
Accuracy scores are recorded for every **model–sample combination** to determine which technique yields the highest performance for specific algorithms.

---

## Results Table

The following table summarizes the **accuracy (%)** achieved by each model across the different sampling techniques.


## 📈 Accuracy Comparison Table (%)

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|-----------|-----------|-----------|-----------|-----------|
| **M1** | 25.00 | 93.14 | 93.14 | 93.52 | 91.76 |
| **M2** | 25.00 | 99.35 | 97.06 | 97.95 | 98.88 |
| **M3** | 25.00 | 100.00 | 99.35 | 99.66 | 100.00 |
| **M4** | 25.00 | 75.82 | 72.55 | 73.72 | 79.03 |
| **M5** | 0.00 | 96.08 | 96.73 | 99.66 | 97.75 |


![Accuracy Comparison of Models vs Sampling Techniques](sampling_plots.png)

---

## Conclusion

This project highlights how the choice of sampling technique can significantly influence model performance when handling imbalanced datasets, helping practitioners select the most effective approach for fraud detection tasks.

---



