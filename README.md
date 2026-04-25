# RAINBOW WORLD SALES PERFORMANCE DASHBOARD (2024)
## Introduction
This project analyzes the Rainbow World sales dataset for the year 2024 to evaluate overall sales performance, identify trends, and uncover key business insights.
The analysis focuses on understanding product performance, regional contributions, and seasonal sales patterns to support better decision-making and improve business growth.
## Problem Statement
Although the business recorded significant sales in 2024, there is a need to gain deeper insights into performance across products, regions, and time periods.
This analysis aims to answer the following key questions:
- Which product categories and products generate the most sales?
- Which regions contribute the highest and lowest revenue?
- How do sales vary across months and quarters?
- When do sales peak during the year?
- What opportunities exist to improve overall performance?
## Tools Used
This analysis was carried out using:
- Microsoft Excel
- Pivot Tables
- Pivot Charts
- Slicers
- Dashboard designs
## Dataset Description
Rainbow World Sales Dataset contained 3,355 rows and 10 columns, including:
- Order ID
- Order Date
- Customer ID
- Product Category
- Segment
- Region
- Category
- Quantity
- Product Cost
- Sales
These fields provide essential information for analyzing sales performance, customer behavior, and product trends.
## Data Cleaning & Preparation
During data inspection, several issues were identified and resolved:
- Incorrect data formats in Order Date, Quantity, Product Cost, and Sales
- Inconsistent text formatting (case sensitivity and extra spaces) in Product Category and Region
- 54 duplicate rows based on Order ID
- 10 missing values in the Segment column
- Product Cost stored as text due to the inclusion of the "$" symbol
- Missing values in Product Cost and Sales columns
### Actions Taken:
- Converted all columns to appropriate formats (Date, Number, Currency)
- Cleaned text fields using TRIM and PROPER functions
- Removed duplicate records
- Dropped rows with missing Segment values (minimal impact)
- Removed "$" using SUBSTITUTE + VALUE functions
- Used XLOOKUP to retrieve Product Cost from the lookup table
- Created Sales column = Quantity × Product Cost
- Created helper columns:
  - Month
  - Year
  - Quarter
  - Weekday
  - Order Category (Large vs Standard orders)
## Dashboard
The dashboard provides an interactive overview of sales performance using key metrics and visualizations.
<img width="1849" height="786" alt="rainbow_store_dashboard" src="https://github.com/user-attachments/assets/6544a85e-e4de-471b-a0b7-3e27cd2053ed" />
It includes:
- KPI cards (Total Sales, Average Order Value, Orders, Customers)
- Sales by Region
- Sales by Product Category
- Top 5 Products
- Monthly Sales Trend
- Quarterly Sales Trend
- Weekday vs Weekend Sales
Users can interact with the dashboard using slicers for:
- Product Category
- Region
- Month
- Quarter
- Year
## Key Perfomance Indicators (KPIs)
The following KPIs were identified from the analysis:
- Total Sales: $4,183,448.68 which indicates overall revenue performance
- Average Order Value: $1,271.56 which shows average customer spending per order
- Number of Orders: 3290 which reflects purchasing activity
- Number of Customers: 101 which represents the size of the customer base
## Key Insights
### Top Performing Category:
Office Supplies generated the highest sales (~$859,782), followed closely by Home & Kitchen, while Electronics recorded the lowest sales.
### Top Products:
The best-performing products include Air Fryer, Coffee Maker, Toaster, Smartphone, and Socks, with Home & Kitchen dominating the top positions.
### Regional Performance:
The East region recorded the highest sales (~$887,417), indicating strong market performance, while the South region had the lowest sales, suggesting potential improvement opportunities.
### Monthly Trend:
Sales fluctuate throughout the year, with noticeable peaks in July and October, indicating possible seasonal demand patterns.
### Quarterly Trend:
Q4 recorded the highest sales, showing strong end-of-year performance, while Q1 had the lowest sales, suggesting slower activity at the beginning of the year.
### Customer Behavior:
Weekday sales (72.86%) significantly exceed weekend sales (27.14%), indicating that most purchases occur during working days.
## Business Recommendation
Based on the analysis, the business should:
- Focus marketing efforts on high-performing categories such as Office Supplies and Home & Kitchen
- Investigate low-performing regions (e.g., South) and apply targeted strategies to improve sales
- Increase inventory for top-selling products to avoid stock shortages
- Introduce promotions or campaigns during low-performing periods (e.g., early months of the year)
- Leverage strong Q4 performance by planning early for peak-season demand
## Conclusion
The analysis provides valuable insights into sales performance across products, regions, and time periods.
By focusing on high-performing areas and addressing underperforming segments, Rainbow World can improve decision-making, optimize operations, and drive sustained business growth.
