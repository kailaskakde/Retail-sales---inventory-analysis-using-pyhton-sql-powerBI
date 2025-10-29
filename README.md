# 🛒 Store Sales & Customer Behavior Analysis Dashboard  

---

## 📘 **Brief One-Line Summary**
A Power BI dashboard analyzing store sales trends and customer behavior to uncover key business insights.

---

## 🧭 **Overview**
This project explores how sales and customer data can be transformed into actionable insights using Power BI.  
It provides visual analytics on sales performance, customer demographics, and profitability to support data-driven decision-making.

---

## ❓ **Problem Statement**
Businesses often struggle to understand **what drives their sales performance** and **how customers behave** across products and regions.  
This project aims to solve that by visualizing critical KPIs such as:
- Total Revenue and Profit
- Top Products and Categories
- Customer Retention and Repeat Behavior
- Profit Margin and Regional Trends

---

## 🧩 **Dataset**
| Dataset Name | Description |
|---------------|-------------|
| `Sales_Data.xlsx` | Order details including product, region, revenue, and profit. |
| `Customer_Data.xlsx` | Customer demographics, purchase frequency, and type (New/Returning). |

---

## 🧠 **Tools and Technologies**
- **Power BI Desktop** – Dashboard design and data visualization  
- **Power Query** – Data cleaning and transformation  
- **DAX (Data Analysis Expressions)** – KPI calculations  
- **Excel/CSV** – Raw data source  

---

## ⚙️ **Methods**
1. Imported sales and customer datasets into Power BI.  
2. Cleaned and transformed data using Power Query.  
3. Built relationships between tables (Sales ↔ Customer).  
4. Created DAX measures for Revenue, Profit, and Margins.  
5. Designed interactive visuals with filters, slicers, and drill-throughs.  

---

## 🔑 **Key Insights**
- 📈 Clothing and Electronics are the top-performing categories.  
- 🌍 East region generated the highest sales revenue.  
- 👥 Equal distribution between new and returning customers (50%-50%).  
- 💰 Top 10 customers account for the majority of total revenue.  
- 🧾 August marked the highest monthly sales (₹8.9M).  

---

## 📊 **Dashboard / Model / Output**

### 🏠 Page 1 – Sales Overview  
**Objective:** Analyze sales performance and profitability by category and region.  

**Visuals Included:**
- Total Orders, Quantity, Revenue, Profit, Margin KPIs  
- Donut Chart → Revenue by Category  
- Line Chart → Revenue & Profit Trends by Month  
- Bar Chart → Revenue by Region  
- Filters → Category, Product, Location  

**Screenshot:**  
![Sales Page](sales%20page.png)

---

### 👥 Page 2 – Customer Insights  
**Objective:** Understand customer retention and identify top spenders.  

**Visuals Included:**
- Total Orders, Quantity, Revenue, Profit, Margin KPIs  
- Donut Chart → New vs Returning Customers  
- Bar Chart → Top 10 Customers by Revenue  
- Matrix Table → Customer Type by Gender  
- Filters → Region, Product, Category  

**Screenshot:**  
![Customer Page](customers%20page.png)

---

## 🧮 **Key DAX Formulas**
DAX
Total Revenue = SUM(Sales[Revenue])
Total Profit = SUM(Sales[Profit])
Profit Margin % = DIVIDE([Total Profit], [Total Revenue], 0)
Total Orders = COUNTROWS(Sales)
Total Quantity = SUM(Sales[Quantity])

---

## 🧰 **How to Run This Project**
1. Download or clone this repository.
2. Open the `.pbix` file → `store sales and customer behavior.pbix` in **Power BI Desktop**.
3. Refresh data connections if needed.
4. Use slicers and filters for dynamic analysis.

---

## 🏁 **Results & Conclusion**
- Power BI dashboards deliver quick visibility into performance metrics.  
- Businesses can identify top customers and optimize category-level strategies.  
- Monthly and regional analysis helps align future marketing and inventory decisions.  

---

## 🔮 **Future Work**
- Integrate real-time sales data from SQL Server or APIs.  
- Add predictive analytics for future sales forecasting.  
- Expand the dashboard with customer lifetime value (CLV) metrics.  

---

## 👤 **Author & Contact**
**Kailas Kakde**  
📊 *Data Analyst | Power BI | SQL | Python | Excel*  

📧 **Email:** [your-email@example.com]  
🌐 **LinkedIn:** [linkedin.com/in/kailaskakde](https://linkedin.com/in/kailaskakde)  

🏷️ *Tags:* `#PowerBI` `#SalesDashboard` `#CustomerAnalysis` `#DataAnalytics`  

---

© 2025 Kailas Kakde | All Rights Reserved
