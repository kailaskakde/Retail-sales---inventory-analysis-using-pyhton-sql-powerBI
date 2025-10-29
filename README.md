
# 🏬 Retail Sales & Inventory Analysis – Using Python, SQL & Power BI

---

## 📘 **Brief One-Line Summary**
A complete end-to-end data analytics project analyzing **retail sales and inventory performance** using **Python, SQL, and Power BI** to optimize stock levels and understand customer demand.

---

## 🧭 **Overview**
This project demonstrates how retail data can be transformed into **actionable business insights** by combining:
- **Data Extraction (SQL)**
- **Data Cleaning & Transformation (Python)**
- **Visualization & Insights (Power BI)**

It focuses on analyzing **sales performance, inventory health, and demand trends** to assist management in making smarter decisions about stock, supply, and revenue strategy.

---

## ❓ **Problem Statement**
Retail businesses often face challenges like:
- Over- or under-stocking of items  
- Poor visibility into product performance  
- Lack of data-driven insights for sales optimization  

This project resolves those challenges by building an **interactive Power BI dashboard** showing:
- 📈 Sales by region, product, and category  
- 📦 Inventory quantity and out-of-stock items  
- 🗓️ Monthly sales and stock movement  
- 💰 Revenue and demand correlation  

---

## 🧩 **Dataset**
| Dataset Name | Description |
|---------------|-------------|
| `retail_sales.csv` | Contains sales transactions with date, product, region, and revenue. |
| `inventory_data.csv` | Contains product inventory levels, quantity sold, and stock information. |

---

## 🧠 **Tools and Technologies**
- 🐍 **Python (Pandas, NumPy, Matplotlib)** – Data cleaning, analysis, and transformation  
- 🗄️ **MySQL** – Querying and structuring sales and inventory data  
- 📊 **Power BI Desktop** – Data modeling and visualization dashboard  
- ⚙️ **Power Query** – Data extraction and ETL pipeline setup  

---

## ⚙️ **Project Workflow**
1. **Data Extraction:**  
   - Pulled retail sales and inventory data from MySQL.  

2. **Data Cleaning & Transformation (Python):**  
   - Used Pandas for removing null values and aggregating key metrics.  
   - Exported cleaned data into CSV for Power BI connection.  

3. **Dashboard Creation (Power BI):**  
   - Built relationships between Sales and Inventory tables.  
   - Designed interactive visuals with slicers for product, region, and month.  

4. **Insight Generation:**  
   - Combined inventory and sales KPIs for actionable business metrics.  

---

## 📊 **Dashboard Preview**

### 📦 Page 1 – Inventory Management by Stocks  
**Objective:** Track inventory quantity, daily sales, and out-of-stock items.  

**Visuals Included:**  
- Total Stock Sold & Inventory KPI cards  
- Bar Chart – Inventory Quantity by Category  
- Line Chart – Inventory Trends by Month  
- Region-wise Stock Distribution  
- Product Table – Current Stock Levels  

**Screenshot:**  
![Inventory Dashboard](https://github.com/kailaskakde/Retail-Sales-and-Inventory-Analysis-using-Python-SQL-PowerBI/blob/main/Screenshots/inventory_page.png)

---

### 💹 Page 2 – Sales Performance Overview  
**Objective:** Evaluate total sales, profit, and regional contribution.  

**Visuals Included:**  
- KPI Cards – Total Sales, Profit, Margin %  
- Monthly Sales Trend Line  
- Category-wise Revenue Bar Chart  
- Region-wise Performance Comparison  
- Filters for Product, Month, and Region  

**Screenshot:**  
![Sales Dashboard](https://github.com/kailaskakde/Retail-Sales-and-Inventory-Analysis-using-Python-SQL-PowerBI/blob/main/Screenshots/sales_page.png)

---

## 🧮 **Key Python & SQL Components**

### 🔹 Python Code
python
# Load and clean data
import pandas as pd

# Load datasets
sales = pd.read_csv('retail_sales.csv')
inventory = pd.read_csv('inventory_data.csv')

# Merge and aggregate data
merged = pd.merge(sales, inventory, on='product_id')
summary = merged.groupby('category')[['sales', 'inventory_qty']].sum().reset_index()

# Export cleaned dataset
summary.to_csv('cleaned_retail_data.csv', index=False)

