🔹 Calculated Columns
1. Tenure – 12 Month Segments

Explanation:
Segments customers into detailed 12-month tenure buckets to analyze churn behavior across different customer lifecycle stages.
```bash
Tenure_12Segments =
SWITCH(
    TRUE(),
    Customer[tenure] <= 6, "0–6",
    Customer[tenure] <= 12, "7–12",
    Customer[tenure] <= 18, "13–18",
    Customer[tenure] <= 24, "19–24",
    Customer[tenure] <= 30, "25–30",
    Customer[tenure] <= 36, "31–36",
    Customer[tenure] <= 48, "37–48",
    Customer[tenure] <= 60, "49–60",
    Customer[tenure] <= 66, "61–66",
    "67–72"
)
```
2. Tenure – 6 Month Segments

Explanation:
Creates simplified tenure risk buckets used for churn prediction and high-level segmentation.
```bash
Tenure_6Segments =
SWITCH(
    TRUE(),
    Customer[tenure] <= 12, "0–12",
    Customer[tenure] <= 24, "13–24",
    Customer[tenure] <= 36, "25–36",
    Customer[tenure] <= 48, "37–48",
    Customer[tenure] <= 60, "49–60",
    "61–72"
)
```
3. Service Count

Explanation:
Counts the total number of active services subscribed by each customer to measure engagement level.
```bash
Service_Count =
INT(Customer[PhoneService] = "Yes") +
INT(Customer[InternetService] <> "No") +
INT(Customer[OnlineSecurity] = "Yes") +
INT(Customer[OnlineBackup] = "Yes") +
INT(Customer[DeviceProtection] = "Yes") +
INT(Customer[TechSupport] = "Yes") +
INT(Customer[StreamingTV] = "Yes") +
INT(Customer[StreamingMovies] = "Yes")
```
🔹 Measures (DAX Measures)
4. Total Customers

Explanation:
Calculates the total number of unique customers in the dataset.
```bash
Total Customers =
DISTINCTCOUNT(Customer[customerID])
```
5. Churned Customers

Explanation:
Counts customers who have discontinued the service.
```bash
Churned Customers =
CALCULATE(
    [Total Customers],
    Customer[Churn] = "Yes"
)
```
6. Churn Rate (%)

Explanation:
Measures the percentage of customers who churned.
```bash
Churn Rate =
DIVIDE(
    [Churned Customers],
    [Total Customers]
)
```
7. Average Monthly Charges

Explanation:
Calculates the average monthly billing amount per customer.
```bash
Avg Monthly Charges =
AVERAGE(Customer[MonthlyCharges])
```
8. Total Revenue

Explanation:
Calculates total revenue generated from all customers.
```bash
Total Revenue =
SUM(Customer[TotalCharges])
```
9. Lost Revenue (Churned Customers)

Explanation:
Calculates total revenue lost due to customer churn.
```bash
Lost Revenue =
CALCULATE(
    [Total Revenue],
    Customer[Churn] = "Yes"
)
```
10. Retained Revenue

Explanation:
Calculates revenue retained from active (non-churned) customers.
```bash
Retained Revenue =
CALCULATE(
    [Total Revenue],
    Customer[Churn] = "No"
)
```
11. Churn Risk Bucket

Explanation:
Classifies customers into churn risk categories based on churn rate thresholds.
```bash
Churn Risk Bucket =
SWITCH(
    TRUE(),
    [Churn Rate] >= 0.40, "High",
    [Churn Rate] >= 0.25, "Medium",
    "Low"
)
```
