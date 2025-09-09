# Task 4: Predicting Customer Churn in Telecom

## 📌 Objective
The goal of this task is to build a machine learning model that predicts whether a customer will churn (leave the telecom service) based on their demographic, account, and service usage data.

---

## 📂 Dataset
- **Name:** Telco Customer Churn (Kaggle)
- **Rows:** ~7,000  
- **Columns:** 21  
- **Target Variable:** `Churn` (Yes/No)

---

## 🛠️ Tools & Libraries
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- scikit-learn (Logistic Regression, Random Forest, preprocessing)
- joblib (for saving model)

---

## 🔎 Workflow
1. Data Cleaning & Preprocessing  
   - Converted `TotalCharges` to numeric  
   - Handled missing values  
   - Encoded categorical variables (LabelEncoder + OneHotEncoder)  
   - Scaled numerical features with StandardScaler  

2. Model Training  
   - **Logistic Regression** (baseline)  
   - **Random Forest Classifier** (better performance, used for feature importance)  

3. Model Evaluation  
   - Metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC  
   - Confusion Matrix and Classification Report  

4. Feature Importance  
   - Identified top drivers of churn (e.g., Contract type, Tenure, InternetService, PaymentMethod)  

5. Model Saving  
   - Best performing model saved as `churn_model.pkl` for future deployment  

---

## 📊 Results
- Logistic Regression: ~80% accuracy  
- Random Forest: ~85% accuracy with better recall  
- Key churn drivers: Contract type, Tenure, Internet service, Payment method  

---

## 📁 Deliverables
- `Customer Churn.ipynb` → Jupyter Notebook with full workflow  
- `WA_Fn-UseC_-Telco-Customer-Churn.csv` → dataset  
- `churn_model.pkl` → saved RandomForest model  
- `README.md` → documentation  

---

