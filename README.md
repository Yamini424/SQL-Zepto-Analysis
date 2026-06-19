**🛒 Zepto E-commerce SQL Data Analyst Portfolio Project**

This is a complete real-world SQL Data Analyst portfolio project based on an e-commerce inventory dataset inspired by Zepto, one of India’s fastest-growing quick-commerce platforms. This project simulates real Data Analyst workflows, from raw data exploration to business-focused data analysis.

This project is perfect for:

📊 Data Analyst aspirants who want to build strong portfolio projects for interviews and job applications

📚 Anyone learning SQL through practical hands-on projects

💼 Students preparing for roles in retail analytics, e-commerce analytics, or business intelligence

Project Overview

The goal of this project is to simulate how Data Analysts in e-commerce and retail companies use SQL to solve business problems.

The project focuses on:

✅ Setting up a real-world e-commerce inventory database

✅ Performing Exploratory Data Analysis (EDA) to understand product categories, pricing patterns, and stock availability

✅ Implementing Data Cleaning by removing invalid records, handling missing values, and converting pricing values into standard format

✅ Writing business-focused SQL queries to derive insights around revenue, pricing strategy, discounts, and inventory management

Dataset Overview

The dataset represents product inventory data from an e-commerce platform. It simulates real-world retail inventory systems used by online delivery companies.

Each row represents a unique SKU (Stock Keeping Unit). Duplicate product names may exist because products can appear in different package sizes, quantities, discounts, or categories.

Dataset Columns
sku_id → Unique identifier for each product
name → Product name
category → Product category
mrp → Maximum retail price
discountPercent → Discount percentage
discountedSellingPrice → Final selling price after discount
availableQuantity → Inventory quantity available
weightInGms → Product weight in grams
outOfStock → Product availability status
quantity → Number of units per package
Project Workflow
1. Database and Table Creation

Created a PostgreSQL database and designed the table structure.

CREATE TABLE zepto (
  sku_id SERIAL PRIMARY KEY,
  category VARCHAR(120),
  name VARCHAR(150) NOT NULL,
  mrp NUMERIC(8,2),
  discountPercent NUMERIC(5,2),
  availableQuantity INTEGER,
  discountedSellingPrice NUMERIC(8,2),
  weightInGms INTEGER,
  outOfStock BOOLEAN,
  quantity INTEGER
);
2. Data Import

Imported CSV dataset into PostgreSQL using database import tools and prepared data for analysis.

3. Data Exploration

Performed exploratory analysis by:

Counting total records in dataset
Viewing sample records
Checking null values across columns
Identifying distinct product categories
Comparing in-stock and out-of-stock products
Detecting duplicate product names with multiple SKUs
4. Data Cleaning

Performed cleaning operations including:

Removing products with invalid zero pricing values
Converting product prices from paise into rupees
Standardizing pricing data for analysis
5. Business Insights Generated

Generated business insights by solving analytical questions such as:

Top 10 products with highest discount percentage
High-value products currently out of stock
Revenue estimation for each category
Products with high MRP and low discount
Categories with highest average discount percentage
Price per gram analysis for best-value products
Product segmentation into Low, Medium, and Bulk categories
Inventory weight analysis for each category
SQL Concepts Used
CREATE TABLE
SELECT Statements
WHERE Clause
GROUP BY
ORDER BY
HAVING Clause
Aggregate Functions (COUNT, SUM, AVG)
CASE Statements
UPDATE Queries
DELETE Queries
Data Cleaning Techniques
Tools Used
PostgreSQL
SQL
CSV Dataset
GitHub
Project Outcome

This project helped me understand how Data Analysts work with real-world business data by cleaning raw datasets, analyzing inventory patterns, and generating business insights that support decision-making.

It also improved my practical SQL skills and strengthened my Data Analyst portfolio.

Author

Yamini Konchada

Aspiring Data Analyst

Skills: SQL | Python | Power BI | Excel | Data Analytics
