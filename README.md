Retail Sales Performance Dashboard
Project Overview

The Retail Sales Performance Dashboard is a Business Intelligence project developed using Microsoft Power BI. The objective of this project is to analyze retail sales data and provide insights into sales performance, product profitability, regional distribution, and customer behavior.

The dashboard helps stakeholders monitor key business metrics such as total sales, profit margins, customer segments, and product performance. By using data modeling and DAX calculations, the dashboard transforms raw transactional data into meaningful insights that support strategic decision-making.

Objectives of the Project
The main objectives of this project are:
Analyze overall sales performance
Understand profitability across products and categories
Identify top-performing products
Analyze regional sales distribution
Understand customer segments and purchasing behavior
Monitor sales growth trends over time

Tools and Technologies Used

Microsoft Power BI – Data visualization and dashboard creation
DAX (Data Analysis Expressions) – Used for calculated columns and measures
Data Modeling – Creating relationships between tables
CSV Datasets – Used as the source data

Dataset Description
The project uses a retail dataset consisting of four tables.

1. Sales Table
This table contains transaction-level data.
Columns:

Order Id
Order Date
Customer ID
Product Id
Region
Quantity
Unit Price
Cost
Return Flag
This table acts as the Fact Table in the data model.

2. Customers Table
This table contains customer-related information.

Columns:
Customer ID
Customer Name
City
Segment
Customer segmentation helps analyze purchasing behavior across different groups.

3. Products Table

This table contains product details.
Columns:
ProductID
Product Name
Category
This table is used to analyze product and category-level sales performance.

4. Date Table

This table is used for time-based analysis.
Columns:
Date
Year
Month
Quarter
The date table enables time intelligence functions such as YTD, YoY growth, and rolling calculations.

Data Modeling
A Star Schema data model was implemented in Power BI.
The Sales table acts as the central fact table, while Customers, Products, and Date tables act as dimension tables.

Relationships created:
Customers Table (1) → Sales Table ()
Products Table (1) → Sales Table ()
Date Table (1) → Sales Table (*)

This data modeling approach improves query performance and ensures efficient filtering across visuals.

Calculated Columns
Several calculated columns were created using DAX to derive additional information from the dataset.

Total Sales
Calculates revenue generated per transaction.
Total Sales = Quantity × Unit Price

Profit
Calculates profit per transaction.
Profit = Total Sales − Cost

Profit Category
Classifies transactions into profit groups.
High Profit → Profit greater than threshold
Low Profit → Profit below threshold

These columns allow deeper analysis of transaction profitability.

Measures Created (DAX)
Measures were created to calculate aggregated metrics across the dataset.

Total Sales
Calculates total revenue generated.

Total Profit
Calculates overall profit.
Profit Percentage
Shows profit as a percentage of total sales.
Sales YTD (Year-To-Date)
Calculates cumulative sales for the current year.
Sales LY (Last Year)
Calculates sales from the previous year.
YoY Growth Percentage
Shows growth rate compared to the previous year.
Running Total
Calculates cumulative sales over time.

These measures form the core KPIs used in the dashboard.

Advanced Measures
Advanced analytical measures were implemented to enhance insights.
Rolling 12 Months Sales
Tracks sales performance over the previous 12 months.
Contribution Percentage by Product
Calculates how much each product contributes to total sales.
Average Order Value
Calculates average revenue per order.
Average Order Value = Total Sales / Number of Orders

Repeat Customers
Identifies customers who placed multiple orders.
These advanced measures help understand customer loyalty and long-term sales trends.

Dashboard Structure

The dashboard consists of three interactive pages.

Page 1 – Executive Sales Overview
This page provides a high-level summary of business performance.
Visualizations included:
Total Sales KPI Card
Total Profit KPI Card
Profit Percentage KPI Card
YoY Growth KPI Card
Sales Trend Line Chart
Sales by Region Column Chart

Purpose:
Provide executives with a quick overview of business performance.

Page 2 – Product Performance Analysis

This page focuses on analyzing product-level performance.

Visualizations included:
Top 5 Products by Sales
Category vs Sales Matrix
Profit by Category Column Chart
Purpose:
Identify best-performing products and profitable categories.

Page 3 – Customer Insights Dashboard

This page focuses on customer analysis.
Visualizations included:
Sales by Customer Segment (Pie Chart)
Top Customers Table
Customer Growth Trend (Line Chart)

Purpose:
Understand customer behavior and segmentation.

Dashboard Features

The dashboard includes several interactive features:
Slicers for filtering data by Year
Slicers for filtering by Category
Slicers for filtering by Customer Segment
Dynamic visuals that update automatically when filters are applied
This allows users to perform interactive analysis.

Business Insights

The dashboard helps identify:
Regions generating the highest sales
Products contributing the most revenue
Categories generating maximum profit
Customer segments that drive sales growth
Sales trends across time periods
These insights can help businesses improve marketing strategies, optimize product offerings, and increase profitability.

Conclusion
The Retail Sales Performance Dashboard demonstrates how Business Intelligence tools like Power BI can transform raw data into actionable insights.
By using data modeling, DAX calculations, and interactive visualizations, this dashboard provides a comprehensive overview of sales performance, product profitability, and customer behavior.
This project showcases the practical use of Power BI for data-driven decision making in retail businesses.
