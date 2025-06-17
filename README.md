
# 📞 Telecom Churn Analysis and Prediction – Power BI & ML Project

An interactive Power BI dashboard project designed to analyze customer churn behavior for a telecom company. This solution helps understand churn drivers and patterns using demographic, behavioral, geographic, and service usage dimensions.

### 🔗 Download Dashboard on your PC: [Dashboard URL](https://drive.google.com/file/d/1-7r-CzWsZQ5Io7Q7aBk1i1ZYDuJe7WAW/view?usp=drive_link)

---

## 📊 Project Overview

This project investigates customer churn for a telecom company by combining descriptive and predictive analytics using Power BI, SQL, and Python. It comprises four major components:

### 1. ETL Process

A structured ETL (Extract, Transform, Load) pipeline was implemented using SQL Server tools:

Source data ingested from CSV files.

Transformation and cleaning using SQL queries.

Loaded into a production-ready database with views created for Power BI.

### 2. Churn Analysis Dashboard

   This Dashboard investigates churn among telecom customers and answers key questions such as:
   
  Which customer segments have the highest churn rate?
  
  How do contracts, services, and payment methods influence churn?
  
  What are the key geographical zones contributing to churn?
  
  Which reasons dominate churn categories?

### 3. Churn Prediction Model based on Random Forest Algorithm

A machine learning-based prediction model was developed using the Random Forest algorithm in Python. It included:

Preprocessing with label encoding and null handling

Training and evaluation of the model using a variety of performance metrics

Predicting churn probability and assigning risk profiles to customers

### 4. Churn Prediction Dashboard

A dedicated dashboard was built in Power BI on top of the prediction output. It includes:

Total predicted churners

Gender-based churn counts

Churn by age group, marital status, tenure, contract, payment method, and state

Customer risk profile matrix

Using advanced DAX measures and data modeling, the dashboard presents insights to support **retention strategies** and **customer lifetime value enhancement**.

---

## 🔄 ETL Framework

The data for this project was extracted and processed using a structured ETL pipeline as described below:

CSV File: This is the raw source file containing customer churn data.

SQL Server Management Studio (SSMS): Used the built-in import wizard to load and transform the data into a staging table.

SQL Server Database: Final cleaned data was inserted into a production table, which is then used to build Power BI views.

This process ensures data quality, consistency, and scalability for downstream analysis.


## 🧠 Insights & Visual Analysis

### 1. 🧮 KPI Metrics Overview

**Visual Used:** 



![KPI Card Metrics (Total Customers, New Joiners, Total Churn, Churn Rate)](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/KPIs.png)




**Insights:**  
These KPIs provide a quick snapshot of business health:
- **Total Customers:** 6,418  
- **New Joiners:** 411  
- **Total Churn:** 1,732  
- **Churn Rate:** 26.99%  

Helps track churn dynamics and growth pace at a glance.

---

### 2. 🔗 Churn Rate by Contract Type

**Visual Used:** 



![Churn Rate by Contract](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20%20y%20contract.png)




**Insights:**  
- **Month-to-Month:** Highest churn (46.53%)  
- **Two Year:** Very low churn (2.73%)  

**Suggestion:** Longer contracts significantly improve customer retention.

---

### 3. 💳 Churn Rate by Payment Method

**Visual Used:** 



![`Churn Rate by Payment`](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20payment.png)




**Insights:**  
- **Mailed Check:** 37.82% churn  
- **Bank Withdrawal:** 34.43%  
- **Credit Card:** Lowest at 14.80%  

Promoting digital payments can help reduce churn.

---

### 4. ⏳ Churn by Tenure Group

**Visual Used:** 


![`Churn Rate and Total Churn by Tenure Group.png`](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20tenure.png)




**Insights:**  
- Churn is highest in **<6 months** and **>24 months** groups.  
- Shows a need for better onboarding and long-term engagement.

---

### 5. 📡 Churn by Internet Type

**Visual Used:** 



![`Churn Rate by Internet type.png`](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20internet%20final.png)




**Insights:**  
- **Fiber Optic:** 41.10% churn rate  
- **None:** Only 7.84%  
Service type plays a major role in customer satisfaction and retention.

---

### 6. 🌐 State-Wise Churn Rates

**Visual Used:** 


![Churn Rate by State(Top 5)](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20state.png)




**Insights:**  
Top states by churn rate:
- **Jammu & Kashmir:** 57.19%  
- **Assam:** 38.13%  
Geo-specific patterns help prioritize regions for service improvement.

---

### 7. 📦 Churn by Services Used

**Visual Used:** 



![`Churn Rate by Services.png`](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20services.png)




**Insights:**  
- Customers **without Online Security**, **Online Backup**, or **Device Protection** churn at a much higher rate.  
- **Unlimited Data** and **Streaming Services** reduce churn.  

Bundling value-added services can enhance loyalty.

---

### 8. 📁 Churn Category Breakdown

**Visual Used:** 



![`Churn by Category.png`](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20reason.png)




**Insights:**  
- **Competitor**: Leading cause with 350 churns  
- Followed by **Attitude**, **Dissatisfaction**, **Price**, and **Others**  

These help identify emotional and competitive factors affecting loyalty.

**Also added a Tooltip in this Visual which shows data dynamically as we hover over the Churn Category plot to further elaborate the data and provide clarification to the stakeholder's eye.**

**Tooltip Visual**



![Tooltip Visual](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cr%20tooltip.png)




---

### Dashboard Snapshot



![Churn Dashboard](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/churn%20dashboard%20snapshot.png)




---

## 🧱 Data Modeling

Star schema implemented in Power BI with:

- **Fact Table:** Churn Info  
- **Dimensions:** Customers, Account Info, Payment, Services, Geography

Relationships are built using `Customer ID` as the primary key across multiple tables.

---

## 📌 Key Takeaways

- Long-term contracts and credit card payments show reduced churn.
- Streaming, unlimited data, and online security services retain customers.
- Regional churn variation highlights weak service areas.
- Competitor-driven churn dominates; strategic pricing and upgrades are needed.

---
### Churn Prediction Analysis

## 📊 Churn Prediction Model using Random Forest

In addition to historical churn analysis, a **Random Forest-based Churn Prediction Model** was built using Python. The steps included:

1. **Data Preprocessing:**
   - Handled missing values.
   - Converted categorical variables using Label Encoding.
2. **Feature Selection:**
   - Key features: tenure, payment method, contract type, services used, etc.
3. **Model Training:**
   - Trained a Random Forest Classifier on the cleaned dataset.
4. **Evaluation:**
   - Evaluated performance using accuracy, precision, recall, F1-score, and confusion matrix.
5. **Prediction:**
   - Applied model to generate churn predictions and assigned risk scores.

A separate dashboard was then created in Power BI based on these predictions.

---

## 📊 Churn Prediction Dashboard




![Churn Prediction Dashboard](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/PredicitonDashboard.png)




**Key Metrics & Visuals:**
- **Total Predicted Churners:** 382
- **Gender Split:**
  - Female: 249
  - Male: 133




![Churn Count by Gender](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_churncount.png)




- **Demographics:**
  - By Age Group



 
![Churn Count by Age Group](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_agegrp.png)




  - Marital Status



 
![Churn Count by Marital Status](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_married.png)




  - Tenure Group



 
  ![Churn Count by Tenure Group](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_tnrgrp.png)


 
    
- **Behavioral Patterns:**
  - By Contract Type



![Churn Count by Contract](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_contract.png)




  - Payment Method



![Churn Count by Contract](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_paymentmethod.png)




- **Geography:**
  - Predicted churn by state
 


  ![Churn Count by Contract](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_state.png)




- **Customer Risk Table:**
  - Includes Customer ID, Monthly Charge, Total Revenue, Refunds, Number of Referrals



  ![Churn Count by Contract](https://github.com/gurpreet998/Telecom-Churn-Analysis/blob/main/Images/cp_customerrisk.png)


    

## This dashboard provides forward-looking insights into which customers are at risk and helps create proactive retention strategies.


## 🙋‍♂️ About Me

Hi, I’m **Gurpreet Singh**, a Data Analyst passionate about solving business problems using data. I specialize in Power BI, SQL, and storytelling through visuals. Currently working at Accenture (Gurugram), I’m open to exciting new opportunities in data analytics and business intelligence.

📫 **Email:** gs268197@gmail.com  
📱 **Mobile:** +917018320090  
🔗 **LinkedIn:** [linkedin.com/in/gurpreetsingh1998](https://linkedin.com/in/gurpreetsingh1998)  
💻 **GitHub:** [github.com/gurpreet998](https://github.com/gurpreet998)  
🌐 **Website:** [gurpreet-singh-998.vercel.app](https://gurpreet-singh-998.vercel.app)
