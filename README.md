# Fraud-Detection-in-Financial-Transactions-Using-Machine-Learning

[![Open in Colab](https://img.shields.io/badge/Open%20in-Colab-ffa500.svg)](https://colab.research.google.com/drive/1EuxqO-rxH7fKSH2RPZaTEi8l_v8c6olA#scrollTo=26GsVX6fxRju)
[![Dataset on Kaggle](https://img.shields.io/badge/Dataset%20on-Kaggle-blue.svg)](https://www.kaggle.com/datasets/ealaxi/paysim1)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
---
This repository contains a complete machine learning pipeline for detecting fraudulent financial transactions using the [PaySim](https://www.kaggle.com/datasets/ealaxi/paysim1) dataset. 
We implement and compare five classification models to evaluate their performance in identifying fraud in an extremely imbalanced dataset.

---

![Fraud-Detection](https://github.com/ABUALHUSSEIN/Fraud-Detection-in-Financial-Transactions-Using-Machine-Learning/blob/main/Fraud_Detection.jpg)

---
## 📊 Dataset Overview

The **PaySim** dataset simulates mobile money transactions similar to real financial services. It contains over 6 million transactions and features like transaction type, amount, sender/receiver IDs, and fraud label.

- Total transactions: 6,362,620  
- Fraudulent transactions: ~0.1%  
- Highly imbalanced, requiring specialized techniques to detect fraud effectively.

---

## 🧪 Models Implemented

We trained and compared the following classification models:

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**
4. **Naive Bayes**
5. **XGBoost**

Each model includes:
- Custom preprocessing pipeline ( scaling, encoding)
- Class imbalance handling using **SMOTE**
- Threshold tuning for optimal decision boundary
- Model evaluation using ROC AUC, F1-score, classification report, and confusion matrix

---

## ⚙️ Preprocessing Pipeline

- Missing value imputation (if any)
- One-hot encoding for categorical features
- Standard scaling for numerical features
- SMOTE for synthetic oversampling of fraud cases
- Stratified train-test split to preserve class distribution

---

## 📈 Model Evaluation Metrics

We focused on metrics suitable for imbalanced classification:

- **ROC AUC Score**
- **Precision, Recall, F1-Score**
- **Confusion Matrix**
- **Classification Report**
- **PR Curve & ROC Curve**

---

## 🏆 Best Model

After metric comparison, **XGBoost** performed best in balancing precision and recall for fraud detection, followed closely by **Random Forest**.

---
## Run the Notebook
1. **Clone the repository**
```bash
git clone https://github.com/ABUALHUSSEIN/Fraud-Detection-in-Financial-Transactions-Using-Machine-Learning
cd Fraud-Detection-in-Financial-Transactions-Using-Machine-Learning
```
2. **Install dependencies**
```bash
pip install -r requirements.txt
```
---


📚 References
[PaySim Dataset - Kaggle](https://www.kaggle.com/datasets/ealaxi/paysim1)





