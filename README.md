# Superstore-Sales-Analysis
End-to-End Sales Analysis using Excel, Oracle SQL and Power BI
# 📊 Superstore Sales Performance Dashboard

## 📌 Project Overview

This project analyzes Superstore sales data using Oracle SQL and Power BI. The objective is to identify sales trends, evaluate regional performance, analyze product categories, and build an interactive dashboard for business decision-making.

---

## 🛠️ Tools & Technologies

- Microsoft Excel
- Oracle SQL
- Microsoft Power BI
- GitHub

---

## 📂 Dataset

- Dataset: Superstore Sales Dataset
- Total Records: 9,800+
- Contains:
  - Customer Information
  - Product Details
  - Sales
  - Profit
  - Discount
  - Region
  - Order Date

## 🔄 Project Workflow

1. Collected the Superstore sales dataset in CSV format.
2. Imported the dataset into Oracle SQL.
3. Performed SQL analysis to calculate KPIs and business metrics.
4. Connected the processed data to Power BI.
5. Designed an interactive dashboard with KPIs, charts, and slicers.
6. Derived business insights to support decision-making.
---

## 📈 SQL Analysis Performed

The following analyses were performed using Oracle SQL:

- Total Sales
- Total Profit
- Total Orders
- Top 10 Products by Sales
- Region-wise Sales Analysis
- Region-wise Profit Analysis
- Category-wise Sales
- Category-wise Profit
- Monthly Sales Trend
- Profit Margin Calculation
- Average Discount Analysis

---
## 📝 Sample SQL Queries

### 1. Total Sales

```sql
SELECT SUM(sales) AS total_sales
FROM superstore;
```

### 2. Top 10 Products by Sales

```sql
SELECT product_name,
       SUM(sales) AS total_sales
FROM superstore
GROUP BY product_name
ORDER BY total_sales DESC
FETCH FIRST 10 ROWS ONLY;
```

### 3. Monthly Sales Trend

```sql
SELECT TO_CHAR(order_date, 'Mon YYYY') AS month,
       SUM(sales) AS total_sales
FROM superstore
GROUP BY TO_CHAR(order_date, 'Mon YYYY')
ORDER BY MIN(order_date);
```
## 📝 SQL Highlights

Some key SQL operations performed in this project include:

- Aggregate Functions (SUM, AVG, COUNT)
- GROUP BY and ORDER BY
- Top-N Analysis
- Profit Margin Calculation
- Monthly Sales Trend Analysis
- Regional Performance Analysis

---
## 📊 Dashboard Features

The Power BI dashboard includes:

- KPI Cards
  - Total Sales
  - Total Profit
  - Total Orders
  - Average Discount

- Visualizations
  - Monthly Sales Trend
  - Region-wise Sales vs Profit
  - Category-wise Sales
  - Top 10 Products

- Interactive Slicers
  - Region
  - Category
  - Segment
  - Year

---

## 📸 Dashboard Preview

![Dashboard](dashboard.png)

---

## 📁 Project Structure

```
Superstore-Sales-Analysis
│
├── README.md
├── dashboard.png
├── Superstore_Final.csv
├── final_projects1.sql
└── superstore_sale_dashboard.pbix
```

---

## 💡 Key Business Insights

- Technology was the highest-performing product category based on total sales.
- The West region consistently generated the highest revenue among all regions.
- Monthly sales trends indicate seasonal fluctuations in customer demand.
- A small group of top-selling products contributed a significant portion of overall revenue.
- Interactive filtering enables comparison across regions, categories, and customer segments for better business decisions.

---

## 📚 Key Learnings

Through this project, I gained hands-on experience in:

- Writing SQL queries for business analysis
- Performing KPI calculations
- Data visualization using Power BI
- Dashboard design and storytelling
- Converting raw data into actionable business insights

## 🚀 Future Improvements

- Add advanced SQL queries using Window Functions and CTEs.
- Publish the dashboard to Power BI Service.
- Include additional business KPIs and drill-through pages.
- Enhance dashboard with more interactive visualizations.

  
## 👨‍💻 Author

Rahul Gandhi

Aspiring Data Analyst

Skills:
- SQL
- Power BI
- Excel
- Python
