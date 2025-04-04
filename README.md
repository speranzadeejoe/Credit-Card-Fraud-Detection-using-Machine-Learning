# Credit-Card-Fraud-Detection-using-Machine-Learning
# 💳 Credit Card Fraud Detection using Machine Learning

This project uses machine learning techniques to detect fraudulent credit card transactions. It includes data preprocessing, model training, evaluation, and model explainability using SHAP.

---

## 📂 Dataset

- **Source**: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Rows**: 284,807 transactions
- **Features**: 30 (anonymized PCA-transformed features + Time and Amount)
- **Target**: `Class` (0 = Not Fraud, 1 = Fraud)

---

## 🛠️ Project Steps

1. **Data Cleaning**
   - Removed duplicates
   - Checked for missing values

2. **Outlier Detection**
   - Boxplot visualizations revealed many outliers
   - Chose **not to remove outliers** (fraud cases are rare & extreme by nature)

3. **Feature Scaling**
   - Used `RobustScaler` to reduce the effect of outliers
   - Scaled dataset stored as `df_scaled`

4. **Correlation Analysis**
   - Used a heatmap to explore feature correlation
   - No strong multicollinearity found, kept all features

5. **Class Imbalance Handling**
   - Used **SMOTE** or **undersampling** to balance the data
   - Focused on metrics like **Precision, Recall, F1-Score, ROC-AUC**

6. **Modeling**
   - Trained **Random Forest** and **XGBoost** classifiers
   - Tuned hyperparameters for better performance

7. **Explainability with SHAP**
   - Used SHAP to explain feature importance
   - `V14` was the most important feature influencing fraud predictions
   - Visualizations: SHAP summary plot

---

## 📊 Evaluation Metrics

Due to class imbalance, accuracy was not a good metric. Instead, we used:

- ✅ Precision
- ✅ Recall
- ✅ F1-Score
- ✅ ROC-AUC

---

## 🔍 Visualizations

- 📌 Correlation heatmap
- 📌 Boxplot for outliers
- 📌 SHAP summary plot for feature importance

---

## author 
speranza deejoe 
