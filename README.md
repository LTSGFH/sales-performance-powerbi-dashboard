# Sales Performance Dashboard (Power BI)

## Project Overview
This project analyzes customer insights, sales performance, and sales team performance using Power BI.  
The dashboard helps track revenue trends, customer distribution, and sales target achievement.

The goal of this report is to help business stakeholders understand:

• Customer distribution across countries  
• Sales performance trends over time  
• Sales team target achievements  
• Manager and team performance  

The report is built using Power BI with data modeling and DAX measures to generate business insights.

---

# Tools Used

- Power BI
- Excel
- DAX
- Data Modeling
- Data Visualization

---

# Dataset Description

The dataset contains three tables used to build the data model.

### Orders
Contains transaction-level order data.

Columns include:
- Order ID
- Order Datetime
- Order Value
- Order Source
- Sales POC

---

### Customers
Contains demographic information about customers.

Columns include:
- Customer ID
- Age
- Gender
- Country
- Customer Category

---

### Sales Targets
Contains sales targets assigned to each Sales POC.

Columns include:
- Sales POC
- Sales Manager
- Sales Team
- 2023 Sales Target

---

# Data Model

The dashboard uses a relational data model connecting the three tables.

Relationships:

Customers[Customer ID] → Orders[Customer ID]

Sales Targets[Sales POC] → Orders[Sales POC]

This structure allows sales performance to be analyzed by:

- Customer demographics
- Country
- Sales manager
- Sales team

---

# Dashboard Pages

## 1. Customer Insights

This page analyzes the customer base.

Key visuals include:

- Total Customers KPI
- Male vs Female distribution
- Country-wise customer distribution
- Customer age segmentation

This helps identify customer demographics and geographic distribution.

---

## 2. Sales Performance

This page focuses on sales metrics and order trends.

Key visuals include:

- Total Revenue KPI
- Total Orders KPI
- Highest Order Value KPI
- Monthly order trend
- Orders and Average Order Value by Country (Map)

This helps track sales trends and country-level performance.

---

## 3. Sales Team Performance

This page evaluates sales team performance against targets.

Key visuals include:

- Total Teams
- Total Managers
- Total Sales POC
- Best Team of the Year
- Target vs Achieved Sales Matrix
- Average Shortfall analysis
- Best Manager by Country

This helps understand team productivity and target completion.

---

# Key DAX Measures

Some of the key DAX measures used in the report:

Total Revenue
