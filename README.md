Power BI Customer Churn Analysis

This project focuses on analyzing customer churn behavior for a telecom company using Power BI to answer real-world business questions related to customer demographics, service subscriptions, contract types, billing methods, and revenue impact.

The project demonstrates end-to-end Power BI analytics skills, including data cleaning, data modeling, DAX-based calculations, and interactive dashboard development for business decision-making.

Skills Demonstrated

Data cleaning and transformation using Power Query

Data modeling with relationships and star-schema concepts

Creation of calculated columns and measures using DAX

KPI development for churn and revenue analysis

Customer segmentation and risk analysis

Business-focused dashboard design and storytelling

Project Structure
customer-churn-analysis-powerbi/
│
├── Dataset/
│   └── customer_churn.csv
│
├── PowerBI/
│   └── Customer Churn Analysis.pbix
│
├── Screenshots/
│   ├── customer_demographics.png
│   ├── service_subscription.png
│   ├── contract_billing.png
│   └── churn_drivers.png
│
└── README.md

Data Preparation Approach

Raw customer churn data was imported from a CSV file into Power BI.

Data cleaning and transformation were performed using Power Query, including:

Handling missing and inconsistent values

Data type corrections

Feature standardization for analysis

A structured data model was created with calculated columns and measures using DAX.

This approach reflects real-world BI workflows where raw business data is transformed into analytics-ready datasets.

Business Questions Answered

What is the overall customer churn rate?

How does churn vary across different tenure segments?

Which customer demographics are more likely to churn?

How do service subscriptions impact churn behavior?

Which contract types and payment methods show higher churn?

What is the revenue impact of churned versus retained customers?

Which customer segments represent the highest churn risk?

Dashboard Pages and Insights
Customer Demographics Analysis

Analyzes churn across gender, senior citizen status, and tenure

Identifies higher churn concentration in low-tenure customers

Highlights trends between tenure and monthly charges

Service Subscription Analysis

Evaluates churn by internet service type

Analyzes impact of add-on services on churn

Shows relationship between service count and churn likelihood

Contract and Billing Insights

Compares churn rates across contract types

Analyzes payment method behavior

Highlights tenure distribution by contract category

Churn Drivers and Revenue Impact

Displays overall churn rate

Identifies high-risk customer segments

Quantifies revenue lost due to churn versus retained revenue

DAX Calculations Used

The project includes custom DAX calculated columns and measures, such as:

Tenure segmentation (6-bucket and 12-bucket models)

Service count per customer

Total customers and churned customers

Churn rate calculation

Lost revenue and retained revenue measures

Churn risk categorization

These calculations enable deeper analytical insights beyond basic visual reporting.

Key KPIs

Total Customers: 7,043

Churned Customers: Approximately 1,869

Churn Rate: Approximately 26 percent

Average Monthly Charges: Approximately 64.7

Total Revenue: Approximately 456K

Lost Revenue Due to Churn: Approximately 139K

Business Impact and Insights

Month-to-month contract customers exhibit the highest churn

Low-tenure customers are at the greatest risk of churn

Fiber optic service users show higher churn compared to other services

Churn leads to significant revenue loss, indicating strong retention opportunities

How to Run the Project

Download the .pbix file from the PowerBI/ folder

Open the file using Power BI Desktop

Load or refresh the dataset if required

Use slicers and filters to explore insights interactively

Tools Used

Power BI Desktop

Power Query

DAX (Data Analysis Expressions)

CSV dataset

Author

Manikanta Chundu
Data Analyst | Power BI | SQL | Python
