# 📊 E-Commerce Performance & Sales Analytics Dashboard

An interactive, end-to-end **Power BI** dashboard designed to evaluate e-commerce store performance, monitor sales trajectories, track order lifecycles, and analyze customer behaviors to drive data-driven decision-making.

---

## 📌 Project Overview

This project transforms multi-dimensional retail and e-commerce transactional data into actionable business intelligence. The interactive report enables stakeholders to track primary key performance indicators (KPIs), evaluate product catalog health, uncover regional revenue patterns, and analyze customer acquisition and retention.

---

## 📑 Dashboard Architecture & Pages

The dashboard is structured into targeted analytical views based on the reporting layers:

1. **Executive Overview (eCommerce Hub):**
   * High-level summary of total revenue, order volume, and Average Order Value (AOV).
   * Revenue trends over time with dynamic period-over-period performance comparisons.

2. **Sales Performance:**
   * Revenue and profit breakdown across product categories and sub-categories.
   * Identification of top-performing items and underperforming product lines.
   * Regional and channel-level revenue distribution.

3. **Orders & Operations Analysis:**
   * Order volume tracking across daily, monthly, and seasonal cycles.
   * Fulfillment efficiency, shipping distribution, and order status tracking.
   * Return and cancellation rate monitoring.

4. **Customer Insights:**
   * Customer segmentation based on purchase frequency and Customer Lifetime Value (CLV).
   * New vs. returning customer trends and repeat purchase behavior.

---

## 🛠️ Tools & Technical Workflow

* **Microsoft Power BI Desktop:** Interactive visualization design, layout modeling, and dashboard publication.
* **Power Query:** Data extraction, transformations, cleaning, and schema structuring (ETL).
* **Data Modeling:** Optimized Star Schema architecture linking transactional fact tables with dedicated dimension tables (Date, Customers, Products, Regions).
* **DAX (Data Analysis Expressions):** Custom measures, time-intelligence calculations, and analytical indicators.

---

## 💡 Key DAX Measures

dax
// Total Sales Revenue
Total Sales = SUM(Sales[SalesAmount])

// Distinct Order Volume
Total Orders = DISTINCTCOUNT(Orders[OrderID])

// Average Order Value (AOV)
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Author
Marwan Hamdy Alsweny - Data Analyst





// Total Unique Customers
Total Customers = DISTINCTCOUNT(Customers[CustomerID])
