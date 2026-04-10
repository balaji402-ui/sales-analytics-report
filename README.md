# 📊 Sales Data Analysis

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Tools](https://img.shields.io/badge/Tools-SQL%20%7C%20Excel%20%7C%20Power%20BI-blue)
![Made With](https://img.shields.io/badge/Made%20With-ChatGPT%20%7C%20GitHub-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📌 Overview

> A end-to-end sales data analysis project using **SQL**, **Excel**, and **Power BI** to uncover revenue trends, top customers, and country-level performance.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| ![SQL](https://img.shields.io/badge/SQL-Database%20Queries-informational) | Data extraction & aggregation |
| ![Excel](https://img.shields.io/badge/Excel-Data%20Cleaning-success) | Data cleaning & preparation |
| ![Power BI](https://img.shields.io/badge/Power%20BI-Visualization-yellow) | Dashboard & visual reporting |
| ![ChatGPT](https://img.shields.io/badge/ChatGPT-AI%20Assistance-blueviolet) | Insight generation |
| ![GitHub](https://img.shields.io/badge/GitHub-Version%20Control-black) | Project management |

---

## 🎯 Objective

Analyze sales data to:
- ✅ Identify **top-performing countries** by revenue
- ✅ Discover **monthly sales trends**
- ✅ Find **top customers** driving the most sales
- ✅ Generate **actionable business insights**

---

## 💻 SQL Queries

### 🔹 Total Sales by Country
```sql
SELECT country, SUM(sales) AS total_sales
FROM sales_data
GROUP BY country
ORDER BY total_sales DESC;
```

### 🔹 Top 5 Customers
```sql
SELECT customer_name, SUM(sales) AS total_spent
FROM sales_data
GROUP BY customer_name
ORDER BY total_spent DESC
LIMIT 5;
```

### 🔹 Monthly Sales Trend
```sql
SELECT MONTH(order_date) AS month,
       SUM(sales) AS monthly_sales
FROM sales_data
GROUP BY month
ORDER BY month;
```

---

## 🔍 Key Insights

| # | Insight |
|---|---------|
| 1 | 🌍 Top 3 countries contribute over **60% of total revenue** |
| 2 | 📈 Sales peak during **Q4 (October–December)** |
| 3 | 👤 Top 5 customers account for **30% of all sales** |
| 4 | 📉 Lowest sales observed in **Q1 (January–March)** |

---

## 📁 Project Structure

```
sales-data-analysis/
│
├── 📄 README.md          # Project documentation
├── 📂 data/
│   └── sales_data.csv    # Raw sales dataset
├── 📂 sql/
│   └── queries.sql       # All SQL queries used
├── 📂 excel/
│   └── cleaned_data.xlsx # Cleaned data file
└── 📂 dashboard/
    └── sales_report.pbix # Power BI dashboard file
```

---

## 🚀 Conclusion

This project demonstrates how **SQL + Excel + Power BI + ChatGPT** can be combined to:
- Clean and query raw sales data
- Build interactive dashboards
- Generate meaningful business insights

---

## 🙋 Author

**Balaji Shashank**
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/balaji402-ui)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com/in/balaji-shashank-k-074755366)

---

⭐ *If you found this project helpful, please give it a star!*
