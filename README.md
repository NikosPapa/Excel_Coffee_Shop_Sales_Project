# Excel_Coffee_Shop_Sales_Project

## Project Overview

This project analyzes transactional sales data from a **fictitious coffee shop in New York City** using **Microsoft Excel**. The goal is to clean, prepare, and analyze sales records in order to uncover revenue trends, customer purchasing behavior, and product performance. The final deliverable is an **interactive Excel dashboard** built with PivotTables, PivotCharts, and slicers to support dynamic exploration of the data.

---

## Dataset

An existing fictional dataset was used for this project.

**Coffee Shop Sales Dataset**
- Transaction-level records from a coffee shop in NYC  
- **149,116 records** and **11 fields**

### Raw Data Fields
- `transaction_id`  
- `transaction_date`  
- `transaction_time`  
- `transaction_qty`  
- `store_id`  
- `store_location`  
- `product_id`  
- `unit_price`  
- `product_category`  
- `product_type`  
- `product_detail`  

---

## Project Scope

- Data inspection and basic quality assurance.  
- Data cleaning and transformation in Excel.  
- Feature engineering (calculated date and time fields).  
- Exploratory data analysis (EDA) using PivotTables.
- Interactive dashboard creation using PivotCharts and slicers.

---

## Data Cleaning & Preparation

Data preparation included:

- Validation of record counts and field completeness.  
- Verification of data types for dates, times, quantities, and prices.  
- Creation of calculated fields to support time-based and revenue analysis.  

### Calculated Columns

The following columns were added to enhance analysis:

- **Revenue** – calculated as `unit_price × transaction_qty`  
- **Month** – extracted from `transaction_date`  
- **Day of Week** – derived from `transaction_date`  
- **Hour of Day** – extracted from `transaction_time`  

These fields enabled efficient aggregation and time-based exploration of sales trends.

---

## Exploratory Data Analysis (EDA)

### Revenue by Month
A PivotTable was created to aggregate total revenue by month, allowing for the identification of overall revenue trends and seasonal patterns.

### Transactions by Day of Week
A PivotTable was used to analyze transaction volume by day of week, highlighting differences in customer activity between weekdays and weekends.

### Transactions by Hour of Day
Hourly transaction analysis revealed peak purchasing periods throughout the day, helping identify the most operationally critical hours.

### Transactions by Product Category
Transaction counts were summarized by product category and sorted in descending order to determine which categories contribute the most to overall sales volume.

### Top 15 Product Types
A PivotTable was created to display the **Top 15 product types** based on transaction count, along with their associated revenue. This view helps identify best-selling products and supports inventory and menu optimization decisions.

---

## Dashboard Development

The dashboard was assembled using PivotCharts and organized into a single, cohesive layout.

### Visualizations Included
- **Line Chart:** Revenue by Month  
- **Column Charts:**  
  - Transactions by Day of Week  
  - Transactions by Hour of Day  
- **Bar Chart:** Transactions by Product Category  

### Interactivity
- A **store location slicer** was added and connected to all PivotTables and charts  
- The slicer allows users to filter results by location or view performance across **all locations simultaneously**

<p align="center">
  <img width="554" height="225" alt="Dashboard" src="https://github.com/user-attachments/assets/35253a97-d63c-404e-97f1-86ffc8c4273b" />
</p>

---

## Conclusion

This interactive Excel dashboard provides a comprehensive view of coffee shop sales performance across **all store locations** in New York City. By transforming transaction-level data into analysis-ready features and leveraging PivotTables, PivotCharts, and slicers, the project uncovers meaningful patterns in revenue trends, customer behavior, and product performance.

Revenue demonstrates a steady upward trend across the observed months, indicating increasing customer demand and overall business growth. Transaction activity varies by day of week, with weekdays, particularly later in the workweek, showing slightly higher volumes than weekends, suggesting a strong commuter-driven customer base.

Hourly transaction analysis highlights a clear concentration of sales during morning hours, consistent with typical coffee consumption habits. Activity gradually declines as the day progresses.

From a product perspective, Coffee and Tea categories dominate transaction volume, while a relatively small group of product types accounts for a large share of both transactions and revenue. These insights can inform decisions related to product focus, inventory planning, and promotional strategy.

Overall, this project demonstrates how Microsoft Excel can be effectively used to clean, analyze, and visualize large transactional datasets, transforming raw sales data into actionable business insights through an intuitive and interactive dashboard.
