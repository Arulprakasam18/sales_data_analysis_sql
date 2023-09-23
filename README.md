# sales_data_analysis_sql
Walmart-Sales-Data-Analysis-SQL-Project
# Project Description
This SQL project aims to utilize the Walmart Sales data to gain insights into various aspects, including top-performing branches and products, sales trends across different products, and customer behavior. The primary objective is to analyze the data using SQL queries and identify opportunities for improving and optimizing sales strategies.

#  Data Dictionary
This dataset contains sales transactions from three different branches of Walmart, respectively located in Mandalay, Yangon and Naypyitaw. The data contains 17 columns and 1000 rows:

Column	                       Description	             Data Type
invoice_id	        Invoice of the sales made	           VARCHAR(30)
branch	           Branch at which sales were made	     VARCHAR(5)
city	             The location of the branch	           VARCHAR(30)
customer_type     The type of the customer	             VARCHAR(30)
gender	          Gender of the customer making purchase VARCHAR(10)
product_line	     set of related products	             VARCHAR(100)
unit_price	       The price of each product	           DECIMAL(10, 2)
quantity	         The amount of the product sold	       INT
VAT	               The amount of tax on the purchase	   FLOAT(6, 4)
Revenue	          The total cost of the purchase (sales) DECIMAL(10, 2)
date	            The date on which the purchase was made	DATETIME
time	            The time at which the purchase was made	TIME
payment_method	  The total amount paid	                  DECIMAL(10, 2)
cogs	            Cost Of Goods sold	                    DECIMAL(10, 2)
Profit	          Net Income	                            DECIMAL(10, 2)
Profit Margin	    percentage of Profit	                  FLOAT(11, 9)
rating	          Rating	                                FLOAT(2, 1)

# Methodology
# Data Understanding:

Familiarized with dataset structure, columns, data types, and data dictionary.
Identified specific business questions or objectives.
# Data Assessment:

Evaluated data quality and structure for issues like missing values, outliers, and formatting inconsistencies.
# Data Cleaning and Preprocessing:

Implemented constraints on the data, including the use of a Primary Key constraint to ensure uniqueness, data integrity, and data consistency.
Specified appropriate data types for columns to ensure accurate storage and manipulation of data.
Applied NOT NULL constraints on specific columns to enforce the requirement that they must have non-null values. This ensures data completeness and prevents the insertion of null values in those columns.
# Feature Engineering:

Created new variables and features from existing data that provided additional insights, such as:
created a column called time_of_day to capture sales patterns in the Morning, Afternoon, and Evening. This information will help determine the peak sales periods during the day.
created a column named day_nameto extract the specific day of the week when each transaction occurred (Mon, Tue, Wed, Thur, Fri). This data will aid in understanding the busiest days for each branch.
created a column named month_name to extract the month of the year for each transaction (Jan, Feb, Mar). This data will assist in identifying the months with the highest sales and profitability.
# Exploratory Data Analysis (EDA):
Some of the business questions I've answered based on the data:

# Generic Questions
How many unique cities does the data have?
In which city is each branch?
# Product related Questions
How many unique product lines are included in the data?
Which payment method is the most frequently used?
Which product line has the highest sales volume?
What is the total revenue for each month?
Which month had the highest Cost of Goods Sold (COGS)?
Which product line generated the highest revenue?
Which city had the highest revenue?
Which product line had the highest Value Added Tax (VAT)?
For each product line, add a column indicating whether it has "Good" or "Bad" sales, based on whether its sales are above or below the average.
Which branch sold more products than the average number of products sold?
What is the most common product line based on gender?
What is the average rating for each product line?
# Sales related Questions
How many sales were made during each time of the day for each weekday?
Which customer type generates the highest revenue?
Which city has the highest tax percentage or VAT (Value Added Tax)?
Among the customer types, which one pays the highest amount in VAT?
# Customer related Questions
How many distinct customer types are represented in the data?
How many unique payment methods are available in the data?
Which customer type generates the highest revenue?
Which customer type has the highest total sales?
What is the predominant gender among the customers?
How is the gender distributed across branches?
During which time of the day do customers provide the most ratings?
During which time of the day do customers provide the most ratings for each branch?
Which day of the week has the highest average ratings overall?
Which day of the week has the highest average ratings for each branch?
# Analysis Approach
  # Product Analysis:

Utilized SQL to conduct in-depth analysis of product lines to identify top-performing and underperforming segments.
Identified areas for improvement within each product line.
# Sales Analysis:

Leveraged SQL to analyze sales trends, providing insights into product performance and effectiveness of sales strategies.
Implemented SQL queries to measure the impact of different sales strategies and recommend modifications for increased sales.
# Customer Analysis:

Uncovered customer segments and their purchasing patterns.
Utilized SQL queries to extract actionable insights, enabling targeted marketing efforts and optimizing customer satisfaction.
Revenue And Profit Calculations
COGS = unitsPrice * quantity

VAT = 5% * COGS

VAT is added to the 
 and this is what is billed to the customer.

Revenue = VAT + COGS

Profit = revenue - COGS

Profit Margin % = (total profit/ total revenue)*100
