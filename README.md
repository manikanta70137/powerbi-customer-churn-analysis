📊 Customer Churn Analysis | Power BI Project
📌 Project Overview

This project presents an end-to-end Customer Churn Analysis for a telecom company using Power BI.
The objective is to identify key churn drivers, high-risk customer segments, and revenue impact, enabling data-driven customer retention strategies.

The dashboard is fully interactive and powered by custom DAX calculations, advanced segmentation, and KPI-driven insights.

🎯 Business Objectives

Analyze customer churn patterns across demographics, services, and contracts

Identify high-risk customer segments contributing most to churn

Quantify revenue loss vs retained revenue

Support strategic decisions for customer retention and upselling

🛠 Tech Stack

Power BI Desktop – Data modeling & interactive dashboards

Power Query – Data cleaning and transformation

DAX (Data Analysis Expressions) – Calculated columns, measures & KPIs

CSV Dataset – Telecom customer churn data

📂 Dataset Summary

Total Records: 7,043 customers

Target Variable: Churn (Yes / No)

Key Features:

Demographics: Gender, Senior Citizen, Partner, Dependents

Services: Internet, Phone, Streaming, Security, Tech Support

Billing: Contract Type, Payment Method, Monthly & Total Charges

Tenure: Customer lifetime in months

📊 Dashboard Walkthrough & Insights
1️⃣ Customer Demographics Analysis

Screenshot:
Screenshots/customer_demographics.png

What This Shows:

Gender-wise customer distribution

Churn comparison between senior and non-senior citizens

Customer segmentation across tenure ranges

Relationship between tenure and monthly charges

Key Insights:

Customers with low tenure (0–12 months) have the highest churn rate

Senior citizens show relatively higher churn

Monthly charges tend to increase with tenure

2️⃣ Service Subscription Analysis

Screenshot:
Screenshots/service_subscription.png

What This Shows:

Subscription distribution across services

Churn rate by internet service type

Impact of add-on services on churn

Relationship between number of services and churn likelihood

Key Insights:

Fiber optic customers exhibit the highest churn rate

Customers with fewer subscribed services churn more frequently

Add-on services improve customer stickiness

3️⃣ Contract & Billing Insights

Screenshot:
Screenshots/contract_billing.png

What This Shows:

Churn rate by contract type

Payment method distribution and churn behavior

Monthly and total charges across billing methods

Tenure distribution by contract

Key Insights:

Month-to-month contracts have significantly higher churn

Customers using electronic check payments churn more often

Long-term contracts improve customer retention

4️⃣ Churn Drivers & Revenue Impact

Screenshot:
Screenshots/churn_drivers.png

What This Shows:

Overall churn rate

High-risk customer segments

Revenue lost due to churn vs retained revenue

Key Insights:

Overall churn rate is approximately 26%

High churn concentration among:

Month-to-month contracts

Low-tenure customers

Fiber optic users

Churn results in substantial revenue loss, highlighting retention opportunities

📐 Data Modeling & DAX Highlights

This project includes custom DAX calculated columns and measures to support advanced analytics, including:

Tenure-based customer segmentation (6 & 12 bucket models)

Service count per customer to measure engagement

Core churn KPIs (Churn Rate, Churned Customers)

Revenue impact analysis (Lost vs Retained Revenue)

Risk-based churn classification

➡️ All DAX formulas are documented directly in this repository for transparency and interview discussion.

📈 Key KPIs
Metric	Value
Total Customers	7,043
Churned Customers	~1,869
Churn Rate	~26%
Avg Monthly Charges	~64.7
Total Revenue	~456K
Lost Revenue	~139K

🚀 Business Recommendations

Encourage customers to move from month-to-month to long-term contracts

Promote bundled services to improve engagement

Incentivize auto-payment methods to reduce churn

Target high-risk segments with personalized retention campaigns
```bash
📎 Repository Structure
Customer-Churn-Analysis-PowerBI/
│
├── Dataset/
│   └── customer_churn.csv
├── PowerBI/
│   └── Customer Churn Analysis.pbix
├── Screenshots/
│   ├── customer_demographics.png
│   ├── service_subscription.png
│   ├── contract_billing.png
│   └── churn_drivers.png
└── README.md
```

🔗 Add your LinkedIn & GitHub profile links here
