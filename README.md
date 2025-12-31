# Customer 360 Analytics Platform (Microsoft Fabric)

## Overview
This project demonstrates an end-to-end Customer 360 analytics solution built using Microsoft Fabric.
It integrates customer, order, payment, support, and web activity data into a unified analytics layer
to support marketing, customer service, and leadership decision-making.

## Architecture
- Azure Data Lake Storage Gen2 (source)
- Microsoft Fabric Lakehouse
- Medallion Architecture (Bronze / Silver / Gold)
- PySpark for transformation
- Power BI for reporting

## Data Flow
CSV Sources → Bronze (Parquet + Delta)
→ Silver (Cleaned & Normalized)
→ Gold (Star Schema + Customer 360 Summary)
→ Power BI Semantic Model & Report

## Key KPIs
- Total Active Customers
- Average Order Value (AOV)
- Repeat Customer %
- Open Support Ticket Count
- Churn Risk Indicator
- Payment Method Split
- Device Preference Trends

## Tools Used
- Microsoft Fabric
- PySpark
- Delta Lake
- Power BI
