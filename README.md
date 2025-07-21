# 💳 Credit Card Fraud Detection

Detecting fraudulent transactions using machine learning on the imbalanced Kaggle dataset: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

---

## 📁 Dataset Summary

- **Records:** 284,807 transactions
- **Fraudulent:** 492 (~0.17%)
- **Features:** 30 total (V1–V28 anonymized, Amount, Time), `Class` is target (0 = legit, 1 = fraud)

---

## ⚙️ Workflow Overview

1. **EDA**
   - No missing values
   - Extreme class imbalance detected
2. **Preprocessing**
   - Dropped `Time`, scaled `Amount`
   - Handled imbalance using **SMOTE**
3. **Feature Engineering**
   - Reviewed low-variance features, retained for modeling
4. **Model Training**
   - Trained 3 models: Logistic Regression, Random Forest, Isolation Forest

---

## 🤖 Model Performance

### ✅ Random Forest (Best)

- **Training Accuracy:** 100.00%  
- **Testing Accuracy:** 99.94%  
- **ROC AUC:** 0.9682  
- **Fraud Detection (Class 1):**  
  - Precision: 0.8657  
  - Recall: 0.7838  
  - F1-score: 0.8227  

### 📉 Logistic Regression

- **Training Accuracy:** 95.72%  
- **Testing Accuracy:** 97.68%  
- **ROC AUC:** 0.9676  
- **Fraud Detection (Class 1):**  
  - Precision: 0.0620  
  - Recall: 0.8784  
  - F1-score: 0.1158  

### 🧪 Isolation Forest

- **Accuracy:** 99.73%  
- **ROC AUC:** 0.9426  
- **Fraud Detection (Class 1):**  
  - Precision: 0.2297  
  - Recall: 0.2297  
  - F1-score: 0.2297  

---

## 🧰 Tools Used

- Python, Pandas, NumPy
- Scikit-learn, Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

---

## 📌 Conclusion

- **Random Forest** achieved the best balance of fraud detection accuracy and precision.
- Logistic Regression was underfitting.
- Isolation Forest underperformed for precision/recall, but useful for anomaly detection.

---


