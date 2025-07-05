# Data Portfolio: Excel to Power BI




# Table of contents

- [Project Overview](#project-overview)
  - [Objective](#objective)
  - [Business Context](#business-context)
- [Data Collection](#data-collection)
  - [Source](#source)
  - [Structure & Format](#structure-&-format)
- [Data Cleaning & Preparation](#data-cleaning-&-preparation)
  - [Data Types & Formatting](#data-types-&-formatting)
- [SQL Analysis](#dsql-analysis)
  - [Business Questions Answered](#business-questioned-answered)
- [Data Modeling](#data-modeling)
  - [Star Schema Design](#star-schema-design)
  - [Table Relationships](#table-relationships)
- [DAX Calculations](#dax-calculations)
  - [Core Measures](#core-measures)
  - [Time Intelligence](#time-inteligence)
- [Dashboard Design](#dashboard-design)
  - [Visuals Used](#visuals-used)
- [Key Insights](#key-insghts)
  - [Trends Identified](#trends-identified)
  - [Recommendations](#recommendations)

# Project Overview
## Objective
The objective of this project is to develop a dynamic and interactive Power BI dashboard that analyses Superstore sales performance across key business dimensions — including sales, profitability, operations, and product-level insights. This dashboard is designed to support real-time decision-making by providing drill-down capabilities and intuitive visualisations tailored for the Regional Sales Director and other stakeholders.
## Business Context
The organisation currently relies on static, Excel-based reports that are time-consuming to update and offer limited visibility into trends and inefficiencies. As a result, business leaders struggle to:
 - Identify underperforming products or regions in a timely manner
 - Detect profit leaks caused by high discounting or returns
 - Understand seasonal or regional sales trends
 - Optimise operations such as shipping performance and order efficiency

This project addresses those challenges by transforming raw sales data into actionable insights through a clean, easy-to-use dashboard that delivers value across sales, operations, and profitability


# Data Collection
## Source
The dataset used for this project is the publicly available Superstore Sales dataset, which simulates a retail company’s historical order data. It contains detailed transactional information on customer orders, product categories, shipping performance, and regional sales.
## Structure & Format
The data was provided in Excel format and included the following key fields:
 - Order Details: Order ID, Order Date, Ship Date, Customer ID, Segment, Region
 - Product Info: Product Name, Category, Sub-Category
 - Sales Metrics: Sales, Quantity, Discount, Profit
 - Shipping Metrics: Shipping Mode, Ship Date, Order Priority

This raw dataset was first analysed in SQL to answer business questions and then imported into Power BI for further cleaning, modeling, and visualisation.

# Data Cleaning & Preparation
## Data Types & Formatting
Data cleaning was performed in Microsoft Excel before importing the dataset into PostgreSQL. The following steps were taken to ensure consistency and accuracy:
 - Converted Order Date and Ship Date columns into proper date formats
 - Verified that numeric columns such as Sales, Profit, Discount, and Quantity were correctly typed as numbers
 - Standardized text formatting for categorical fields like Region, Segment, Category, and Sub-Category (e.g., removing extra spaces and fixing case mismatches)
## Handling Missing or Duplicate
  - Scanned the dataset for blank cells and filled or removed non-critical ones as appropriate
  - Removed duplicate rows based on Order ID to ensure each transaction was unique
  - Cleaned inconsistent values in fields such as Product Name and Region to prevent grouping errors in Power BI
  - After cleaning, the Excel file was saved as a structured dataset and imported into PostgreSQL for analysis

# SQL Analysis
## Business Questions Answered
Before importing the dataset into Power BI, exploratory data analysis was performed in SQL to answer key business questions such as:
 - How have monthly sales changed across different regions?
 - What is the total profit by product category and region?
 - Which products rank highest in sales and lowest in profit?
 - How do discounts above 20% affect profitability?
 - Which consumer segment drives the most revenue?
 - Which region shows consistent YoY growth?
















