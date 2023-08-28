# Kimia Farma Database Project README

This project involves creating a MySQL database for managing customer information, product details, and sales transactions for Kimia Farma. It also provides instructions for importing data from CSV files into the database, creating an aggregate table, and exporting data to a CSV file.

## Table of Contents

- [Database Setup](#database-setup)
- [Importing Data](#importing-data)
- [Creating Aggregate Table](#creating-aggregate-table)
- [Exporting Data](#exporting-data)
- [SQL Data Analysis](#sql-data-analysis)
- [Tableau Data Visualization]

## Database Setup

1. Create a new MySQL database named `kimia_farma`.
2. Use the newly created database: `USE kimia_farma`.

## Importing Data

1. Create the `customers` table using the provided SQL script. This table stores customer information.
2. Create the `products` table using the provided SQL script. This table stores product details.
3. Create the `sales` table using the provided SQL script. This table stores sales transaction information.

After creating the tables, you can import data from CSV files into each table using MySQL's Table Data Import Wizard or by running appropriate SQL commands.

## Creating Aggregate Table

1. Create an aggregate table named `aggregate_table` by performing a LEFT JOIN operation on the `sales`, `customers`, and `products` tables. This table will combine sales data with customer and product details.
2. Add a computed column named `total_sales` to the `aggregate_table`. This column calculates the total sales amount for each transaction by multiplying the `number_of_products` with the `product_price`.

## Exporting Data

1. Use MySQL's Table Data Export Wizard to export the `aggregate_table` data to a CSV file. Alternatively, you can run the SQL query `SELECT * FROM aggregate_table` and then click Export.
2. The exported CSV file will contain the aggregated sales data along with customer and product information.

## SQL Data Analysis

In addition to setting up the database structure and importing data, this project involves performing SQL data analysis on the collected data to gain valuable insights into the sales and customer behavior within Kimia Farma. The SQL data analysis queries are designed to extract meaningful information from the database and provide a deeper understanding of the business operations. Below is an overview of the key areas covered in the SQL data analysis:

### Average Monthly Revenue

This analysis helps in understanding the average sales revenue generated for each month, considering all the years. By grouping the data by month and calculating the average revenue, it becomes possible to identify patterns and trends in sales performance over time.

### Top 5 Customers by Purchase Value

Identifying the top customers based on their total purchase value is crucial for recognizing the most valuable clients. This analysis ranks customers according to the sum of their total purchases, allowing you to pinpoint the highest revenue-generating customers.

### Top 5 Best-Selling Products

The analysis of the top-selling products based on the total number of units sold provides insights into product popularity. By identifying the products that have the highest sales volume, businesses can focus on optimizing their inventory and marketing strategies.

### Customer Loyalty Tiers

Categorizing customers into different loyalty tiers based on their total purchase value offers a way to segment the customer base. This analysis assists in identifying loyal customers and tailoring marketing efforts to enhance customer retention.

### Average Product Price by Brand

Calculating the average product price for each brand aids in understanding brand positioning and pricing strategies. This analysis helps to compare the average prices of products from different brands.

### Top 5 Revenue Dates

Identifying the top revenue-generating dates helps in recognizing specific time periods with exceptional sales performance. This analysis allows businesses to plan and allocate resources effectively during peak sales periods.

### Distinct Products per Customer

Analyzing the number of distinct products purchased by each customer sheds light on customer buying behavior. It helps to identify customers who explore a variety of products and those who prefer specific items.

### Average Transaction Value by Customer Group

Calculating the average transaction value for each customer group provides insights into the spending patterns of different customer segments. It aids in understanding the revenue contribution of various customer groups.

These SQL data analysis queries provide a comprehensive understanding of sales trends, customer behavior, and product performance within the Kimia Farma sales ecosystem. By leveraging these insights, businesses can make informed decisions to optimize their operations, enhance customer experiences, and drive growth.

## Tableau Data Visualization

### Kimia Farma Sales Dashboard on Tableau: Visualizing Sales Insights

In this Tableau project, I designed a dynamic and insightful dashboard to visualize sales data for Kimia Farma, a pharmaceutical company. Leveraging Tableau's powerful features, I created compelling visualizations that provide a comprehensive understanding of sales performance, customer behavior, and product analysis.

### Key Dashboard Visualizations:

1. Total Sales by Brand (Line Chart): I developed a line chart showcasing day-to-day total sales for each brand. This visualization allows for easy tracking of brand performance over time and highlights sales trends.

2. Average Price by Brand (Bar Chart): To analyze pricing strategies, I designed a bar chart illustrating the average price for each brand. This visualization aids in evaluating brand positioning and competitiveness in the market.

3. Items Sold per Product (Horizontal Bar Chart): I crafted a horizontal bar chart to display the number of items sold per product. This visualization identifies best-selling products and provides insights into demand patterns.

4. Total Sales per Customer (Treemaps): Using treemaps, I depicted total sales per customer group. This visualization helps identify key customer segments contributing to overall revenue and provides a hierarchical view of sales distribution.

The dashboard serves as a powerful tool for decision-makers to gain actionable insights into sales performance and customer trends. By combining multiple visualizations, I aimed to provide a comprehensive overview of the company's sales landscape, enabling informed business decisions.

[Visit The Dashboard] (https://public.tableau.com/views/KimiaFarmaSalesDashboard/SalesDashboard2?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

![image](https://github.com/billy-enrizky/Kimia-Farma-Sales-Management-Database-Project/assets/132111170/c816d79b-32b5-4ac6-8991-7603df5be2be)

Note: Make sure to replace placeholders such as file paths, table names, and column names with actual values according to your system configuration and project requirements.

For any issues or inquiries, feel free to contact the project contributors.

---
Project Contributors: [Muhammad Enrizky Brillian]
