# 🍕 Pizza Sales Analysis Dashboard – Power BI + SQL

An interactive dashboard to analyze pizza sales performance using *Power BI* for visualization and *SQL* for backend data processing.  
The goal is to provide insights into revenue, order trends, pizza category performance, and customer behavior.

---

## 📊 Dashboard Features

- ✅ Total Revenue, Average Order Value
- ✅ Total Pizzas Sold, Total Orders
- ✅ Daily & Monthly Order Trends
- ✅ Sales by Pizza Category & Size
- ✅ KPI Cards with DAX Measures
- ✅ Clean, interactive visuals with slicers

---

## 🛠 Tools Used

- *Power BI* – Reports, Dashboards, DAX
- *SQL* – KPI Calculations, Data Cleaning
- *DAX* – Measures & Calculated Columns
- *Excel* – For raw dataset overview

---

## 🗃 Dataset Overview

Sample dataset includes:
- order_id, order_date, pizza_id, size, category, quantity, total_price

📝 Dummy dataset created for practice and demonstration.

---

## 🧠 SQL Queries Used

```sql
-- 1. Total Revenue
SELECT SUM(total_price) AS Total_Revenue FROM pizza_sales;

-- 2. Average Order Value
SELECT SUM(total_price) / COUNT(DISTINCT order_id) AS Avg_order_Value FROM pizza_sales;

-- 3. Total Pizzas Sold
SELECT SUM(quantity) AS Total_pizza_sold FROM pizza_sales;

-- 4. Total Orders
SELECT COUNT(DISTINCT order_id) AS Total_Orders FROM pizza_sales;
