# Joduke Scientific — Sales & Product Profitability Analysis

## Introduction

Joduke Scientific is a scientific equipment and laboratory apparatus business that supplies products used by schools, universities, science tutorial centres and individual buyers.

This project analyzes Joduke Scientific's sales transactions to understand revenue, profitability, product performance and customer purchasing patterns.

The analysis was performed using SQL in PostgreSQL to demonstrate how SQL can be used to clean, transform, analyze and extract business insights from transactional data.

---

## Problem Statement

Joduke Scientific records sales transactions across different products, customer types and locations.

However, without analyzing the sales data, it can be difficult to determine which products are generating the most revenue and profit, which customer groups contribute the most to sales, and how business performance changes over time.

The business therefore needs a data-driven analysis to understand its sales and profitability performance and support better decisions around inventory, product focus and customer targeting.

---

## Project Objective

The objective of this project was to use SQL to analyze Joduk Scientific's sales data and identify:

- Overall sales revenue and profit
- Best-performing products
- Most profitable products
- Best-performing product categories
- Customer types generating the most revenue
- Monthly sales and profit trends

The goal was to turn transactional data into useful business insights that can support better decision-making.

---

## Business Questions

1. What is the total sales revenue and total profit?
2. Which products generate the most revenue?
3. Which products generate the highest profit?
4. Which product categories perform best?
5. Which customer type generates the most revenue?
6. How do sales and profit change over time?

---

## Tools Used

- PostgreSQL
- SQL
- pgAdmin
- Excel

PostgreSQL and pgAdmin were used to store and analyze the transactional data using SQL queries.

Excel was used to organize and present selected analysis results and visualizations.

---

## Data Sourcing

The dataset used for this project was gotten from Joduke Scientific records.

The dataset contains **1,806 sales transaction records** covering January to December 2025.

The dataset includes information about:

- Order dates
- Products
- Product categories
- Quantity sold
- Selling prices
- Cost prices
- Discounts
- Sales revenue
- Cost
- Profit
- Customer types
- Locations
- Payment methods
- Sales representatives
- Profit margins

---

## Data Structure

The main table used for the analysis was:

`sales_data`

Important columns included:

- `order_id`
- `order_date`
- `product_name`
- `category`
- `quantity`
- `unit_selling_price`
- `unit_cost_price`
- `discount_rate`
- `sales_amount`
- `cost_amount`
- `customer_type`
- `location`
- `payment_method`
- `sales_rep`
- `profit`
- `profit_margin_pct`

---

## Data Cleaning & Transformation

The dataset was reviewed before analysis to identify potential data quality issues.

The cleaning process included:

- Checking for duplicate transactions
- Checking for missing values
- Reviewing inconsistent product names
- Standardizing category names
- Reviewing inconsistent capitalization
- Checking numerical fields
- Validating dates
- Reviewing calculated sales and profit values
- Checking profit margin values

Some inconsistent labels were identified, including variations such as:

- `Measuring cylinder 100ml`
- `compound microscope`
- `Lab Equipments`

These were reviewed and standardized where appropriate.

Duplicate-like transactions were also investigated to ensure that repeated transaction records did not distort the analysis.

---

## SQL Concepts Applied

The following SQL concepts were used in the project:

- `SELECT`
- `WHERE`
- `ORDER BY`
- `GROUP BY`
- Aggregate functions
- `SUM()`
- `AVG()`
- `COUNT()`
- `ROUND()`
- `CASE WHEN`
- Date functions
- Calculated metrics
- Filtering
- Sorting
- Data quality checks
- Duplicate checks
- Grouped analysis
- Monthly trend analysis

These SQL techniques were used to transform raw transaction data into business-focused analysis results.

---

## Analysis Performed

### 1. Overall Sales & Profitability

The first analysis calculated the overall performance of the business, including:

- Total revenue
- Total profit
- Total cost
- Total orders
- Profit margin

This provided an overall view of Joduk Scientific's financial performance during the period analyzed.

---

### 2. Revenue by Product

Products were ranked based on total revenue generated.

This helped identify the products contributing the largest amount of sales revenue and provided insight into which products may deserve greater attention from the business.

---

### 3. Profit by Product

Products were also analyzed based on total profit.

This is important because a product generating high revenue does not necessarily generate the highest profit.

Comparing revenue and profit helps the business understand which products are financially valuable rather than focusing only on sales volume.

---

### 4. Category Performance

Sales and profitability were grouped by product category to determine which categories performed best.

The categories analyzed included:

- Biology Equipment
- Microscopes
- Physics Equipment
- Chemistry Equipment
- Measuring Instruments
- Lab Equipment
- Glassware

This analysis helps identify categories that contribute strongly to revenue and profit.

---

### 5. Customer Type Analysis

Revenue and other sales metrics were analyzed by customer type.

Customer groups included:

- Secondary Schools
- Private Schools
- Public Schools
- Science Tutorial Centres
- Universities
- Individual Buyers

This analysis helps identify the customer groups contributing the most revenue.

---

### 6. Monthly Sales & Profit Analysis

Sales and profit were grouped by month to identify changes in business performance throughout the year.

Monthly analysis can help the business identify:

- Strong sales periods
- Weak sales periods
- Seasonal patterns
- Changes in profitability

---

## Key Insights

### 1. Secondary Schools were the largest customer segment

Secondary Schools generated the highest revenue among the analyzed customer groups, with approximately **₦98.7 million** in revenue.

Private Schools followed with approximately **₦68.6 million**, while Public Schools generated approximately **₦65.2 million**.

This suggests that schools, particularly secondary schools, represent an important customer segment for Joduk Scientific.

---

### 2. Biology Equipment generated the highest category revenue

Biology Equipment generated approximately **₦112.3 million** in revenue, making it the highest-revenue category in the analysis.

Microscopes followed with approximately **₦94.5 million**, while Physics Equipment generated approximately **₦55.97 million**.

This indicates that Biology Equipment and Microscopes are particularly important categories for the business.

---

### 3. Human Torso Model was the highest-revenue product

The Human Torso Model generated approximately **₦62.5 million** in revenue and ranked highest among the products analyzed by revenue.

Compound Microscope followed with approximately **₦52.6 million**.

This suggests that certain specialized educational and laboratory products contribute significantly to overall revenue.

---

### 4. Revenue and profit should be considered together

The highest-revenue product is not necessarily the product with the highest profit margin.

For this reason, the analysis considered both revenue and profitability rather than using sales revenue alone to evaluate product performance.

---

### 5. Customer segmentation can support sales strategy

The significant contribution from school-based customers suggests that Joduk Scientific could focus marketing and sales efforts on educational institutions.

This could include targeted relationships with schools, tutorial centres and universities.

---

## Business Decisions Supported

Based on the analysis, Joduk Scientific can use the findings to:

- Prioritize high-performing products
- Maintain adequate stock levels for high-demand products
- Focus marketing on high-revenue categories
- Develop stronger relationships with schools
- Target secondary schools with relevant products
- Review low-performing products
- Compare revenue against profit before making product decisions
- Plan inventory based on historical sales patterns
- Identify opportunities for category-specific promotions
- Monitor monthly sales performance
- Improve sales strategies using customer segmentation

---

## Dashboard / Analysis Screenshots

Screenshots of the SQL analysis results and Excel visualizations are included below.


### Overall Sales & Profitability dasboard

<img width="518" height="277" alt="Joduke dashboard" src="https://github.com/user-attachments/assets/cea13551-ce1a-4f60-97d5-f6c8f3d2b53d" />



### Highest Revenue Products

<img width="959" height="490" alt="Joduke Products by revenue" src="https://github.com/user-attachments/assets/662359fa-bfbb-4aea-8669-b24386414f7e" />


### KPIS

<img width="958" height="491" alt="Joduke KPIS" src="https://github.com/user-attachments/assets/a181bd10-0f75-4047-b8a6-58dd850dd16c" />


---

## Project Summary

This project analyzed 1,806 simulated sales transactions for Joduk Scientific using PostgreSQL and SQL.

The analysis focused on sales revenue, profitability, product performance, category performance, customer segments and monthly trends.

The results showed that secondary schools were the largest customer segment and Biology Equipment generated the highest category revenue.

The project demonstrates how SQL can be used to transform transactional data into meaningful business insights and support data-driven decisions around products, customers, inventory and sales strategy.

---

## Skills Demonstrated

- SQL
- PostgreSQL
- pgAdmin
- Data cleaning
- Data transformation
- Data aggregation
- Business analysis
- Revenue analysis
- Profitability analysis
- Customer segmentation
- Product analysis
- Trend analysis
- Data visualization
- Business decision-making
