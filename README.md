# Customer Behavior Analysis: A Multi-Stage Data Engineering & Analytics Project

## Project Overview
This project provides a comprehensive analysis of customer shopping behavior by integrating **Python (Pandas)** for data cleaning and feature engineering, **SQL (PostgreSQL)** for complex analytical querying, and **Power BI** for interactive data visualization. The goal is to extract actionable insights into customer demographics, purchasing patterns, and revenue drivers.

---

## 🚀 Workflow

### 1. Data Cleaning & Feature Engineering (Python)
The initial raw dataset (`customer_shopping_behavior.csv`) was processed in a Jupyter Notebook (`customer_shopping_behaviour.ipynb`) using the following steps:
- **Standardization:** All column names were converted to `snake_case` for a clean, consistent coding experience.
- **Handling Missing Values:** Missing values in the `review_rating` column were handled using **median imputation** grouped by product category to maintain statistical integrity.
- **Feature Engineering:**
    - **Age Segmentation:** Used `pd.qcut` to divide the customer base into four distinct groups: *Young Adult, Adult, Middle-Aged,* and *Senior*.
    - **Frequency Mapping:** Categorical purchase frequencies (e.g., Weekly, Monthly) were mapped to numerical days (`purchase_frequency_days`) for easier analysis.
- **ETL:** The cleaned and transformed data was programmatically exported to a **PostgreSQL** database named `customer_behaviour`.

### 2. Analytical Querying (SQL)
With the data structured in PostgreSQL, ten key business questions were addressed in `sql_queries_customer_behaviour_key_findings.sql`. Highlights include:
- **Revenue Drivers:** Analysis of revenue contribution by gender and age group.
- **Customer Segmentation:** Classification of customers into *New, Returning,* and *Loyal* based on purchase history.
- **Product Performance:** Identifying top-performing products by category and highest review ratings.
- **Discount Impact:** Measuring the adoption rate of discounts and their relationship with high-spending behavior.

### 3. Interactive Visualization (Power BI)
The final phase involved building an **"Awesome Dashboard"** in Power BI (`customer_behavior.pbix`). This dashboard provides:
- **Key Performance Indicators (KPIs):** Real-time tracking of total revenue, average spend, and customer counts.
- **Demographic Slicers:** Interactive filtering by gender, age group, and location.
- **Trend Analysis:** Visualizing purchasing frequency and category preferences.

![Power BI Dashboard Preview](Screenshot%202026-02-23%20013725.png)

---

## 📂 Project Structure
```text
customer-behaviour/
├── customer_shopping_behavior.csv         # Raw Dataset
├── customer_shopping_behaviour.ipynb     # Python Cleaning & ETL Script
├── sql_queries_customer_behaviour_key_findings.sql # SQL Analysis
├── customer_behavior.pbix                 # Power BI Dashboard
├── Customer_Behavior_Analysis_Report.docx # Comprehensive Project Report
└── README.md                              # Project Documentation
```

---

## 🛠️ Tech Stack
- **Languages:** Python (Pandas, SQLAlchemy, Psycopg2), SQL (PostgreSQL)
- **Tools:** Jupyter Notebook, Power BI, Microsoft Word (for reporting)
- **Environment:** Windows 10/11

## 📈 Key Insights
*Detailed findings from the SQL queries and Power BI dashboard can be found in the `Customer_Behavior_Analysis_Report.docx` file.*

---
**Author:** [Ishtiaque Ahmed](https://github.com/mashroorzisan)  
**Date:** February 2026
