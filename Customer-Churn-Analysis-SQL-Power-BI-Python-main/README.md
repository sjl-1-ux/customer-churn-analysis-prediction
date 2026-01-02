# Customer Churn Analysis  
**by Sejal Dewangan**

---

## 📘 Project Overview  
This project analyzes the **Telco Customer Churn** dataset from Kaggle to identify key factors influencing customer churn and to build a predictive model for customer retention.  
The workflow includes **data cleaning**, **interactive visualization**, and **machine learning** using a **Random Forest classifier**.

---

## 🛠️ Tools & Technologies  
- **SQL Server:** Data cleaning and preprocessing  
- **Power BI:** Interactive dashboards and visualizations  
- **Python (Jupyter Notebook):** Machine learning modeling and evaluation  
- **Libraries:** pandas, matplotlib, seaborn, scikit-learn  

---

## 📊 Dataset  
Dataset: [Telco Customer Churn – Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  

The dataset contains detailed customer data, including demographics, services subscribed, account details, and churn status.  

**Data Preparation Steps:**  
- Handled missing values and data inconsistencies in **SQL Server**.  
- Converted the `TotalCharges` column from string to float.  
- Encoded the `Churn` column as binary (`Yes = 1`, `No = 0`).  
- Imported the cleaned dataset into **Power BI** to build interactive dashboards.  
- Exported data to **Python (Jupyter Notebook)** for machine learning analysis using the **Random Forest** algorithm.  

**Model Setup:**  
- Data split: **80:20 (train:test)**  
- Estimators: **100**  
- Random state: **42**  
- Evaluation metrics: Precision, Recall, F1-Score, and Accuracy  

---

## 📈 Model Evaluation  

| Metric    | Class 0 (Retained) | Class 1 (Churned) |
| ---------- | ------------------ | ----------------- |
| Precision  | 83%                | 67%               |
| Recall     | 92%                | 46%               |
| F1-Score   | 87%                | 55%               |

**Overall Accuracy:** 80%

---

## 🔍 Key Insights  

1. **Tenure and Churn:**  
   - Churned customers stay for an average of **18 months**, while retained customers stay around **38 months**.  
   - Longer tenure correlates with higher retention.

2. **Internet Service Type:**  
   - **Fiber optic** users show the highest churn (~42%),  
     **DSL** users churn moderately (~20%),  
     and customers **without internet service** churn the least (~6%).  

3. **Contract Type:**  
   - **Month-to-month** users have the highest churn (~45%),  
     compared to **one-year (~12%)** and **two-year (~2%)** contracts.  

4. **Lifetime Value (LTV):**  
   - Retained customers contribute significantly higher LTV compared to churned ones.  

5. **Feature Importance:**  
   - **Internet Service** and **Contract Type** strongly influence churn and LTV,  
     while **Gender** has negligible impact.  

---

## 💡 Business Insights & Recommendations  

### 1. Encourage Long-Term Contracts  
- **Insight:** Month-to-month users churn the most (~45%), while two-year users churn the least (~2%).  
- **Action:** Offer loyalty discounts, rewards, or exclusive benefits for long-term contract commitments.

### 2. Improve Fiber Optic Customer Experience  
- **Insight:** Fiber optic users show the highest churn (~42%).  
- **Action:** Assess service quality and pricing issues; introduce tailored plans or enhanced support.  

### 3. Strengthen Early Engagement  
- **Insight:** Most churn occurs within the first **18 months**.  
- **Action:** Implement onboarding programs, customer education, and first-year retention incentives.  

### 4. Boost Lifetime Value via Segmentation  
- **Insight:** Contract type and internet service significantly affect LTV.  
- **Action:** Use customer segmentation to identify low-LTV customers and apply upselling or cross-selling strategies.  

### 5. Offer Proactive Technical Support  
- **Insight:** Strong technical support correlates with higher retention.  
- **Action:** Launch proactive support initiatives and monitor high-risk accounts for early intervention.  

### 6. Leverage Machine Learning for Churn Prediction  
- **Insight:** The Random Forest model predicts churn with **80% accuracy**.  
- **Action:** Deploy the model for early churn detection and trigger automated retention campaigns.

---

## 🧠 Summary  
This project demonstrates a complete data-driven workflow — from **data cleaning in SQL**, **visual storytelling in Power BI**, to **predictive modeling in Python**.  
By understanding churn patterns and leveraging machine learning, businesses can **proactively retain customers**, **increase LTV**, and **enhance overall service experience**.

---
