# Restaurant-Sales-Insights-Reporting-Power-BI
#🍽️ Restaurant Sales Insights – Power BI

An end-to-end Business Intelligence project analyzing restaurant sales data using Power BI to generate actionable insights and interactive dashboards.

#📌 Project Overview

This project focuses on transforming raw restaurant sales data into meaningful business insights.
The workflow covers data cleaning, data modeling, KPI development, and interactive reporting to support data-driven decision-making.

#📂 Data Source

The dataset was imported from CSV files and consists of two main tables:

menu_items (Dimension Table)

order_details (Fact Table)

#🧹 Data Preparation

Data cleaning and transformation were performed using Power Query:

Handled missing and inconsistent values

Ensured proper data types

Created calculated column LineCost using item price

Built relationships between fact and dimension tables

#📅 Date Dimension Table

A dedicated Date Table was created to enhance time-based analysis, including the following columns:

Year

Month

Quarter

Day

Day of Week

Events

Daily Time Classification

This enables flexible time intelligence and filtering capabilities.

#📊 Key Performance Indicators (KPIs)

The following measures were created using DAX:

#SelledItems = COUNT('order_details(fact)'[order_details_id])

MenuItemsUsed = DISTINCTCOUNT('order_details(fact)'[item_id])

MostExpensiveItem = MAX('menu_items(dim)'[price])

TotalIncome = SUM('order_details(fact)'[LineCost])

TotalOrders = DISTINCTCOUNT('order_details(fact)'[order_id])

These KPIs help measure:

Total items sold

Unique menu items used

Maximum item price

Total revenue

Total number of orders

#📈 Insights & Analysis

The dashboard provides the following analytical insights:

📅 Total Orders by Date

💰 Total Income by Category

🕒 Total Orders by Daily Time

📊 Dynamic Measure Switching by Day of Week

🔄 Switch Analysis by Category & Item Name

🎛️ Interactive Features

Category & Item-level filtering

Date slicer for time-based analysis

Dynamic switching between measures

Fully interactive dashboard experience

#🛠️ Tools & Technologies

Power BI

Power Query

DAX

Data Modeling

#🚀 Business Value

This project demonstrates:

Building a clean star schema model

Creating dynamic KPIs using DAX

Designing interactive dashboards

Extracting meaningful business insights from raw data
