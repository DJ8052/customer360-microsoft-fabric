# Customer 360 Analytics Platform with Microsoft Fabric

## Project Overview

This project demonstrates an end-to-end **Customer 360 analytics platform** built using **Microsoft Fabric**, **Apache Spark**, **Delta Lake**, and **Power BI**.

The solution integrates customer, order, payment, support, and web activity data into a unified analytics platform that provides a consolidated customer view for business reporting and decision-making.

Using the Medallion Architecture (Bronze → Silver → Gold), the project transforms raw operational data into analytics-ready datasets that support marketing, customer service, finance, and executive reporting.

---

# Business Problem

Organizations often store customer information across multiple operational systems.

Customer orders, payments, support activity, and web interactions frequently exist in separate datasets, making it difficult to answer important business questions such as:

* Who are our most valuable customers?
* Which customers are at risk of churn?
* What purchasing behaviors are emerging?
* How effective are our payment channels?
* Which customer segments require additional attention?

This project demonstrates how Microsoft Fabric can consolidate multiple customer-related datasets into a unified Customer 360 analytical model.

---

# Solution Architecture

```text
Operational Source Files
(Customer, Orders, Payments,
Support, Web Activity)
            │
            ▼
Microsoft Fabric Lakehouse
            │
            ▼
Bronze Layer
(Raw Data)
            │
            ▼
Silver Layer
(Data Cleansing & Standardization)
            │
            ▼
Gold Layer
(Customer 360 Analytics Model)
            │
            ▼
Warehouse / SQL Endpoint
            │
            ▼
Semantic Model
            │
            ▼
Power BI Executive Dashboard
```

---

# Microsoft Fabric Components

This solution demonstrates several Microsoft Fabric capabilities working together.

### Data Storage

* Microsoft Fabric Lakehouse
* Delta Lake

### Data Engineering

* Apache Spark Notebooks
* PySpark transformations
* Silver-layer data cleansing
* Data validation

### Analytics

* Warehouse
* SQL Analytics Endpoint
* Semantic Model
* Power BI

### Orchestration

* Microsoft Fabric Data Pipeline
* Pipeline execution monitoring

---

# Data Engineering Workflow

The platform follows a modern Medallion Architecture.

1. Load raw customer datasets into the Lakehouse.
2. Store raw data within the Bronze layer.
3. Cleanse and standardize customer data in the Silver layer.
4. Validate transformed data through quality checks.
5. Publish business-ready Customer 360 datasets in the Gold layer.
6. Expose curated data through the SQL Endpoint and Semantic Model.
7. Deliver business insights through Power BI.

---

# Data Validation

The project includes dedicated data validation steps to improve data quality before reporting.

Validation includes checks such as:

* Row counts
* Duplicate records
* Missing values
* Data consistency

Separating validation from transformation reflects a production-minded analytics engineering workflow.

---

# Business Insights

The Customer 360 model supports reporting across several business domains.

### Customer Analytics

* Total Active Customers
* Customer Segmentation
* Customer Activity

### Sales Analytics

* Average Order Value (AOV)
* Repeat Customer Percentage
* Revenue Trends

### Customer Service

* Open Support Tickets
* Service Activity

### Customer Behavior

* Device Preferences
* Payment Method Distribution
* Churn Risk Indicators

---

# Technologies Used

* Microsoft Fabric
* Apache Spark
* PySpark
* Delta Lake
* Microsoft Fabric Lakehouse
* Warehouse
* SQL Analytics Endpoint
* Microsoft Fabric Data Pipeline
* Power BI

---

# Skills Demonstrated

This repository demonstrates experience with:

* Microsoft Fabric
* Medallion Architecture
* Lakehouse architecture
* Apache Spark
* PySpark
* Delta Lake
* Data engineering
* Data validation
* Analytics engineering
* Customer analytics
* SQL analytics
* Power BI dashboard development

---

# Business Value

This project demonstrates how organizations can transform disconnected operational data into a unified Customer 360 platform that supports:

* Customer segmentation
* Executive reporting
* Marketing analytics
* Customer service analytics
* Revenue analysis
* Churn identification
* Data-driven decision-making

Although this project uses sample customer datasets, the architecture can be adapted to enterprise CRM, ERP, and customer engagement platforms.

---

# Lessons Learned

This project reinforced several analytics engineering principles.

* Separate raw and curated data through the Medallion Architecture.
* Perform data cleansing before downstream analytics.
* Validate data quality before publishing analytical datasets.
* Centralize customer information into a unified business model.
* Design analytics platforms that support multiple downstream reporting tools.

---

# Repository Structure

```text
README.md

nb-silver-data-cleaning.ipynb
nb-data-validation-checks.ipynb

Fabric Lakehouse.png
Fabric Warehouse.png
Fabric SQL Endpoint with Query And Output.png
Fabric Data Pipeline.png
Fabric Pipeline History.png
Power BI Table View.png
ECommerce Power BI Report.png
```

---

# Author

**Devon Johnson**

This repository is part of my Microsoft Fabric and Analytics Engineering portfolio and demonstrates an end-to-end Customer 360 analytics solution using Microsoft Fabric, Apache Spark, Delta Lake, and Power BI.
