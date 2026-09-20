# Olist SQL Analysis

## Overview

This project explores Olist's Brazilian e-commerce data to understand customer purchases, products, orders, and sales performance. It has 9 related tables covering order activity from September 2016 to October 2018. Since the tables are connected through different IDs, careful joins are needed to avoid counting the same order, payment, or customer more than once. This project focuses on using SQL to turn the raw data into useful business insights.

## Business Questions

The analysis answers the following business questions:

1. Who are the top 10 customers by total amount spent?
2. What is the monthly revenue trend across the dataset?
3. What is the month-over-month change in revenue?
4. Which product categories generate the most revenue?
5. What are the top 3 products within each category by revenue?
6. How can customers be segmented into Low, Medium, and High spend tiers?
7. How many customers are repeat buyers versus one-time buyers?
8. What percentage of total revenue comes from the top-performing product category?

## Key Findings

1. The business has a retention gap, not a customer acquisition gap: The customer base is overwhelmingly made up of one-time buyers, with 93,099 customers (96.9%) purchasing only once compared with just 2,997 repeat buyers (3.1%), while the top 10 customers each spent at least R$4,764.34 and the highest spender reached R$13,664.08. This means Olist has a clear opportunity to increase customer lifetime value by converting more first-time buyers into repeat customers through personalized follow-ups, cross-category recommendations, and targeted incentives after the first purchase. The combination of a very large one-time customer base and a smaller group of high-spending customers creates a strong opportunity for customer segmentation and retention-focused marketing.

2. Revenue is concentrated in winning categories, but no single category dominates: Health & Beauty generated the most revenue at R$1.259M, followed by Watches & Gifts (R$1.205M) and Bed, Bath & Table (R$1.037M), yet even the top category represented only 9.39% of total product revenue, while individual products such as the top Health & Beauty product generated R$63,885. This means Olist has a relatively diversified revenue base rather than depending on one dominant category, while its strongest categories and products provide clear opportunities for expanding successful assortments, improving product visibility, and cross-selling complementary products. The key finding is not simply that Health & Beauty leads, but that several category “engines” contribute meaningfully to overall revenue.

3. Revenue growth has strong momentum but also significant volatility: Monthly revenue increased from R$138K in January 2017 to more than R$1.16M by April 2018, with the largest positive month-over-month increase occurring in November 2017 (+R$415K), but the data also shows an extreme decline of approximately R$1.02M in September 2018. This means the business demonstrated substantial growth capacity while also experiencing large fluctuations that require careful interpretation. In particular, the September–October decline should not automatically be treated as a genuine loss of demand because the Olist dataset has incomplete coverage toward the end of the period; instead, management should investigate data completeness, order activity, and seasonality before using those months for forecasting or performance evaluation.


## Recommendations

1. Launch a data-driven customer retention program: Segment the 93,099 one-time buyers based on their purchase history and send personalized follow-ups, cross-category recommendations, and targeted incentives within 30–60 days after their first purchase. Prioritize high-value customers and customers who purchased from the strongest categories to increase repeat purchases and customer lifetime value.

2. Scale winning categories while strengthening revenue planning: Increase inventory, advertising visibility, and promotional placement for high-performing products across Health & Beauty, Watches & Gifts, and Bed, Bath & Table, while using cross-selling to connect customers across these categories. Because no single category contributes more than 10% of revenue, Olist can pursue growth across multiple category leaders rather than over-investing in one segment, while monitoring monthly sales and data completeness to distinguish genuine demand changes from incomplete reporting (September–October 2018).


## Tools & Skills

Language & Database: MySQL

SQL Techniques:

Relational Joins: Multi-table INNER JOIN operations linking customers, orders, order payments, order items, products, and product categories.

Aggregations & Grouping: SUM(), COUNT(), ROUND(), GROUP BY, and ORDER BY for revenue, customer spending, and product performance analysis.


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
- Geolocation
- Orders
- Order Payments
- Order Items
- Order Reviews
- Products
- Product Categories
- Sellers

## Project Purpose

The purpose of this project is to analyze the Olist e-commerce dataset using SQL and transform transactional data into meaningful business insights.

The analysis focuses on customer spending and behavior, revenue trends, product and category performance, customer segmentation, and repeat purchasing patterns. It answers key business questions such as identifying high-value customers, tracking monthly and month-over-month revenue, ranking top-performing products and categories, segmenting customers by spending level, and comparing one-time versus repeat buyers.

This project also demonstrates practical SQL and data analysis skills, including multi-table joins, aggregations, CTEs, subqueries, conditional logic, date analysis, set operations, and window functions. Overall, it showcases the use of SQL to solve business questions and support data-driven decision-making.
