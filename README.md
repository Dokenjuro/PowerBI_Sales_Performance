📊 Power BI Sales Performance Dashboard

**Author:** Chiedozie Charles Chigboh  
**Email:** [chigboh@gmail.com](mailto:chigboh@gmail.com)  
**GitHub:** [github.com/dokenjuro](https://github.com/dokenjuro)  
**Role Focus:** Business Analyst | Data-Driven Decision Support | AI & Analytics Enthusiast

---

## 📘 Project Overview

This project demonstrates end-to-end data modeling and visualization using Power BI, connected directly to a SQLite database via ODBC.  
It’s part of my Business Analytics & Data Portfolio, showing how I transform raw relational data into actionable business insights.

The dataset represents a fictional retail company’s customer and sales data, including:

- Customer demographics (region, join date)
- Sales transactions (product, quantity, price)
- Derived business metrics such as revenue growth, product performance, and customer acquisition.

## 🧩 Objectives

- Connect Power BI to SQLite using an ODBC data source.
- Build an interactive two-page dashboard for executive and analytical insights.
- Develop DAX measures for key performance metrics.
- Visualize sales trends, growth performance, and acquisition dynamics.
- Add slicers for Year, Region, and Product for flexible filtering.

---

## 🧠 Key Insights

From 206 transactions across 50 customers (2021–2024):

| Metric                        |      Result |
| ----------------------------- | ----------: |
| **Total Revenue**             | $105,648.94 |
| **Total Orders**              |         206 |
| **Unique Customers**          |          50 |
| **Average Order Value (AOV)** |     $512.86 |
| **Top Product**               |      Laptop |
| **Top Region**                |        West |

---

### Insight Summary:
- Revenue steadily grew from 2021 to 2023, peaking in 2023 before slightly slowing in 2024.
- Customer growth followed a similar upward trend, showing strong acquisition in the early years.

---

## 📊 Dashboard Pages

| Page  | Title                         | Description                                                                                                     |
| ----- | ----------------------------- | --------------------------------------------------------------------------------------------------------------- |
| **1** | **Executive Overview**        | Displays total revenue, orders, AOV, and customer count, with visuals for top regions, products, and customers. |
| **2** | **Revenue & Growth Insights** | Focuses on YoY revenue growth, product revenue, and monthly customer acquisition, filtered by region.           |

---

## 🖼️ Visualizations

| Insight                             | Visualization Type       |
| ----------------------------------- | ------------------------ |
| **Total Revenue by Product**        | Column Chart             |
| **Year-over-Year Revenue Growth %** | Combo Chart (Bar + Line) |
| **Total Customers by Year**         | Column Chart             |
| **Monthly New Customers**           | Line Chart               |
| **Top 10 Customers by Revenue**     | Bar Chart                |
| **Revenue by Region**               | Bar Chart                |
| **Monthly Revenue Trend**           | Line Chart               |
| **KPIs (AOV, Orders, Revenue)**     | Card Visuals             |


The final dashboard is available as both a .pbix file and a sales_performance_overview.pdf for presentation.

---

## ⚙️ Tools & Technologies
| Category            | Tools Used                                         |
| ------------------- | -------------------------------------------------- |
| **BI Tool**         | Power BI Desktop                                   |
| **Database**        | SQLite (`Granger_Analytics_DB.db`)                 |
| **Connection**      | ODBC (System DSN: `Granger_Analytics_DB`)          |
| **Modeling**        | One-to-Many: `customers → sales` via `customer_id` |
| **Language**        | DAX                                                |
| **Version Control** | Git + GitHub                                       |

---

## 🧰 File Structure

```bash
Granger_Analytics/
├── Portfolio/
│   ├── PowerBI_Sales_Performance/
│   │   ├── sales_performance.pbix               # Power BI dashboard
│   │   ├── sales_performance_overview.pdf       # Exported visuals
│   │   ├── visuals/
│   │   │   ├── page1.png                        # Executive Overview
│   │   │   └── page2.png                        # Growth Insights
│   │   └── README.md                            # This file
```
---

## 🧾 Methodology

**Data Integration:**
- Connected Power BI directly to the SQLite database using ODBC.
- Imported customers and sales tables, linked via customer_id.


**DAX Measures Created:**
- Total Revenue = SUM(sales[price] * sales[quantity])
- Average Order Value (AOV) = DIVIDE([Total Revenue], [Total Orders])
- YoY Revenue Growth % = (CurrentYear - PreviousYear) / PreviousYear

**Visualization Design:**
- Developed 8 visuals across two pages for balanced storytelling.
- Included slicers for Region, Product, and Year.
- Applied consistent color palette and KPI layout for executive readability.

**Export & Documentation:**
- Dashboard exported to PDF and integrated into GitHub documentation.

---

## 🚀 How to Reproduce

1. Clone this repository:

```bash
  git clone https://github.com/dokenjuro/Granger_Analytics.git
  cd Granger_Analytics/Portfolio/PowerBI_Sales_Performance
```
2. Open the Power BI file:
```bash
  sales_performance.pbix
```
3. Update the ODBC connection if needed:

- System DSN: Granger_Analytics_DB
- Database path: C:\Users\HP\Granger_Analytics_DB.db

4. Refresh the dataset and explore the visuals interactively

---

*💡 Future Improvements*

- Automate data refresh using Power BI Gateway.

- Add Customer Lifetime Value (CLV) and churn metrics.

- Integrate Python scripts for forecasting and trend smoothing.

---

🏁 Outcome

This project demonstrates capability in business intelligence storytelling — connecting raw databases, modeling relationships, building analytical measures, and delivering interactive dashboards.
It bridges technical fluency with executive clarity, aligned with Business Analyst and BI Developer roles.

© 2025 — Chiedozie Chigboh | Business Analytics & AI Portfolio
