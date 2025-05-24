# 📊 Power BI Learning Guide

A complete hands-on guide and learning path demonstrating in-depth knowledge of Power BI through structured topics, examples, and real-world scenarios.

---

## ✅ 1. Getting Started with Power BI

### 🔹 Description:
Introduction to Power BI ecosystem including installation, UI (Data View, Model View, Report View), and types of tools.

### 🔹 Tools:
- Power BI Desktop
- Power BI Service
- Power BI Mobile
- Power BI Report Builder

### 🔹 Example:
- A business user pulls raw sales data and builds a report with tiles, charts, and dashboards for decision-making.

---

## ✅ 2. Get Data and Transform Data (Power Query Editor)

### 🔹 Description:
ETL process within Power BI using Power Query. Covers data sourcing, transformations, cleaning, and shaping.

### 🔹 Key Features:
- Merge & Append Queries
- Split Column, Fill Down/Up
- Pivot / Unpivot
- Replace & Clean / Trim
- Custom & Conditional Columns
- Creating Parameters

### 🔹 Example:
Append Excel files from a folder and clean up headers, nulls, and unnecessary columns. Use "Use First Row as Header" and "Remove Blank Rows".

---

## ✅ 3. Data Modeling in Power BI

### 🔹 Description:
Create relationships and define schema structures like Star and Snowflake. 

### 🔹 Concepts:
- Fact & Dimension Tables
- Relationships (One-to-Many, Many-to-Many, One-to-One)
- Filter Direction & Cardinality
- Composite Key & Bridge Table
- Granularity, OLAP vs OLTP

### 🔹 Example:
Create a Date Dimension table using:
```DAX
DimDate = CALENDAR(FIRSTDATE(Sales[Date]), LASTDATE(Sales[Date]))
```

---

## ✅ 4. Data Visualization

### 🔹 Description:
Building interactive and dynamic visuals using built-in and custom charts.

### 🔹 Visuals Covered:
- Table, Matrix
- Clustered Column, Stacked Bar
- Pie, Donut, Tree Map
- KPI Cards, Gauge, Waterfall, Maps
- Slicers, Tooltips, Bookmarks, Buttons

### 🔹 Example:
Use a bar chart to show Sales by Region with dynamic drilldown using a slicer.

---

## ✅ 5. Data Analysis Expressions (DAX)

### 🔹 Description:
Powerful expression language used to build logic in calculated columns, measures, and tables.

### 🔹 Categories:
- Aggregators: `SUM`, `AVERAGE`, `MAX`, `COUNT`
- Iterators: `SUMX`, `AVERAGEX`
- Logical: `IF`, `SWITCH`, `AND`, `OR`
- Text: `CONCATENATE`, `LEFT`, `RIGHT`, `LEN`
- Time Intelligence: `YTD`, `MTD`, `SAMEPERIODLASTYEAR`, `DATEADD`
- Ranking: `RANKX`, `TOPN`

### 🔹 Example:
```DAX
Profit Margin = DIVIDE([Profit], [Revenue], 0)
```
```DAX
Rank = RANKX(ALLSELECTED(Products), [TotalSales], , DESC, DENSE)
```

---

## ✅ 6. Power BI Service (Cloud)

### 🔹 Description:
Collaborate, publish and schedule reports online. Build dashboards and share insights across teams.

### 🔹 Features:
- Create Workspaces
- Publish PBIX files
- Row-Level Security
- Schedule Refresh & Gateway setup
- Mobile Layout Design

### 🔹 Example:
Publish a report to Power BI Service and configure 8-hour interval refresh with on-prem Gateway.

---

## ✅ 7. Interview Questions

### 🔹 Description:
Scenario and conceptual questions to prepare for job interviews.

### 🔹 Types:
- Difference between `CALCULATE` vs `CALCULATETABLE`
- Explain Fact vs Dimension table
- When to use `ALL` vs `ALLEXCEPT`

---

## ✅ 8. End-to-End Power BI Project

### 🔹 Description:
Build a complete BI solution for a sales domain with:
- Data ingestion (Excel/SQL)
- Clean-up using Power Query
- Dimensional modeling
- DAX calculations
- Reports, Drillthrough, Tooltips

### 🔹 Example Output:
KPI Card (Total Sales), Map (Sales by Region), Bar Chart (Monthly Sales Trend)

---

## 🟧 Advanced Topics to Explore Next

- Performance Analyzer & Optimization
- Power BI Deployment Pipelines
- Power Automate Integration
- Power BI Embedded for web apps
- Admin Portal, Audit Logs, and Tenant Settings
- Theme JSON & Branding
- Integration with Python, R, Azure ML

---
