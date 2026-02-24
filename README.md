Customer Retention Dashboard – KPI & Business Insights
Project Overview

This project demonstrates how a Business Analyst supports executive reporting through KPI analysis and dashboard design focused on customer retention metrics.

The objective was to identify churn trends and improve retention performance.

Business Problem

The company observed declining customer retention rates over two quarters.

Leadership required a dashboard to monitor churn rate, revenue impact, and customer segmentation trends.

Dataset Overview

The dataset included:

Customer ID

Subscription Type

Monthly Revenue

Churn Status

Region

Signup Date

Key KPIs Defined

Customer Retention Rate

Churn Rate

Revenue by Subscription Type

Monthly Recurring Revenue (MRR)

Regional Customer Distribution

Analysis Approach

Validated customer records using SQL

Cleaned and transformed data using Python (Pandas)

Aggregated KPI metrics

Designed dashboard structure for executive reporting

Business Insights Identified

Higher churn observed in basic subscription tier

Revenue impact concentrated in two regions

Customers with lower engagement showed higher churn probability

Outcome

Provided leadership with structured KPI dashboard enabling data-driven retention strategy decisions.

Tools Used

SQL

Python (Pandas)

Power BI / Tableau

Excel
-- Calculate churn rate
SELECT 
  (SUM(CASE WHEN ChurnStatus = 'Yes' THEN 1 ELSE 0 END) * 100.0 / COUNT(*)) AS ChurnRate
FROM customer_data;
