# 📊 Sales Analytics Report

## 📌 Overview
This project analyzes sales data to identify trends, top-performing regions, and customer behavior using SQL and Power BI.

## 🎯 Objectives
- Analyze total revenue and sales performance
- Identify top regions and customers
- Track monthly sales trends
- Support data-driven business decisions

## 🧰 Tools Used
- SQL (MySQL)
- Power BI
- Microsoft Excel

## 📊 Dataset
The dataset contains:
- Order ID
- Order Date
- Region
- Category
- Sales
- Customer Name

## 💻 SQL Analysis

### 1. Total Revenue
```sql
SELECT SUM(sales) AS total_revenue
FROM sales_data;

### 2. Sales by Region
SELECT region, SUM(sales) AS revenue
FROM sales_data
GROUP BY region
ORDER BY revenue DESC;

### 3. Monthly Sales Trend
SELECT 
    DATE_FORMAT(order_date, '%Y-%m') AS month,
    SUM(sales) AS monthly_sales
FROM sales_data
GROUP BY month
ORDER BY month;
