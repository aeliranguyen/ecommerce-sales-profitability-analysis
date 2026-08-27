# E-commerce Sales & Profitability Analysis

**Business Performance Analysis | E-commerce | Power BI**

---

## Table of Contents

1. [Background & Overview](#-background--overview)
2. [Dataset Description & Data Structure](#-dataset-description--data-structure)
3. [Design Thinking Process](#-design-thinking-process)
4. [Main Process](#-main-process)
5. [Key Insights & Visualizations](#-key-insights--visualizations)
6. [Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

# Background & Overview

## Objective

This project analyzes e-commerce sales performance and profitability using Power BI to help business stakeholders understand:

- How sales and profit are performing over time.
- Which markets and regions contribute the most revenue and profit.
- Which product categories perform well or underperform.
- How profitability changes across markets and categories.
- Where return rates may negatively affect business performance.
- Which markets and categories have strong growth but weak profitability, or vice versa.

The goal is to turn transaction-level sales data into a business performance dashboard that supports data-driven decision-making.

## What is this project about?

This project focuses on understanding the relationship between **sales growth, revenue, profit, profitability and product returns**.

The analysis helps answer key business questions such as:

- How is overall business performance changing over time?
- Which markets generate the highest revenue?
- Which markets generate the highest profit?
- Which markets have the strongest profit margins?
- Which categories contribute most to revenue and profit?
- Are high-growth markets also profitable?
- Which areas have relatively high return rates?
- Where should management focus to improve business performance?

The Power BI report provides an interactive view of these metrics through multiple dashboards.

## Who is this project for?

This analysis can support:

- Data Analysts
- Business Analysts
- Sales Managers
- Commercial Managers
- Category Managers
- Regional / Market Managers
- Business Decision-Makers

---

# Dataset Description & Data Structure

## Data Source

The project uses e-commerce order and return transaction data.

The Power BI model contains the following main business entities:

- `Order`
- `Return`
- `Dim_date`

The report also uses dedicated measures and parameter tables to support dynamic analysis and KPI calculations.

## Data Format

The data is modeled and analyzed in Power BI.

Main analytical components include:

- Order transactions
- Return transactions
- Date dimension
- Calculated measures
- Parameter tables for dynamic metric selection

---

## Data Structure & Relationships

### Main Tables

### 1. Order Table

The `Order` table contains transaction-level sales information used to analyze revenue, profit, market, region and category performance.

Key business attributes used in the report include:

| Field | Description |
|---|---|
| Order | Sales transaction information |
| Market | Business market |
| Region | Geographic region |
| Category | Product category |
| Sub-category | Product sub-category |
| Sales / Revenue | Revenue generated from sales |
| Profit | Profit generated from sales |
| Date | Transaction date |

---

### 2. Return Table

The `Return` table contains information about returned transactions.

Return information is used to evaluate return performance across markets and categories.

The analysis includes:

- Return rate
- Return performance by market
- Return performance by category

---

### 3. Dim_date

The `Dim_date` table provides the date dimension used for time-based analysis.

It supports:

- Year analysis
- Time-series trends
- Year-over-year comparisons
- Sales growth
- Profit growth
- Profit margin trends

---

## Data Model

The Power BI model connects transaction data with the date dimension to allow consistent filtering and time-based analysis.

The model also contains measure and parameter tables to support dynamic KPI and metric selection.

> Add a screenshot of the Power BI Model View here.

Example:

```text
              Dim_date
                  |
                  |
                Order
                  |
               Return
