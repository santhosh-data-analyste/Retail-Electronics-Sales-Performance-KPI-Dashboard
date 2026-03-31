

# 📊 Retail Electronics Sales Analytics Dashboard – KPI & Performance Insights (Power BI & SQL)

## 📖 Problem Statement
Retail businesses need a centralized system to monitor sales performance, track key performance indicators (KPIs), and identify product and regional trends.  
The objective of this project is to analyze retail electronics sales data and build an interactive dashboard that provides insights into revenue, product performance, and customer trends for better business decision-making.

---

## 📊 Dataset Information
- **Dataset Type:** Retail Electronics Sales Dataset  
- **Total Records:** 500+ transactions  
- **Key Columns:**  
  - Product Category (Phone, Laptop, Monitor, etc.)  
  - Customer Name  
  - Region (North, South, East, West)  
  - Sales Amount  
  - Quantity Sold  
  - Order Date  

- **Data Format:** SQL Database / CSV  
- **Data Process:** Extracted using SQL and transformed using Power BI Query Editor  

---

## 🛠 Tools Used
- **SQL** – Data extraction, aggregation (JOIN, GROUP BY)  
- **Power BI Desktop** – Dashboard development & visualization  
- **Power Query** – Data cleaning & transformation  
- **Data Visualization Techniques** – Bar Charts, Line Charts, KPI Cards, Slicers  

---

## 📈 Key Insights
- 📌 Total sales revenue exceeds **130K+** with over **600+ units sold**  
- 📌 Phones and laptops are the **top-performing product categories**  
- 📌 Regional analysis shows strong sales performance in selected zones  
- 📌 Customer-level insights highlight high-value customers contributing major revenue  
- 📌 Sales trends indicate variation across time and product categories  
- 📌 Interactive dashboard enables filtering by product, customer, and region  

---

## 🖥 Dashboard Screenshots
📌 Retail Electronics Sales Dashboard  

![Dashboard Screenshot](sales-dashboard.png)

---

## 🔹 Sample SQL Queries
```sql
-- Product-wise Sales
SELECT product, SUM(sales_amount) AS total_sales
FROM sales_data
GROUP BY product;

-- Region-wise Revenue
SELECT region, SUM(sales_amount) AS revenue
FROM sales_data
GROUP BY region;

-- Top Customers
SELECT customer_name, SUM(sales_amount) AS total_spent
FROM sales_data
GROUP BY customer_name
ORDER BY total_spent DESC;
