**🛒 Zepto E-commerce SQL Data Analyst Portfolio Project**


This project is a real-world SQL Data Analyst portfolio project based on an e-commerce inventory dataset inspired by Zepto, one of India’s fast-growing quick-commerce platforms. The project simulates how Data Analysts work with raw business data, perform data cleaning, analyze inventory patterns, and generate business insights using SQL.

This project demonstrates practical SQL skills required in real-world business environments and helps strengthen a Data Analyst portfolio for job opportunities.

---

# Project Overview

The objective of this project is to simulate how Data Analysts in e-commerce and retail companies use SQL to solve business problems.

The project focuses on:

✅ Setting up a structured e-commerce inventory database

✅ Performing Exploratory Data Analysis (EDA) to understand product categories, pricing patterns, and stock availability

✅ Cleaning raw data by removing invalid records and standardizing pricing values

✅ Writing business-focused SQL queries to generate insights related to inventory, revenue, discounts, and stock management

---

# Dataset Overview

The dataset represents product inventory data from an e-commerce platform and simulates a real-world retail inventory system.

Each row represents a unique SKU (Stock Keeping Unit). Duplicate product names may exist because products can appear in different package sizes, discounts, quantities, or categories.

---

# Dataset Columns

* **sku_id** → Unique identifier for each product
* **name** → Product name
* **category** → Product category
* **mrp** → Maximum Retail Price
* **discountPercent** → Discount percentage applied
* **discountedSellingPrice** → Final selling price after discount
* **availableQuantity** → Available stock quantity
* **weightInGms** → Product weight in grams
* **outOfStock** → Product stock availability status
* **quantity** → Number of units per package

---

# Project Workflow

## 1. Database Creation

Created database schema and designed table structure using SQL in PostgreSQL.

```sql id="a8y7fk"
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
```

---

## 2. Data Import

Imported CSV dataset into PostgreSQL database and prepared raw data for analysis.

---

## 3. Data Exploration

Performed exploratory analysis by:

* Counting total records in dataset
* Viewing sample data
* Checking null values
* Identifying distinct product categories
* Comparing in-stock and out-of-stock products
* Detecting duplicate products with multiple SKUs

---

## 4. Data Cleaning

Performed data cleaning operations including:

* Removing invalid records with zero pricing values
* Converting prices from paise into rupees
* Standardizing price data for accurate analysis

---

## 5. Business Analysis

Generated insights by solving analytical business questions related to pricing and inventory management.

---

# Business Queries Performed

* Find top 10 products with highest discount percentage
* Identify high-value products currently out of stock
* Calculate estimated revenue for each product category
* Find products with high MRP and low discount percentage
* Identify top 5 categories with highest average discount
* Calculate price per gram for value comparison
* Group products into Low, Medium, and Bulk categories
* Calculate total inventory weight for each category

---

# SQL Concepts Used

* CREATE TABLE
* SELECT Statements
* WHERE Clause
* GROUP BY
* ORDER BY
* HAVING Clause
* Aggregate Functions (COUNT, SUM, AVG)
* CASE Statements
* UPDATE Queries
* DELETE Queries
* Data Cleaning Techniques

---

# Tools Used

* PostgreSQL
* SQL
* CSV Dataset
* [GitHub](https://github.com?utm_source=chatgpt.com)

---

# Project Outcome

This project improved my understanding of how Data Analysts work with real-world business data by cleaning raw datasets, analyzing inventory patterns, and generating business insights that support decision-making.

It also strengthened my practical SQL knowledge and helped me build a strong portfolio project for Data Analyst roles.

---

# Author

**Yamini Konchada**

Aspiring Data Analyst

**Skills:** SQL | Python | Power BI | Excel | Data Analytics


