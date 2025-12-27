# 🍕 Pizza Sales Analysis Dashboard (Power BI)

## 📌 Project Overview
This project presents an **interactive sales analysis dashboard built entirely in Power BI** using a pizza sales dataset.  
The dashboard focuses on tracking business performance, identifying top-selling products, and understanding customer ordering patterns.

This project is designed to demonstrate **Power BI fundamentals**, including data modeling, DAX measures, and effective dashboard design.

---

## 🎯 Objectives
- Analyze overall sales performance
- Track key business KPIs
- Identify top-performing pizzas and categories
- Understand sales trends over time
- Support data-driven business decisions

---

## 🛠 Tools Used
- **Power BI Desktop**
- **Excel** (data source)
- **DAX** (Data Analysis Expressions)

---

## 📂 Dataset Information
**Dataset:** Pizza Sales Dataset (Excel)

**Key Columns:**
- `order_id`
- `order_date`
- `order_time`
- `pizza_name`
- `pizza_category`
- `pizza_size`
- `quantity`
- `total_price`

---

## 📊 Key KPIs
- **Total Revenue**
- **Total Orders**
- **Total Pizzas Sold**
- **Average Order Value (AOV)**

---

## 📈 Dashboard Visuals
The Power BI dashboard includes:

- **KPI Cards**
  - Total Revenue
  - Total Orders
  - Total Pizzas Sold
  - Average Order Value

- **Monthly Revenue Trend**
  - Line chart showing revenue changes over time

- **Revenue by Pizza Category**
  - Bar chart comparing category performance

- **Top 10 Pizzas by Revenue**
  - Bar chart with Top N filtering

- **Revenue by Pizza Size**
  - Donut chart showing size-wise contribution

---

## 🧮 DAX Measures Basic

Go to Modeling → New Measure

### Total Revenue
```DAX
Total Revenue = SUM(pizza_sales[total_price])
```

### Total Orders
```DAX
Total Orders = DISTINCTCOUNT(pizza_sales[order_id])
```

### Average Order Value
```DAX
Average Order Value = DIVIDE([Total Revenue], [Total Orders])
```
### Total Pizzas Sold
```DAX
Total Pizzas Sold = SUM(pizza_sales[quantity])
```
## create Date Helpers
### Order Year
```DAX
Order Year = YEAR(pizza_sales[order_date])
```
Order Month
```DAX
Order Month = FORMAT(pizza_sales[order_date], "MMM")
```

### 💡 Key Insights

- A small number of pizzas generate a large share of revenue
- Sales show clear monthly trends and seasonality
- Medium and Large pizza sizes contribute the most revenue
- Certain categories consistently outperform others

 ### 🚀 How to Use This Project

- Download the dataset and .pbix file
- Open the report using Power BI Desktop
- Explore visuals and interact with filters
- Review DAX measures to understand KPI calculations

### 📌 What This Project Demonstrates

- Power BI report building from scratch
- KPI development using DAX
- Data visualization best practices
- Business-focused analysis
- Beginner-to-intermediate Power BI skills










