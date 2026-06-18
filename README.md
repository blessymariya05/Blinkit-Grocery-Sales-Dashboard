# Blinkit Grocery Sales Dashboard | Power BI

## Project Overview

This project focuses on analyzing Blinkit grocery sales data and creating an interactive dashboard using Microsoft Power BI.

The dashboard provides insights into sales performance, product categories, outlet characteristics, and customer ratings. The project demonstrates data cleaning, transformation, DAX calculations, and data visualization techniques used for business intelligence analysis.

## Objectives

The main objectives of this project are:

- Analyze overall grocery sales performance
- Identify top-performing product categories
- Understand outlet-level performance
- Analyze sales distribution based on outlet size and location
- Evaluate customer ratings
- Build an interactive dashboard for business insights

---

## Dataset Description

The dataset contains Blinkit grocery sales information with details about products, outlets, sales, and ratings.

### Dataset Columns

- Item Fat Content
- Item Identifier
- Item Type
- Outlet Establishment Year
- Outlet Identifier
- Outlet Location Type
- Outlet Size
- Outlet Type
- Item Visibility
- Item Weight
- Sales
- Rating

---

## Tools and Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel

---

## Data Cleaning and Transformation

Data preprocessing was performed using Power Query.

The following transformation was performed:

### Item Fat Content Standardization

The dataset contained inconsistent category values:

- low fat
- LF
- Low Fat
- reg
- Regular

These values were standardized into two categories:

- Low Fat
- Regular

This helped remove duplicate categories and ensured accurate analysis during visualization.

---

## DAX Measures Created

The following measures were created to calculate key performance indicators:

### Total Sales

```DAX
Total Sales = SUM('BlinkIT Grocery Data'[Sales])
Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])
Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
No of Items = COUNTROWS('BlinkIT Grocery Data')
