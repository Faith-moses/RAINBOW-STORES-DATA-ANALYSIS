# RAINBOW WORLD SALES PERFORMANCE DASHBOARD (2024)
## Introduction
This project analyzes Rainbow World sales dataset for the year 2024 to identify sales trends, top performing products, region performance and areas for improvement. The goal is to support data-driven decision-making and improve overall profitability.
## Problem Statement
Despite generating significant sales in 2024, the business lacks clear insights into product performance, regional contributions, and sales trends over time. This analysis aims to answer the following key questions:
- Which product category has the highest sales?
- What are the top performing products?
- Which region performs best?
- What is the sales trend across the month
- When do purchases increase?
## Tools Used
This analysis was carried out using:
- Microsoft Excel
- Pivot Tables
- Charts
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
During Inspection of the dataset, it was observed that the dataset contained errors which could affect the analyses, such as:
- Invalid format on the Order date, Quantity, Product Cost and Sales column
- Inconsistent casing, leading and trailing spaces in Product Category and Region
- 54 duplicate rows based on the Order ID
- 10 missing entries in the Segment column
- Product Cost column on the Product lookup sheet were in text format due to the manually inputed '$' sign
- No entries on the Product Cost and Sales columns
These missing entries, duplicates and invalid formats were handled in the following ways:
- All columns were correctly formatted, Order Date as Date, Product Cost as Number, Quantity as Number and Sales as Currency.
- The inconsistent casing and leading/trailing spaces in the Category and region were handled using 'proper' and 'trim' function and category was renamed as Product Category to fully imply what it stands for.
- The 54 duplicates were removed as they are repetition of information.
- The rows with the 10 missing entries on the Segment column were removed from the dataset because they are very small and removing them will not affect the analyses
- The '$' which was manually inputted in the Product Cost of the Product lookup sheet was removed and the column converted to currency using the 'Value and Substitute' function.
- The Product Cost column was filled using the 'Lookup' function, which was used to extract the cost of every Product using their Product ID from the Product lookup sheet.
- The Sales column was filled by calculating Quantity x Product Cost.
- Helpers Columns such as Product from Product lookup sheet, Month from Order Date, Year from Order Date, Weekday from Order Date, Order Status (Large Order, Standard Order) using the IF condition on Sales.
## Dashboard
The Rainbow World Sales dashboard shows the Total sales, Average Order Value, Median Quantity sold, Number of Orders and Customers and sales trend over time, top performing products, product categories and regions. This interactive dashboards contains slicers which can be used to filter by Regions, Product Categories, Months and Year.
<img width="1849" height="786" alt="rainbow_store_dashboard" src="https://github.com/user-attachments/assets/6544a85e-e4de-471b-a0b7-3e27cd2053ed" />
## Key Perfomance Indicators (KPIs)
The following KPIs were identified from the analysis:
- Total Sales: $4,183,448.68 which shows the total sales perfomance
- Average Order Value: $1,271.56 which shows spending behaviour of customers
- Number of Orders: 3290 which shows customers purchasing behaviour
- Median Quantity Sold: 10 which shows product performance
- Number of Customers: 101, indicating the size of customer base and overall business reach
## Key Insights
The following insights were derived from the analyses:
- Office Supplies had the highest sales with $859,782, followed by Home & Kitchen which made approximately $854,044 while Electronics had the lowest sales with $813,227
- The Top 5 performing products were Air Fryer, Coffee Maker, Toaster, Smartphone, Socks which are dominated by Home & Kitchen category.
- The East region generated the highest sales (~$887,417), indicating strong market demand or effective sales strategies in that region. In contrast, the South region recorded the lowest sales, suggesting a potential need for improved marketing or customer engagement.
- Sales show fluctuating trends throughout the year, with peaks in June and October. This suggests possible seasonal demand patterns, indicating that the business can strategically increase inventory and marketing efforts during these peak periods. 
## Business Recommendation
Rainbow World should:
- Increase marketing efforts for high-performing categories such as Office Supplies and Home & Kitchen to maximize revenue growth.
- Investigate the South region’s low performance and implement targeted marketing or pricing strategies to improve sales.
- Increase stock on Top performing Products
- Run promotions during low-sales months
## Conclusion
This analysis highlights key opportunities for improving sales performance by focusing on high-performing products and regions while addressing underperforming areas. By leveraging these insights, Rainbow World can make informed decisions to drive growth and increase profitability.
