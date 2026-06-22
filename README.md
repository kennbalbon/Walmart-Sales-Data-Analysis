# 🛒 Walmart Retail Data Pipeline & Analysis

## 📌 Project Overview
This project is an end-to-end data analytics pipeline designed to extract business intelligence from raw retail data. Using the Kaggle Walmart Sales dataset, the project demonstrates enterprise-level data cleaning, standardization, and advanced Exploratory Data Analysis (EDA) within a MySQL database. The optimized SQL queries were deployed as database Views and directly integrated into Microsoft Power BI to generate interactive, executive-ready dashboards.

## 🛠️ Tech Stack
* **Database:** MySQL (Data cleansing, standardizing, staging)
* **Data Manipulation:** Advanced SQL (CTEs, Window Functions, Conditional Aggregation, NTILE)
* **Business Intelligence:** Microsoft Power BI (Direct Query/Views integration, Dashboarding)
* **Data Source:** [Walmart Sales Dataset (Kaggle)](https://www.kaggle.com/datasets/mikhail1681/walmart-sales)

## 📊 Key Business Insights Extracted
Through rigorous SQL querying, the following core business questions were answered mathematically before being visualized:
1. **Sales Performance:** Identified the Top 5 and Bottom 5 performing store locations by average weekly revenue.
2. **Seasonal Trends:** Proved an 8.5% revenue lift during holiday weeks and accurately mapped Month-over-Month (MoM) and Year-over-Year (YoY) growth, highlighting major Q4 spikes.
3. **Macroeconomic Sensitivity:** Created an **Efficiency Index** to prove that prolonged periods of high unemployment (>10%) mathematically suppress earning potential.
   * Analyzed the impact of fuel prices and Consumer Price Index (CPI) inflation on total sales volume by grouping raw continuous data into standardized quartiles and brackets.

## 📁 Repository Structure
* `walmart_sales_data_analysis.sql` - The complete SQL script containing data cleaning commands, table alterations, and the advanced queries/Views used for the EDA.
* `Walmart_Sales.csv` - The original raw dataset.
* `Walmart_Sales_Dashboard.pbix` - The final interactive dashboard file.

## 🚀 How to Replicate
1. Ensure you have **MySQL** and **Power BI Desktop** installed.
2. Download the `Walmart_Sales.csv` file and import it into a new MySQL database named `walmart_sales`.
3. Run the `walmart_sales_data_analysis.sql` script in your SQL editor. This will automatically clean the data, standardize the date formats, and generate the reporting Views.
4. Open Power BI Desktop, select **Get Data -> MySQL database**, and connect directly to the generated Views (e.g., `vw_store_performance_rankings`) to begin visualizing!
