
# ☕ Coffee Shop Sales Analysis
This project is an **end-to-end sales analysis system** for a coffee shop, designed to track and visualize key business metrics using **transactional sales data**, **optimized MySQL queries**, and an **interactive Power BI dashboard**.

It provides insights into:

* 📈 **Key Performance Indicators (KPIs)** like Total Sales, Total Orders, and Total Quantity Sold.
* 📊 Month-on-Month (MoM) comparisons and growth percentages.
* 🗓 Sales trends by day, week, and month.
* 🏆 Top products and category performance.
* 📍 Location-based sales performance.
* ⏰ Peak sales hours and weekday/weekend segmentation.


---

## 🛠 Tech Stack

* **Database**: MySQL
* **Data Visualization**: Power BI
* **Data Source**: Coffee shop transactional dataset (`Coffee Shop Sales.xlsx`)
* **Query Development**: SQL scripts (`MY SQL Queries.docx`)

---

## 📂 Project Structure

```
📁 Coffee-Shop-Sales-Analysis
│
├── 📄 Coffee Shop Sales.xlsx           # Raw transactional dataset
├── 📄 Coffee Shop Dashboard.pbix       # Power BI dashboard file
├── 📄 MY SQL Queries.docx              # MySQL queries for data cleaning & analysis
└── 📄 README.md                        # Project documentation
```

---

## 🔍 Data Preparation

Before analysis, the dataset was cleaned and transformed:

1. **Date & Time Conversion**

   * Converted `transaction_date` and `transaction_time` to proper `DATE` and `TIME` formats.
2. **Column Fixes**

   * Renamed incorrectly encoded column `ï»¿transaction_id` to `transaction_id`.
3. **Data Type Optimization**

   * Ensured all columns had correct data types for efficient querying.

---

## 📊 MySQL Analysis Queries

The SQL scripts include:

### **KPI Calculations**

* **Total Sales**
* **Total Orders**
* **Total Quantity Sold**
* **MoM Difference & Growth %** for all KPIs.

### **Sales Trends**

* Daily, weekly, and monthly trends.
* Above-average vs below-average daily sales.

### **Segmented Analysis**

* Weekday vs weekend performance.
* Sales by **store location**.
* Sales by **product category** and **top 10 products**.
* Hourly sales performance.

### **Advanced Insights**

* Calendar heatmap preparation (daily totals).
* Peak sales hour identification.
* Location-based ranking.

---

## 🚀 How to Use This Project

### **1️⃣ Setup MySQL Database**

```sql
-- Create table
CREATE TABLE coffee_shop_sales (
    transaction_id INT,
    transaction_date DATE,
    transaction_time TIME,
    store_location VARCHAR(50),
    product_category VARCHAR(50),
    product_type VARCHAR(50),
    unit_price DECIMAL(10,2),
    transaction_qty INT
);
```

* Import the data from `Coffee Shop Sales.xlsx` into the MySQL table.
* Run the SQL scripts from `MY SQL Queries.docx` for cleaning and analysis.

### **2️⃣ Open Power BI Dashboard**

* Open `Coffee Shop Dashboard.pbix` in **Power BI Desktop**.
* Connect it to your MySQL database.
* Refresh to see updated visuals.


---

## 📢 Conclusion

This project demonstrates how to:

* **Clean & prepare data** for business intelligence.
* **Write optimized SQL queries** for analytics.
* **Visualize insights** with Power BI for data-driven decision making.

It can be adapted for **any retail or service-based business** seeking actionable sales insights.

