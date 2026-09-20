# Credit_Card_Dashboard
Credit Card Weekly Status Dashboard
📊 Overview

This project is an end-to-end Power BI dashboard that tracks weekly credit card performance metrics, giving stakeholders real-time visibility into revenue, transactions, and customer behavior. It covers the full analytics pipeline — from raw CSV data to a live, interactive dashboard.

🎯 Objective

To build a comprehensive weekly reporting dashboard that surfaces key performance metrics and trends in credit card operations, enabling stakeholders to monitor business health and make data-driven decisions on a rolling weekly basis.

🛠️ Tech Stack
SQL — data storage and querying
Excel/CSV — source data preparation
Power BI — data modeling, DAX, and dashboard visualization
🔄 Workflow

1. Data Preparation
Raw transaction and customer data was cleaned and structured into CSV files for import.

2. SQL Database Setup

Created relational tables to hold customer details (cust_detail) and credit card transaction data (cc_detail)
Imported CSV data into the SQL database using bulk COPY operations
Structured the database to support efficient querying and joins between customer and transaction tables

3. Power BI Data Modeling & DAX
Connected Power BI directly to the SQL database and built custom DAX measures and calculated columns, including:

Segmentation columns — AgeGroup and IncomeGroup, bucketing customers into meaningful ranges (e.g., income tiers: Low/Med/High) using SWITCH(TRUE()) logic
Revenue measure — combining annual fees, transaction amount, and interest earned into a single unified revenue metric
Week-over-week comparison measures — Current_week_Revenue and Previous_week_Revenue, calculated via CALCULATE + FILTER against a custom week_num2 column (derived using WEEKNUM)

4. Dashboard Development
Built an interactive dashboard visualizing weekly and YTD performance, with drill-downs by customer demographics, card category, and geography.

5. Insights & Reporting
The dashboard automatically surfaces WoW (week-over-week) changes and YTD summaries for stakeholder review.

📈 Key Insights (Sample — Week 53)
WoW Revenue Growth: +28.8%
YTD Overall Revenue: $57M
YTD Total Interest Earned: $8M
YTD Total Transaction Amount: $46M
Revenue by Gender: Male customers contributed $31M vs. $26M from female customers
Card Mix: Blue & Silver cards accounted for 93% of overall transactions
Top Geographies: TX, NY, and CA contributed 68% of total activity
Card Activation Rate: 57.5%
Delinquency Rate: 6.06%
✅ Key Skills Demonstrated
SQL database design and data import
Data modeling and DAX (SWITCH, CALCULATE, FILTER, time intelligence)
Interactive Power BI dashboard design
KPI definition and trend/WoW analysis
Translating raw transactional data into business insights


dashboard credit card transaction report
https://github.com/kc8249754-sudo/Credit_Card_Dashboard/commit/1d9ef8763213e6004953f02d0d4a0eb1abec9fa1
