# 📊 Superstore Sales — Exploratory Data Analysis

An end-to-end **Exploratory Data Analysis (EDA)** of a nationwide retail "Superstore" dataset, built in Python using **Pandas**, **Seaborn**, and **Matplotlib**. The project cleans the raw sales data, engineers useful time-based features, and visualizes sales performance across categories, regions, customer segments, shipping modes, and time — surfacing insights that can support decisions in sales, marketing, and operations.

---

## 🎯 Business Objective

A nationwide retail company sells office supplies, furniture, and technology products through online and offline channels. The goal of this analysis is to uncover **actionable, data-driven insights** by:

- **Evaluating sales performance** across categories, segments, and regions
- **Analyzing trends & seasonality** in sales over months and years
- **Assessing operational efficiency** through shipping durations and methods
- **Exploring customer behavior** across segments
- **Identifying improvement areas** — underperforming products, regions, or segments

---

## 📁 Dataset Overview

| Detail | Value |
|---|---|
| Records | 9,788 orders |
| Features | 17 columns |
| Time span | Jan 2015 – Dec 2018 |
| Missing values | 0 |
| Duplicates | 0 |

**Key columns:** `Order_Date`, `Ship_Date`, `Ship_Mode`, `Segment`, `Region`, `State`, `Category`, `Sub_Category`, `Product_Name`, `Sales`.

---

## 🛠️ Tech Stack

- **Python 3**
- **Pandas** — data loading, cleaning, aggregation
- **Seaborn** & **Matplotlib** — data visualization
- **openpyxl** — reading the Excel source file
- **Jupyter Notebook** — analysis environment

---

## 🔄 Project Workflow

1. **Data Understanding** — inspected shape, data types, and summary statistics (`.info()`, `.describe()`).
2. **Data Cleaning** — checked for nulls and duplicates; converted `Order_Date` / `Ship_Date` to datetime and `Postal_Code` to a categorical type.
3. **Feature Engineering** — created three new features:
   - `Shipping_Duration` (days between order and shipment)
   - `Order_Year`
   - `Order_Month`
4. **Exploratory Data Analysis** — grouped and visualized sales across multiple dimensions.

---

## 📈 Key Insights

- **Total sales** across the period: **~$2.25 million**.
- **Technology** is the highest-grossing category (**~$826K**), narrowly ahead of **Furniture** (~$723K) and **Office Supplies** (~$703K).
- The **West** region leads in sales (~$710K), followed closely by the **East** (~$660K); the **South** lags behind (~$389K).
- The **Consumer** segment drives the majority of revenue (~$1.15M) — more than Corporate and Home Office combined.
- **Phones** and **Chairs** are the top-selling sub-categories.
- **Shipping duration** varies clearly by shipping mode, with same-day and first-class options being fastest — useful for logistics planning.
- Monthly sales show a **seasonal pattern**, with sales building toward the end of each year.

---

## 📊 Sample Visualizations

The notebook produces bar charts for:
- Sales by Category
- Sales by Region
- Sales by Segment
- Average Shipping Duration by Ship Mode
- Top 10 Sub-Categories by Sales
- Monthly Sales Trend over time

*(Run the notebook to generate the plots, or view them inline on GitHub.)*

