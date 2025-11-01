# Comprehensive E-commerce Sales Analysis (1M+ Transactions)

This project is an end-to-end analysis of a large-scale e-commerce dataset (**1 million transactions**) using **Power BI**. The goal was to clean, model, and visualize the data to extract deep, actionable insights across multiple business dimensions (Customers, Products, Time, and Geography).

---

## 🎯 Project Objective

* To handle and process a large dataset efficiently.
* To build a robust and scalable data model (Star Schema).
* To create a comprehensive, multi-page dashboard for stakeholders.
* To answer complex business questions related to customer loyalty, product performance, sales growth, and regional focus.

---

## 🛠️ Data Preparation & Modeling

1.  **Data Cleaning:** The dataset was thoroughly cleaned to handle null values, remove duplicates, and correct data types before analysis.
2.  **Data Modeling (Star Schema):** A robust **Star Schema** was implemented, which is crucial for performance when dealing with large datasets. The model consists of:
    * **1 Fact Table:** `fact_table` (containing 1M+ transactions).
    * **5 Dimension Tables:** `customer_dim`, `item_dim`, `store_dim`, `time_dim`, and a payment dimension.
    This model simplifies queries and significantly improves report performance.

---

## 📊 Dashboard & Key Insights

The final report is a 6-page interactive dashboard:

### 1. Overview Page
* **KPIs:** Displays high-level metrics: **Total Sales (~105.40M)**, **Total Transactions (1M)**, **Quantity Sold (~6M)**, and **Unique Customers (~9.2K)**.
* **Visuals:** Includes sales trends over time, sales by payment method, and bar charts for Top 5 Products and Top 5 Regions.

### 2. Customer Analysis Page
* **Loyalty Metrics:** Uses **DAX** and **Bookmarks** to compare `New Customers` vs. `Repeat Customers` and the `Repeat Rate` on a yearly basis.
* **Segmentation:** Customers are segmented (e.g., **Gold, Silver, Bronze**) using DAX. A matrix visual details the count, total sales, and avg. spending for each segment.
* **Top Customers:** Identifies the **Top 10 Customers** by total sales.

### 3. Product Analysis Page
* **Product Performance:** Identifies top products and categories by sales and quantity.
* **Pareto Analysis:** A Pareto chart demonstrates the 80/20 rule, showing which categories contribute most to cumulative sales.

### 4. Time Intelligence Page
* **Advanced DAX:** This page heavily features advanced time-based metrics, including **Sales YOY%** (Year-over-Year), **Sales QOQ%** (Quarter-over-Quarter), and **Sales MoM%** (Month-over-Month).
* **Comparative Visuals:** Line and clustered column charts compare current sales/quantity against the previous period.

### 5. Geographic Analysis Page
* **Regional Performance:** Identifies the **Top Region** and **Top District** by sales.
* **Interactive Map:** A map visual allows for **drill-down** analysis from `Region` > `District` > `Local Area`, showing detailed KPIs at each level.

### 6. Payment Analysis Page
* **Payment Trends:** Analyzes the frequency, total sales, and avg. transaction value for each payment method (e.g., Cash on Delivery, Mobile Banking, Credit Card) over time.

---

## 🔧 Technologies Used
* **Power BI**
* **DAX:** For advanced calculations (Time Intelligence, Customer Segmentation).
* **Data Modeling:** Star Schema implementation.
* **Power Query (M Language):** For data cleaning and pre-processing.
