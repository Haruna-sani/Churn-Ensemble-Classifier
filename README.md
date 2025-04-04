# 🧠 Customer Churn Prediction Using Ensemble Learning

This project focuses on predicting **customer churn** using a combination of powerful machine learning models: **XGBoost**, **Random Forest (RF)**, and **LightGBM (LGBM)**. An **ensemble model** was built to combine the strengths of all three, and the **SMOTE (Synthetic Minority Over-sampling Technique)** was applied to handle class imbalance in the dataset.

---

## 🔧 Models Used
- 🌲 Random Forest (RF)
- ⚡ XGBoost
- 💡 LightGBM
- 🤝 Ensemble (stacking of RF, XGBoost, and LightGBM)

---

## 📊 Dataset Preprocessing
- **Imbalanced classes** were handled using **SMOTE**, ensuring the model is not biased toward the majority class.
- Features were cleaned, scaled, and encoded appropriately.

---

## 🧪 Performance Metrics Comparison

| Model      | Accuracy | F1 Score | Precision | Recall  | AUC-ROC |
|------------|----------|----------|-----------|---------|---------|
| **XGBoost**     | **0.8445**  | **0.7352**  | 0.7673    | 0.4963  | 0.7149  |
| **Random Forest** | 0.8085   | 0.7303   | 0.7155    | **0.6634**  | **0.7545**  |
| **LightGBM**     | 0.8200   | 0.7297   | 0.7241    | 0.5946  | 0.7361  |
| **Ensemble Model** | **0.8445**   | 0.7175   | **0.7786**    | 0.4275  | 0.6893  |

---

## 🏆 Comparative Analysis & Optimal Model Selection

- **Accuracy**: The **XGBoost** and **Ensemble** models performed the best, each achieving an accuracy of **0.8445**.
- **F1 Score**: **XGBoost** slightly outperformed the others with a score of **0.7352**, making it the best for balanced performance between precision and recall.
- **Precision**: The **Ensemble model** achieved the highest precision (**0.7786**), indicating it had fewer false positives.
- **Recall**: **Random Forest** had the best recall (**0.6634**), showing its strength in identifying actual churn cases.
- **AUC-ROC**: **Random Forest** again led with the highest score (**0.7545**), meaning it had the best true positive vs. false positive rate overall.

---

## ✅ Final Verdict: **XGBoost is the optimal model** for this classification task.

While the ensemble model provided great precision and matched accuracy, XGBoost offered the best **balance between accuracy and F1-score**, making it the most **reliable choice** for general use. However, if **maximizing recall** is critical (e.g., catching as many churns as possible), **Random Forest** might be preferred.

---


## 📌 Future Improvements
- Hyperparameter tuning with GridSearchCV or Optuna
- Feature selection and dimensionality reduction
- Deployment as a web app or REST API

---



