# Project : Superstore Sales Data Exploration and Visualization Using Power BI

# Table of content 
- Introduction
* Objective
+ Key Features of the Dashboard
- Tools and Technologies 
- Data Analyis
* Data Modeling
+ Data Analysis (DAX)
- Build Dashboard or report

# Introduction:
In today’s data-driven world, businesses thrive on their ability to harness data for making informed decisions. This project aims to leverage Power BI, a powerful business analytics tool, to analyze and visualize sales data, providing comprehensive insights into sales performance across various dimensions. The project involves creating an interactive dashboard that not only visualizes key sales metrics but also allows stakeholders to explore data dynamically, uncovering trends and patterns that can drive strategic decision-making.

# Objective:
The primary objective of this project is to analyze sales data from an e-commerce business, focusing on understanding sales trends, profit margins, and customer behavior. By creating an interactive Power BI dashboard, we aim to provide a user-friendly platform where users can easily navigate through the data and derive actionable insights.

# Key Features of the Dashboard:
- Sales Overview: Displays total sales, total profit, and average profit per order.
* Sales Trend Analysis: Visualizes sales and profit trends over time.
+ Category and Sub-Category Analysis: Analyzes sales and profit by product category and sub-category.
- Geographical Analysis: Maps sales and profit data by state and city.
* Payment Mode Analysis: Examines sales distribution by different payment modes.
+ Customer Analysis: Identifies top customers by sales and profit.
- Order Details: Provides a detailed view of individual orders.

#  Tools and Technologies:
- Microsoft Power BI
+ DAX Language

# Data Analysis using Power BI:

1. Data Import:
  The first step involves importing the two primary data tables into Power BI: Orders Details and Orders.<br>

- Orders Details Table:
  Fields: Order ID, Amount, Profit, Quantity, Category, Sub-Category, Payment Mode.<br>

- Orders Table:
  Fields: Order ID, Order Date, Customer Name, State, City.

2. Data Cleaning:
  After importing the data, it is essential to clean the data to ensure accuracy and consistency for analysis.

- Remove Duplicates
- Handle Missing Values

3. Data Transformation:
  To facilitate analysis and create useful visualizations, additional transformations and calculations are necessary.

- Create Relationships:

  In the "Model" view, create a relationship between the Orders Details and Orders tables based on the Order ID column.

# Data Modeling:

And then dataset was cleaned and transformed, it was ready to the data modeled.

The sales insights data tables as show below:

# Data Anlysis (DAX):

Key Measures:

1.Total Sales: Create a measure to calculate total sale.
```
Total Sales = SUM('Orders Details'[Amount])
```
2.Total Profit: Create a measure to calculate total profit.
```
Total Profit = SUM('Orders Details'[Profit])
```
3.Average Profit per Order: Create a measure to calculate the average profit per order.
```
Average Profit per Order = DIVIDE([Total Profit], DISTINCTCOUNT('Orders'[Order ID]))
```
4.Profit Margin: Create a measure to calculate the profit margin.
```
Profit Margin = DIVIDE([Total Profit], [Total Sales])
```

# Build Dashboard or report:

!

