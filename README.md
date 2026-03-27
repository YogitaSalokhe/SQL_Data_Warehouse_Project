
# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository! 🚀  
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

---

🧠 Business Problem

A vehicle company collects data from multiple systems such as ERP (sales, products) and CRM (customers).

However, the data is:
- Fragmented across systems
- Not cleaned or standardized
- Not optimized for analysis

This makes it difficult to:
- Track product performance
- Identify high-value customers
- Analyze sales trends
- Make data-driven decisions

----

##  🎯 Objective

To build a centralized data warehouse and analytics solution that:
1. Integrates ERP and CRM data
2. Cleans and standardizes raw data
3. Provides a unified data model for analysis
4. Enables customer and product insights
5. Supports business decision-making

---
## 🏗️ Data Architecture

The data architecture for this project follows Medallion Architecture **Bronze**, **Silver**, and **Gold** layers:
1. **Bronze Layer**: Stores raw data as-is from the source systems. Data is ingested from CSV Files into SQL Server Database.
2. **Silver Layer**: This layer includes Data cleansing and transformation, Handling missing values and inconsistencies, Standardization and normalization to prepare data for analysis.
3. **Gold Layer**: Houses business-ready data modeled into a star schema(Fact & Dimension tables) Optimized for analytical queries and reporting.

---
## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports and dashboards for actionable insights.

----

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

### BI: Analytics & Reporting (Data Analysis)

#### Objective
Develop SQL-based analytics to deliver detailed insights into:
- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

----

## 📈 Analytics & Reporting
📦 Product Report

Purpose: Analyze product performance and behavior

Key Metrics:
Total Orders,
Total Sales,
Total Quantity Sold,
Unique Customers,
Product Lifespan

KPIs:
Recency (months since last sale),
Average Order Revenue (AOR),
Average Monthly Revenue

Insights:
Identifies high-performing and low-performing products
Highlights revenue contribution by product category

## 👥 Customer Report

Purpose: Understand customer behavior and segmentation

Key Metrics:
Total Orders,
Total Sales,
Total Quantity Purchased,
Total Products Purchased,
Customer Lifespan

KPIs:
Recency (months since last order)
Average Order Value (AOV)
Average Monthly Spend

Segmentation:
VIP Customers (high value, long-term),
Regular Customers,
New Customers

## 🔍 Advanced Analytics
📅 Time-Based Analysis: 
Monthly and yearly sales trends
Seasonal performance insights

📊 Cumulative Analysis:
Running total of sales over time

📉 Performance Analysis:
Year-over-year product performance comparison
Comparison against average sales

🧩 Data Segmentation:
Product segmentation based on cost ranges
Customer segmentation based on spending behavior

🧮 Part-to-Whole Analysis:
Contribution of each product category (Bikes, Clothing, Accessories) to total revenue

📈 Key Insights:
- A small percentage of customers (VIP segment) contribute a significant share of total revenue
- Bike category generates the highest revenue 96.46% compared to Clothing and Accessories
- Certain products show low recency, indicating potential decline in demand
- Sales trends reveal seasonal patterns across months
- Customer segmentation helps identify high-value and at-risk customers
  
----

##🛠️ Tools & Technologies
- SQL Server
- T-SQL
- Data Warehousing Concepts
- ETL Pipelines
- Star Schema Modeling

These insights empower stakeholders with key business metrics, enabling strategic decision-making.  

## 📂 Repository Structure
```
data-warehouse-project/
│
├── datasets/                           # Raw datasets used for the project (ERP and CRM data)
│
├── docs/                              # Project documentation and architecture details
│   ├── data_architecture1.drawio      # Draw.io file shows the project's architecture
│   ├── data_catalog.md                # Catalog of datasets, including field descriptions and metadata
│   ├── Data Flow.drawio               # Draw.io file for the data flow diagram
│   ├── Data Model.drawio              # Draw.io file for data models (star schema)
│   ├── Data Integration.drawio        # Shows how tables are connected
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/                         # Scripts for extracting and loading raw data
│   ├── silver/                         # Scripts for cleaning and transforming data
│   ├── gold/                           # Scripts for creating analytical models
│   
├── tests/                              # Test scripts and quality files
│
├── README.md                           # Project overview and instructions
