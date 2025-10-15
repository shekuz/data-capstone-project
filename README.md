# 🧠 Predicting Employee Attrition at Salifort Motors Using Machine Learning

## 📘 Project Overview
This project focuses on predicting **whether an employee at Salifort Motors will leave or stay** using machine learning.  
By leveraging HR data, we built a predictive model to identify employees at risk of attrition and provide actionable insights for HR to improve employee satisfaction and retention.

**Goal:**  
Help Salifort Motors make data-driven HR decisions that reduce turnover and improve productivity.

**Best Model:** Random Forest Classifier  
**Performance:** AUC = 0.96 | Accuracy = 93%  

---

## 💼 Business Understanding
**Stakeholder:** Human Resources (HR) Department, Salifort Motors  

**Business Problem:**  
High employee turnover increases recruitment costs and reduces productivity. The company needs to understand key factors contributing to attrition and proactively retain valuable employees.

**Business Objective:**  
- Identify patterns and key factors that influence employee departures.  
- Build a predictive model to forecast attrition risk.  
- Recommend strategic HR interventions based on insights.

---

## 🧠 Data Understanding
The dataset contains HR records from Salifort Motors, including:  
- **Satisfaction level**  
- **Last evaluation score**  
- **Average monthly hours**  
- **Number of projects**  
- **Time spent at company**  
- **Promotion in last 5 years**  
- **Salary level**  

**Exploratory Data Analysis (EDA):**
- **Box plots & histograms**: Visualized distribution of satisfaction levels and hours worked.  
- **Scatter plots**: Showed correlation between satisfaction and evaluation.  
- **Heatmap**: Identified strong negative correlation between satisfaction level and attrition.

**Key Finding:**  
Employees with **high workload** and **low satisfaction** were more likely to leave.

---

## ⚙️ Modeling and Evaluation
Multiple machine learning algorithms were tested:
- Logistic Regression  
- Decision Tree  
- Random Forest (best-performing model)  

**Best Model:** Random Forest (tuned via GridSearchCV)  

| Metric      | Training | Test |
|--------------|-----------|------|
| Accuracy     | 0.95      | 0.93 |
| Precision    | 0.92      | 0.91 |
| Recall       | 0.94      | 0.92 |
| F1-Score     | 0.93      | 0.92 |
| AUC          | 0.98      | 0.96 |

**Feature Engineering:**
- Created a binary feature `overworked` to capture employees with high working hours.  
- Dropped redundant variables and standardized features.  
- Used 5-fold cross-validation for robust evaluation.

---

## 🔍 Key Insights
1. **Low satisfaction** and **excessive workload** strongly predict employee attrition.  
2. **Lack of promotion** in 5 years correlates with higher turnover risk.  
3. **High performers** working long hours without recognition are at greater risk of leaving.  

---

## 🏁 Conclusion & Recommendations
The Random Forest model effectively predicts attrition and provides valuable insights into employee behavior.  

**Recommendations:**
- Conduct regular satisfaction surveys.  
- Monitor workloads and ensure work-life balance.  
- Improve recognition and promotion systems.  
- Use this model for ongoing HR analytics and retention forecasting.

---

## 🚀 How to Run This Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/salifort-attrition-prediction.git
cd salifort-attrition-prediction
