# Predicting Employee Attrition at Salifort Motors Using Machine Learning

## 📊 Project Overview
This project focuses on predicting whether an employee at **Salifort Motors** will leave or stay at the company using machine learning models. The goal is to help the Human Resources (HR) department proactively identify at-risk employees and implement effective retention strategies.  

By analyzing employee data such as satisfaction level, evaluation score, workload, and promotion history, we developed a predictive model that provides actionable insights into the factors influencing attrition.  

**Model Performance:**  
- **Best Model:** Random Forest Classifier (tuned using GridSearchCV)  
- **AUC Score:** 0.96  
- **Accuracy:** 93%  

---

## 💼 Business Understanding
### **Stakeholder:**  
The Human Resources (HR) team at Salifort Motors.

### **Business Problem:**  
Employee turnover has increased operational costs and affected productivity. The company seeks to understand what factors drive employees to leave and use predictive analytics to reduce attrition rates.

### **Business Objective:**  
1. Identify key factors influencing employee departures.  
2. Build a predictive model to forecast employee attrition.  
3. Provide data-driven recommendations for improving retention.

---

## 🧠 Data Understanding
The dataset contains historical HR data from Salifort Motors, including:  
- **Satisfaction Level**  
- **Last Evaluation**  
- **Number of Projects**  
- **Average Monthly Hours**  
- **Time Spent at Company**  
- **Promotion in Last 5 Years**  
- **Department and Salary Information**  

**Data Timeframe:** Internal HR data covering multiple years of employment records.  

### **Exploratory Data Analysis (EDA):**
- Box plots and histograms were used to visualize the distributions of satisfaction level and working hours.  
- Scatter plots highlighted the relationship between evaluation scores and satisfaction levels.  
- A heatmap revealed strong negative correlations between satisfaction level and attrition.

**Key Finding:** Employees who work longer hours but have low satisfaction are more likely to leave.

---

## ⚙️ Modeling and Evaluation
Several machine learning models were tested, including Logistic Regression, Decision Tree, and Random Forest.  

### **Best Performing Model:**  
**Random Forest Classifier**  
- Tuned using **GridSearchCV** for optimal hyperparameters.  
- **Cross-validation** used to ensure model generalization.  
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, and AUC.

| Metric      | Training | Test |
|--------------|-----------|------|
| Accuracy     | 0.95      | 0.93 |
| Precision    | 0.92      | 0.91 |
| Recall       | 0.94      | 0.92 |
| F1-Score     | 0.93      | 0.92 |
| AUC          | 0.98      | 0.96 |

### **Feature Engineering:**
- Created a new binary variable **`overworked`** to capture employees with high working hours.  
- Dropped redundant features (e.g., satisfaction level) to reduce multicollinearity.  
- Scaled numerical variables for better model performance.

---

## 🧩 Key Insights
1. **Low satisfaction level** is the strongest predictor of attrition.  
2. **Overworked employees** (high average monthly hours) are more likely to leave.  
3. **Lack of promotion** within five years significantly increases turnover risk.  
4. **Departmental and salary factors** also influence employee retention.  

---

## 🏁 Conclusion
The Random Forest model successfully predicts employee attrition with high accuracy. By addressing workload balance, improving recognition, and fostering promotions, Salifort Motors can significantly reduce employee turnover and improve satisfaction.

### **Recommendations:**
- Implement regular employee satisfaction surveys.  
- Review workload and assign projects more evenly.  
- Develop a structured promotion and recognition program.  
- Use this model in HR dashboards for ongoing monitoring.

---

## 🔮 Next Steps
1. **Deploy** the model using Flask for integration into HR analytics dashboards.  
2. **Monitor** prediction accuracy in real-world scenarios and retrain periodically.  
3. **Enhance** the dataset with demographic and departmental details for improved insights.  
4. **Expand** to predictive modeling for performance improvement and engagement scores.

---

## 🧰 Tools and Technologies
- **Languages:** Python  
- **Libraries:** pandas, NumPy, scikit-learn, matplotlib, seaborn  
- **Modeling:** Random Forest, Logistic Regression, GridSearchCV  
- **Visualization:** Matplotlib, Seaborn  
- **Development Environment:** Jupyter Notebook / Visual Studio Code  
- **Version Control:** Git and GitHub  

---

## 🧑‍💼 About the Author
**Name:** Sheku Bangura  
**Certification:** Google Advanced Data Analytics Professional Certificate  
**Role:** Data Analyst / Aspiring Data Scientist  

I’m passionate about leveraging data analytics and machine learning to solve real-world business challenges. This project reflects my ability to translate complex data into strategic insights and actionable business outcomes.

---

## 📂 Repository Structure
