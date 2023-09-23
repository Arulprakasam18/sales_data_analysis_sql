# Walmart Sales Data Analysis with SQL

## Project Description

This project focuses on leveraging Walmart sales data to gain valuable insights into various aspects, including top-performing branches and products, sales trends across different products, and customer behavior. The primary objective is to analyze the data using SQL queries and identify opportunities for improving and optimizing sales strategies.

## Data Dictionary

The dataset contains sales transactions from three different branches of Walmart, located in Mandalay, Yangon, and Naypyitaw. The dataset comprises 17 columns and 1000 rows, with the following data types:

| Column           | Description                                  | Data Type      |
|------------------|----------------------------------------------|----------------|
| invoice_id       | Invoice of the sales made                   | VARCHAR(30)    |
| branch           | Branch where sales were made                | VARCHAR(5)     |
| city             | Location of the branch                      | VARCHAR(30)    |
| customer_type    | Customer type                                | VARCHAR(30)    |
| gender           | Gender of the customer making a purchase    | VARCHAR(10)    |
| product_line     | Set of related products                     | VARCHAR(100)   |
| unit_price       | Price of each product                       | DECIMAL(10, 2) |
| quantity         | Amount of the product sold                  | INT            |
| VAT              | Amount of tax on the purchase               | FLOAT(6, 4)    |
| Revenue          | Total cost of the purchase (sales)          | DECIMAL(10, 2) |
| date             | Date of the purchase                        | DATETIME       |
| time             | Time of the purchase                        | TIME           |
| payment_method   | Payment method                               | DECIMAL(10, 2) |
| cogs             | Cost Of Goods Sold (COGS)                   | DECIMAL(10, 2) |
| Profit           | Net Income                                  | DECIMAL(10, 2) |
| Profit Margin    | Percentage of Profit                        | FLOAT(11, 9)   |
| rating           | Rating                                      | FLOAT(2, 1)    |

## Methodology

### Data Understanding:

- Explored the dataset's structure, columns, data types, and data dictionary.
- Defined specific business questions and objectives.

### Data Assessment:

- Evaluated data quality, identifying issues such as missing values, outliers, and formatting inconsistencies.

### Data Cleaning and Preprocessing:

- Implemented constraints, including Primary Key constraints, to ensure data integrity and consistency.
- Specified appropriate data types for accurate storage and manipulation.
- Applied NOT NULL constraints to enforce data completeness.

### Feature Engineering:

- Created new variables and features:
  - `time_of_day`: Captures sales patterns in the Morning, Afternoon, and Evening.
  - `day_name`: Extracts the specific day of the week for each transaction.
  - `month_name`: Extracts the month of the year for each transaction.

### Exploratory Data Analysis (EDA):

Answered various business questions, including:

- Identifying unique cities in the data.
- Determining branch locations.
- Analyzing product lines and payment methods.
- Investigating sales volumes, revenues, and profitability.
- Assessing tax percentages and VAT.
- Analyzing customer types, gender distribution, and ratings.

## Analysis Approach

### Product Analysis:

- Utilized SQL to conduct in-depth analysis of product lines to identify top-performing and underperforming segments.
- Identified areas for improvement within each product line.

### Sales Analysis:

- Leveraged SQL to analyze sales trends and assess the effectiveness of sales strategies.
- Measured the impact of different sales strategies and recommended modifications for increased sales.

### Customer Analysis:

- Uncovered customer segments and purchasing patterns.
- Extracted actionable insights using SQL queries to optimize customer satisfaction and target marketing efforts.

## Revenue and Profit Calculations

- Cost Of Goods Sold (COGS) = unitPrice * quantity
- VAT = 5% * COGS
- Revenue = VAT + COGS
- Profit = Revenue - COGS
- Profit Margin % = (total profit / total revenue) * 100

This project report outlines the comprehensive analysis of Walmart's sales data using SQL, providing valuable insights and recommendations for optimizing sales strategies and improving business performance.
