# Olist SQL Analysis

## Overview

This project analyzes the **Olist e-commerce dataset** using SQL to uncover insights related to customers, revenue, products, and purchasing behavior.

The analysis focuses on identifying high-value customers, understanding revenue trends, evaluating product and category performance, and segmenting customers based on their spending and purchase frequency.

The project uses **MySQL** queries and demonstrates practical SQL techniques such as joins, aggregation, Common Table Expressions (CTEs), window functions, conditional logic, and ranking.

## Business Questions

The analysis answers the following business questions:

1. Who are the **top 10 customers by total amount spent**?
2. What is the **monthly revenue trend** across the dataset?
3. What is the **month-over-month change in revenue**?
4. Which **product categories generate the most revenue**?
5. What are the **top 3 products within each category by revenue**?
6. How can customers be segmented into **Low, Medium, and High spend tiers**?
7. How many customers are **repeat buyers versus one-time buyers**?
8. What percentage of **total revenue comes from the top-performing product category**?

## Key Findings

The SQL analysis is designed to provide insights into the following areas:

### Customer Value
- Identifies the top 10 customers based on their total payment value.
- Calculates total customer spending using customer, order, and payment data.
- Segments customers into:
  - **Low:** total spend below 500
  - **Medium:** total spend from 500 to 1,500
  - **High:** total spend above 1,500

### Revenue Performance
- Calculates monthly revenue based on order purchase dates and payment values.
- Measures month-over-month revenue changes using the `LAG()` window function.
- Identifies the product category with the highest revenue and calculates its contribution to total category revenue.

### Product Performance
- Ranks product categories according to total revenue.
- Identifies the top 3 revenue-generating products within each product category using `ROW_NUMBER()`.

### Customer Behavior
- Compares the number of **one-time buyers** with **repeat buyers**.
- Customers with one order are classified as one-time buyers, while customers with more than one order are classified as repeat buyers.

> **Note:** The attached SQL files contain the analysis queries but do not include the query output/results. Therefore, specific numerical findings are not stated in this README.

## Recommendations

Based on the types of analysis included in this project, the results can be used to:

- Identify and understand **high-value customers**.
- Develop targeted strategies for different **customer spending segments**.
- Monitor **monthly revenue performance** and changes over time.
- Investigate periods with significant **month-over-month revenue changes**.
- Focus product and marketing efforts on **high-revenue categories and products**.
- Develop strategies to encourage **one-time customers to become repeat buyers**.
- Assess revenue concentration and dependency on the **top-performing product category**.

These recommendations should be refined after reviewing the actual SQL query results.

## Tools & Skills

### Tools
- MySQL
- MySQL Workbench
- GitHub

### SQL Skills Demonstrated
- `SELECT`
- `JOIN`
- `INNER JOIN`
- `GROUP BY`
- `ORDER BY`
- `LIMIT`
- Aggregate functions such as `SUM()` and `COUNT()`
- `ROUND()`
- `DATE_FORMAT()`
- Common Table Expressions (`WITH`)
- Window functions:
  - `LAG()`
  - `ROW_NUMBER()`
  - `SUM() OVER()`
- `CASE` statements
- Customer segmentation
- Ranking and comparative analysis

## Files

| File | Description |
|---|---|
| `query1.sql` | Top 10 customers by total spending |
| `query2.sql` | Monthly revenue trend |
| `query3.sql` | Month-over-month revenue change |
| `query4.sql` | Revenue by product category |
| `query5.sql` | Top 3 products by category |
| `query6.sql` | Customer spending segmentation |
| `query7.sql` | Repeat vs. one-time buyers |
| `query8.sql` | Top category's contribution to total revenue |

## Dataset

The analysis uses the **Olist e-commerce dataset**, including tables related to:

- Customers
- Orders
- Order Payments
- Order Items
- Products
- Product Categories

## Project Purpose

This project demonstrates how SQL can be used to transform raw e-commerce data into **business-focused insights** that support customer analysis, revenue monitoring, product performance evaluation, and decision-making.
