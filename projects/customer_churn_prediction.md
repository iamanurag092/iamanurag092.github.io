# Customer Churn Prediction 📉

## 🧠 Problem Statement
Identify customers who are most likely to **churn** using historical customer behavior data.  
This helps the business reduce churn and improve customer retention strategy.

Churn prediction enables:
- **Proactive Retention** through early identification
- **Cost Efficiency** by focusing on high-risk users
- **Targeted Marketing** and personalized offers
- **Business Growth** via data-driven retention strategy

---

## 📊 Dataset
- Source: Internal telecom company data (simulated)
- Rows / Columns: 100,000 records / 9 variables
- Key features: Age, Gender, Location, Subscription Length, Monthly Bill, Total Usage

---

## 🔧 Approach

### **1️⃣ Data Preprocessing**
- Confirmed no missing values or duplicates
- One-hot encoded categorical variables: Gender, Location
- Applied Min-Max scaling to numeric features
- Checked and confirmed class balance in the churn target

### **2️⃣ Exploratory Data Analysis (EDA)**
- Analyzed churn rate by location and gender
- Explored billing and usage patterns across churn classes
- Correlation matrix and VIF for multicollinearity
- Feature importance identified top predictors:
  - Monthly Bill
  - Total Usage (GB)
  - Age
  - Subscription Length

### **3️⃣ Model Building**
Models used:
- Logistic Regression  
- Random Forest  
- XGBoost (selected final model)
- SVM, Decision Tree, AdaBoost, Gradient Boosting, Neural Network (tested)
- PCA and ensemble stacking (not significantly beneficial)

### **4️⃣ Evaluation**
- **Train Set:**
  - Accuracy: **66.49%**  
  - F1-score: **65.98%**  
  - ROC-AUC: **0.66**

- **Test Set:**
  - Accuracy: **50.05%**  
  - F1-score: **49.23%**  
  - ROC-AUC: **0.50**

---

## 📈 Key Insights
- Higher **monthly bills** are correlated with increased churn risk  
- Users with **shorter subscription lengths** churn more  
- Churn distribution is nearly balanced  
- Feature selection revealed limited benefit from PCA or deep models

---

## 📂 GitHub Repository
👉 [View Full Code](https://github.com/iamanurag092/Customer-Churn-Prediction-main/tree/main)

---
