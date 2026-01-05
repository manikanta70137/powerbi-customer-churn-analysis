Customer Churn Analysis using Power BI
Project Overview

This project presents an end-to-end Customer Churn Analysis for a telecom company using Power BI. The primary objective is to identify key churn drivers, high-risk customer segments, and revenue impact in order to support data-driven customer retention strategies.

The dashboard is fully interactive and built using Power Query for data transformation, DAX for calculated columns and measures, and Power BI visual analytics for business storytelling.

Business Objectives

Analyze customer churn patterns across demographics, services, and contracts

Identify high-risk customer segments contributing most to churn

Measure churn impact on revenue (lost vs retained revenue)

Enable data-driven decisions for customer retention and engagement

Tech Stack

Power BI Desktop – Dashboard development and data modeling

Power Query – Data cleaning and transformation

DAX (Data Analysis Expressions) – Calculated columns, measures, KPIs

CSV Dataset – Telecom customer churn data

Dataset Summary

Total Records: 7,043 customers

Target Variable: Churn (Yes / No)

Key Attributes:

Demographics: Gender, Senior Citizen, Partner, Dependents

Services: Phone, Internet, Streaming, Security, Tech Support

Billing: Contract Type, Payment Method, Monthly Charges, Total Charges

Tenure: Customer lifetime in months

Dashboard Walkthrough and Insights
Customer Demographics Analysis

Screenshot path:
Screenshots/customer_demographics.png

Analysis Covered:

Gender distribution of customers

Senior citizen churn comparison

Customer tenure segmentation

Monthly charges versus tenure analysis

Key Insights:

Customers with low tenure (0–12 months) have the highest churn rate

Senior citizens show relatively higher churn

Monthly charges generally increase with tenure

Service Subscription Analysis

Screenshot path:
Screenshots/service_subscription.png

Analysis Covered:

Subscription distribution across services

Churn rate by internet service type

Impact of add-on services on churn

Service count versus churn likelihood

Key Insights:

Fiber optic users show the highest churn

Customers with fewer subscribed services are more likely to churn

Bundled services improve customer retention

Contract and Billing Insights

Screenshot path:
Screenshots/contract_billing.png

Analysis Covered:

Churn rate by contract type

Payment method distribution and churn behavior

Monthly and total charges comparison

Tenure distribution across contract types

Key Insights:

Month-to-month contracts have significantly higher churn

Customers using electronic check payments churn more frequently

Long-term contracts lead to better customer retention

Churn Drivers and Revenue Impact

Screenshot path:
Screenshots/churn_drivers.png

Analysis Covered:

Overall churn rate

High-risk customer segments

Revenue lost due to churn versus retained revenue

Key Insights:

Overall churn rate is approximately 26 percent

Churn is concentrated among month-to-month contract customers, low-tenure customers, and fiber optic service users

Churn results in substantial revenue loss, highlighting retention opportunities

Data Modeling and DAX Calculations

This project includes custom DAX calculated columns and measures to support advanced analysis, including:

Tenure-based customer segmentation using 6 and 12 bucket models

Service count calculation per customer

Core churn KPIs such as churn rate and churned customers

Revenue impact analysis including lost and retained revenue

Risk-based churn classification

All DAX formulas are documented directly in the repository for transparency and interview discussion.

Key KPIs

Total Customers: 7,043

Churned Customers: Approximately 1,869

Churn Rate: Approximately 26 percent

Average Monthly Charges: Approximately 64.7

Total Revenue: Approximately 456K

Lost Revenue: Approximately 139K

Business Recommendations

Encourage customers to move from month-to-month contracts to long-term contracts

Promote bundled services to improve customer engagement

Incentivize automatic payment methods to reduce churn

Target high-risk segments with personalized retention campaigns

Repository Structure

Customer-Churn-Analysis-PowerBI/
Dataset/
customer_churn.csv
PowerBI/
Customer Churn Analysis.pbix
Screenshots/
customer_demographics.png
service_subscription.png
contract_billing.png
churn_drivers.png
README.md

Author

Manikanta Chundu
Data Analyst | Power BI | SQL | PythonHub profile links here
