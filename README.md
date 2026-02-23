# Restaurant-Sales-Insights-Reporting-Power-BI
## 🍽️ Restaurant Sales Insights – Power BI

An end-to-end Business Intelligence project analyzing restaurant sales data to uncover actionable insights and support data-driven decision-making using Power BI.

## 📌 Project Overview

This project demonstrates the complete BI workflow starting from raw CSV files to an interactive analytical dashboard.
The objective is to analyze restaurant sales performance, track KPIs, and extract meaningful business insights.

## 📂 Data Source

The dataset was imported from structured CSV files and consists of two main tables:

menu_items (Dimension Table) – Contains item details such as price and category.

order_details (Fact Table) – Contains transactional sales data.

## 🧹 Data Preparation & Cleaning

Data transformation was performed using Power Query:

Data type correction

Removing inconsistencies

Creating calculated column: LineCost = RELATED(menu_items[price])

Establishing proper relationships (Star Schema Model)

## 🗓️ Date Dimension

A dedicated Date Table was created to enhance time intelligence and reporting flexibility.

Extracted Columns:

Year

Month

Quarter

Day

Day of Week

Events

Daily Time Classification

This enables dynamic filtering and advanced time-based analysis.

## 📊 Key Performance Indicators (KPIs)

The following DAX measures were created:

#SelledItems → Total number of sold items

MenuItemsUsed → Distinct menu items sold

MostExpensiveItem → Maximum item price

TotalIncome → Total revenue generated

TotalOrders → Total distinct orders

These KPIs provide a clear overview of sales performance and business activity.

## 📈 Insights & Dashboard Analysis

The interactive dashboard provides:

📅 Total Orders by Date

💰 Total Income by Category

🕒 Total Orders by Daily Time

🔄 Dynamic Measure Switching by Day of Week

📊 Category & Item-Level Analysis

🎛️ Interactive Features

Date Slicer

Category & Item Filters

Dynamic Switching Between Measures

Fully Interactive Visual Experience

## 🏗️ Data Model

The project follows a Star Schema approach:

Fact Table → order_details
Dimension Table → menu_items
Date Table → Custom-built for time intelligence

## 🛠️ Tools & Technologies

Power BI

Power Query

DAX

Data Modeling

CSV Data Sources

## 🎯 Key Takeaways

✔ Building a structured data model
✔ Creating advanced DAX measures
✔ Designing business-driven KPIs
✔ Developing interactive dashboards
✔ Translating raw data into business insights

## 🚀 Future Improvements

Profitability analysis (Cost vs Revenue)

Customer segmentation

Advanced time intelligence (YoY / MoM Growth)

Performance benchmarking
