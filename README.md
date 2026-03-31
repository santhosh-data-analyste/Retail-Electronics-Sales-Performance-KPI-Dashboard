# 📊 Retail Electronics Sales Performance & KPI Dashboard

## 🔹 Project Overview
This project presents an interactive **Retail Electronics Sales Dashboard** built using **Power BI**, with data extracted and processed using **SQL**. The dashboard provides insights into sales performance, product trends, and key business metrics through dynamic visualizations.

---

## 🔹 Objectives
- Track key sales KPIs such as revenue, quantity, and performance  
- Analyze product-wise and region-wise sales trends  
- Identify top-performing products and customers  
- Enable data-driven decision-making through interactive reporting  

---

## 🔹 Tools & Technologies
- **SQL** – Data extraction, transformation, and aggregation  
- **Power BI** – Dashboard development and visualization  
- **Power Query** – Data cleaning and preprocessing  
- **DAX** – KPI calculations and measures  

---

## 🔹 Key Features
- 📌 KPI Cards (Total Sales, Quantity, Revenue)  
- 📌 Product-wise performance (Phones, Laptops, etc.)  
- 📌 Region-wise sales trend analysis  
- 📌 Customer-level insights  
- 📌 Interactive slicers and filters  

---

## 🔹 Data Processing
- Extracted data using **SQL queries (JOIN, GROUP BY, aggregations)**  
- Cleaned and transformed data using **Power Query**  
- Created calculated measures using **DAX**  

---

## 🔹 Sample SQL Queries

```sql
-- Product-wise Sales
SELECT product, SUM(sales_amount) AS total_sales
FROM sales_data
GROUP BY product;

-- Region-wise Sales
SELECT region, SUM(sales_amount) AS revenue
FROM sales_data
GROUP BY region;

-- Top Customers
SELECT customer_name, SUM(sales_amount) AS total_spent
FROM sales_data
GROUP BY customer_name
ORDER BY total_spent DESC;
