# ML-TASK-1
# 📊 Customer Churn Prediction



## 🔍 Objective
The goal of this project is to **predict customer churn** (whether a customer will leave the service) using machine learning, enabling companies to take **proactive retention actions**.

---

## 📁 Dataset
- Source: [`Telco Customer Churn`](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- Features include demographics, account info, and service usage
- Target: `Churn` (Yes/No)

---

## ⚙️ Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- SHAP (Explainable AI)
- Matplotlib, Seaborn
- Google Colab

---

## 🧪 Project Workflow

### 1. **Data Preprocessing**
- Convert `TotalCharges` to numeric
- Handle missing values
- Encode categorical variables using Label Encoding
- Scale numerical features (`tenure`, `MonthlyCharges`, `TotalCharges`)

### 2. **Model Training**
- Used `GradientBoostingClassifier` for high accuracy and feature importance
- Alternative models (Logistic Regression, SVM) can also be tested

### 3. **Evaluation Metrics**
- Confusion Matrix
- Classification Report (Precision, Recall, F1)
- ROC AUC Score

### 4. **Model Interpretability**
- Used **SHAP (SHapley Additive Explanations)** for model transparency
  - Global: Feature importance summary
  - Local: Waterfall plots for individual predictions

---

## 🚀 How to Run (Google Colab)

1. Upload the dataset: `WA_Fn-UseC_-Telco-Customer-Churn.csv`
2. Copy the full Colab code into a notebook
3. Run all cells
4. View model performance and SHAP explanations

---

## 📈 Results
- ROC AUC Score: ~0.84 (varies slightly with data split)
- Top churn indicators:
  - Contract type
  - Tenure
  - MonthlyCharges
  - Internet service

---

## 💡 Future Work
- Deploy a Streamlit app for real-time churn scoring
- Integrate with company CRM for churn alerts
- Add customer lifetime value (CLV) prediction

---

## 📜 License
This project is for academic and educational use only.

---

## 🙌 Acknowledgements
- Dataset from IBM Sample Data
- SHAP library by Scott Lundberg
