\# Retail Sales \& Customer Segmentation Analysis using SQL



\## 📌 Project Overview

In the rapidly evolving retail industry, understanding sales performance and customer purchasing behavior is critical for driving growth and improving customer engagement.  

This project analyzes retail transaction, customer, and inventory data using SQL to uncover insights related to product performance, customer segmentation, and repeat purchasing behavior.  

The analysis supports data-driven decision-making for inventory optimization, targeted marketing, and customer retention strategies.



---



\## 🎯 Business Problems

The retail company is experiencing stagnant growth and declining customer engagement.  

This project addresses the following key business problems:



\- Identifying high-performing and low-performing products

\- Segmenting customers based on purchasing behavior

\- Understanding repeat purchases and customer loyalty

\- Supporting inventory planning and marketing decisions using data



---



\## 🗂 Dataset Description

The project uses three relational tables:



\### 1. Sales Transaction

Stores transaction-level sales data.

\- `transaction\_id`

\- `customer\_id`

\- `product\_id`

\- `quantity\_purchased`

\- `transaction\_date`

\- `price`



\### 2. Customer Profiles

Stores customer demographic and profile information.

\- `customer\_id`

\- `age`

\- `gender`

\- `location`

\- `join\_date`



\### 3. Product Inventory

Stores product and inventory-related data.

\- `product\_id`

\- `product\_name`

\- `category`

\- `stock\_level`

\- `price`



\### Data Relationships

\- `sales\_transaction.customer\_id` → `customer\_profiles.customer\_id`

\- `sales\_transaction.product\_id` → `product\_inventory.product\_id`



---



\## 🛠 SQL Concepts Used

\- JOINs (INNER, LEFT)

\- GROUP BY \& HAVING

\- CASE WHEN

\- Common Table Expressions (CTEs)

\- Aggregate functions (SUM, COUNT, AVG)

\- Date functions

\- Filtering and sorting

\- Subqueries



---



\## 🔍 Analytical Approach



\### 1. Data Cleaning \& Validation

\- Checked for NULL values in critical columns such as quantity and price

\- Validated data consistency and row counts

\- Ensured correct aggregation before joining tables to avoid duplication



---



\### 2. Product Performance Analysis

\- Calculated total quantity sold and revenue per product

\- Identified high-performing and low-performing products

\- Highlighted products with high inventory but low sales



---



\### 3. Customer Segmentation

Customers were segmented based on \*\*total quantity purchased\*\*:



| Total Quantity Purchased | Customer Segment |

|--------------------------|------------------|

| 0                        | No Orders        |

| 1 – 10                   | Low              |

| 10 – 30                  | Mid              |

| > 30                     | High Value       |



This segmentation enables targeted marketing and customer retention strategies.



---



\### 4. Customer Behavior Analysis

\- Identified repeat customers using transaction counts

\- Analyzed purchase frequency to infer loyalty

\- Measured contribution of each customer segment to overall sales



---



\## 📊 Key Insights

\- High Value customers contribute a disproportionately large share of total sales

\- Most customers fall into Low and Mid segments, indicating growth potential

\- Certain products show overstocking risk due to low sales and high inventory

\- Repeat customers generate significantly higher purchase volumes



---



\## ⚠ Assumptions \& Limitations

\- Returns and refunds are not included in the dataset

\- Customer activity is measured only through completed transactions

\- Seasonal trends are limited by the available date range

\- Prices are assumed to be accurate per transaction record



---



\## 🧰 Tools Used

\- SQL (MySQL / PostgreSQL compatible syntax)

\- Git \& GitHub for version control and documentation



---



\## 📌 Conclusion

This project demonstrates how SQL can be used to transform raw retail data into meaningful business insights.  

By combining structured queries with analytical reasoning, the project highlights customer behavior patterns, product performance trends, and operational improvement opportunities in a retail environment.



