
# 📞 Telecom Churn Analysis Dashboard – Power BI Project

An interactive Power BI dashboard project designed to analyze customer churn behavior for a telecom company. This solution helps understand churn drivers and patterns using demographic, behavioral, geographic, and service usage dimensions.

### 🔗 Dashboard Link: *(Add your dashboard link here – e.g., Google Drive or Power BI Service)*

---

## 📊 Project Overview

This project investigates churn among telecom customers and answers key questions such as:
- Which customer segments have the highest churn rate?
- How do contracts, services, and payment methods influence churn?
- What are the key geographical zones contributing to churn?
- Which reasons dominate churn categories?

Using advanced DAX measures and data modeling, the dashboard presents insights to support **retention strategies** and **customer lifetime value enhancement**.

---

## 🗂️ Data Sources

| Dataset Name             | Description |
|--------------------------|-------------|
| **Customer Details**     | Customer ID, Age, Gender, Marital Status |
| **Account Info**         | Tenure, Monthly Charges, Total Charges, Contract Type |
| **Service Usage**        | Internet, Streaming, Backup, Security, Tech Support |
| **Payment Info**         | Payment Method, Paperless Billing |
| **Churn Info**           | Churn Flag, Churn Category, Churn Reason |
| **Geography**            | State, Region |

---

## 🧠 Insights & Analysis

### 1. 🧮 KPI Metrics Overview

**Visual Used:**  
*(Insert snapshot of KPI cards – Total Customers, New Joiners, Churned Customers, Churn Rate)*

**Insights:**  
These cards provide an at-a-glance summary of core churn statistics.  
- **Total Customers** gives the active user base.  
- **New Joiners** helps track customer acquisition.  
- **Churn Count** and **Churn Rate** highlight overall attrition.  
These KPIs help benchmark churn over time and provide an instant view for decision-makers.

---

### 2. 👤 Churn by Demographics

**Visual Used:**  
*(Insert bar chart showing churn by age groups, gender, marital status)*

**Insights:**  
The visual shows that:
- Customers aged **above 50** have a higher churn rate.  
- **Divorced and single** customers tend to churn more frequently than married ones.  
These insights can guide targeted retention strategies, like loyalty benefits or personalized plans.

---

### 3. 📍 Churn by Geography

**Visual Used:**  
*(Insert state-wise churn chart or filled map)*

**Insights:**  
Certain states such as **Jammu & Kashmir** exhibit a churn rate exceeding 57%.  
This regional breakdown helps in identifying underperforming regions and optimizing local outreach or support services.

---

### 4. 🔗 Churn by Contract Type

**Visual Used:**  
*(Insert stacked column chart – churn rate by contract type)*

**Insights:**  
- **Month-to-month contracts** have the highest churn rate (~46%).  
- **2-year contracts** are the most stable (churn rate < 3%).  

This analysis suggests pushing long-term contracts via discounts or loyalty programs to reduce customer attrition.

---

### 5. 💳 Payment Method vs Churn Rate

**Visual Used:**  
*(Insert pie or bar chart – churn rate by payment method)*

**Insights:**  
- **Mailed Check** payments lead to the highest churn (~38%).  
- **Credit Card** and **Electronic Check** show better retention.  

Encouraging auto-pay or digital payments can help minimize churn.

---

### 6. ⏳ Tenure-Based Churn Analysis

**Visual Used:**  
*(Insert line or bar chart showing churn by tenure group)*

**Insights:**  
- Highest churn is observed in customers with **<6 months** and **>24 months** tenure.  
- New customers may be disillusioned early, while older ones may feel under-valued.  

Tailored onboarding for new users and loyalty benefits for long-term users are necessary strategies.

---

### 7. 📡 Services vs Churn

**Visual Used:**  
*(Insert matrix or table – services like Streaming, Internet, Tech Support vs churn rate)*

**Insights:**  
- Lack of **Device Protection**, **Online Backup**, or **Streaming Services** increases churn probability.  
- Offering bundled packages may increase stickiness.  

This table helps identify service combinations that retain customers better.

---

### 8. 🗃️ Churn Reasons & Categories

**Visual Used:**  
*(Insert bar chart – Churn Category & Churn Reason frequency)*

**Insights:**  
Top reasons for churn include:  
- **Competition**  
- **Attitude**  
- **Dissatisfaction**  

These qualitative categories offer a powerful lens into customer sentiment and external market pressures.

---

## 🧱 Data Modeling

All datasets were joined using unique keys such as `Customer ID`. The model follows a star schema with:

- **Fact Table:** Churn Info  
- **Dimension Tables:** Customers, Services, Contracts, Geography, Payments

**Key Relationships:**  
- `Customer_ID` → `Customer Details`, `Account Info`, `Service Usage`  
- `Customer_ID` → `Payment Info`, `Churn Category`, `Geography`  

---

## 📈 Dashboard Snapshots

📌 KPI Overview  
*(Insert image)*

📌 Churn by Age Group  
*(Insert image)*

📌 Churn by Contract Type  
*(Insert image)*

📌 Churn by Services  
*(Insert image)*

📌 Churn Category / Reasons  
*(Insert image)*

---

## 🧠 Key Takeaways

- Customers on **month-to-month contracts**, and those aged **above 50**, are at highest churn risk.  
- **Mailed Check** and **paper billing** users are more likely to leave.  
- States like **Jammu & Kashmir** have much higher churn, indicating possible service dissatisfaction or competition.  
- **Lack of streaming and protection plans** contributes to higher churn.  
- Churn due to **competition** and **dissatisfaction** points to market repositioning needs.

---

## 📌 Conclusion

This dashboard serves as a powerful churn management tool. With its interactive features, executives and analysts can:  
- Monitor churn trends  
- Segment risky customers  
- Understand behavioral patterns  
- Deploy targeted retention strategies  

By leveraging churn data effectively, telecom companies can improve profitability, reduce acquisition costs, and enhance customer satisfaction.

---

## 🙋‍♂️ About Me

Hi, I’m **Gurpreet Singh**, a Data Analyst passionate about solving business problems using data. I specialize in Power BI, SQL, and storytelling through visuals. Currently working at Accenture (Gurugram), I’m open to exciting new opportunities in data analytics and business intelligence.

📫 **Email:** gs268197@gmail.com  
📱 **Mobile:** +91 7018320090  
🔗 **LinkedIn:** [linkedin.com/in/gurpreetsingh1998](https://linkedin.com/in/gurpreetsingh1998)  
💻 **GitHub:** [github.com/gurpreet998](https://github.com/gurpreet998)  
🌐 **Website:** [gurpreet-singh-998.vercel.app](https://gurpreet-singh-998.vercel.app)
