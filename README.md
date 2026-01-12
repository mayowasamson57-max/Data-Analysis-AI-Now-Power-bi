# Data-Analysis-AI-Now-Power-bi
Data analysis project in power BI

# 📊 D LITE Electronics Sales Analysis  
*Excel & Power BI Project Report*

**Author:** Mayowa Samson Popoola  
**Date:** January 2026  
**Tools:** Microsoft Excel, Power BI  
**Dataset:** `Sales_Details.xlsx`

---

## 📌 Project Overview

D LITE Electronics operates across major regions in Nigeria. However, the company’s sales data is inconsistent and contains errors.  
This project focuses on:

- Cleaning messy and inconsistent data  
- Analyzing sales performance by region, product, time, and promotion  
- Visualizing insights using **Excel** and **Power BI**  
- Producing management-ready insights for decision-making  

The goal is to transform raw data into **actionable business intelligence**.

## 🎯 Objective

Build an interactive Business Intelligence solution in **Power BI** to:

- Model and clean data with Power Query  
- Create DAX measures  
- Visualize trends and performance  
- Enable management to explore insights dynamical

---

## 🗂 Dataset Description

The dataset contains the following key fields:

| Column | Description |
|--------|-------------|
| Order ID | Unique order identifier |
| Order Date | Date of transaction |
| Unit Cost | Cost per unit |
| Price | Selling price per unit |
| Order Qty | Quantity sold |
| Sales | Total sales amount |
| Channel | Sales channel |
| Promotion Name | Promotion applied |
| Product Name | Product sold |
| Product Sub Category | Detailed category |
| Product Category | Main category |
| State | Nigerian state |
| Zone | Nigerian region |

---

## 🔄 Data Preparation (Power Query)

Steps in Power BI:

1. **Get Data → Excel**  
2. Opened **Power Query Editor**  
3. Actions performed:
   - Trimmed text columns  
   - Standardized Zone & Product fields  
   - Ensured Sales is numeric  
   - Removed duplicates  

> 📸 Screenshot — Power Query Cleaning  
> `![Power Query](../screenshots/powerbi_model.png)`

---

## 🧮 DAX Measures

```DAX
Total Sales = SUM(Sales_Details[Sales])

Total Orders = COUNT(Sales_Details[Order ID])

Average Order Value = DIVIDE([Total Sales], [Total Orders])

Total Quantity = SUM(Sales_Details[Order Qty])

