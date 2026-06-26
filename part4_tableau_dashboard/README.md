# Task 1: Connect and Inspect Data

## Data Inspection and Assumptions

The dataset was successfully imported into Tableau and all fields were reviewed before creating the dashboard.

### Field Classification

**Date Fields**
- order_date
- ship_date

**Geographic Fields**
- region
- state
- city

**Categorical Fields**
- order_id
- customer_id
- customer_segment
- category
- sub_category
- product_name
- ship_mode
- campaign_channel

**Numerical Measures**
- sales
- quantity
- discount
- profit
- delivery_days
- customer_rating

**Binary Field**
- return_flag

### Assumptions

- Sales and Profit values are assumed to be recorded in the same currency.
- Each row represents one individual order transaction.
- The return_flag field accurately identifies returned orders.
- delivery_days represents the number of days between the order date and successful delivery.
- Customer ratings are assumed to be measured on a consistent rating scale.
- Geographic fields are assumed to be complete and correctly assigned.
- Missing values, if any, are assumed to have minimal impact on dashboard-level business insights.
- No duplicate order records were intentionally removed, as the objective of this assignment is dashboard reporting rather than data cleaning.

-------------------

# README Requirements

## Business Problem Summary

A retail company's leadership team needs a centralized executive dashboard to monitor overall business performance. The objective is to analyze sales, profitability, customer behavior, shipping performance, discount impact, and product returns to identify business opportunities and operational risks.

The dashboard is designed to help decision-makers answer key business questions such as:

* How are sales changing over time?
* Which regions generate the highest sales and profit?
* Which product categories are most profitable?
* How do discounts affect profitability?
* Which customer segments contribute the most revenue?
* Are shipping delays affecting business performance?
* Which products or regions experience the highest return rates?

The dashboard provides an interactive and executive-friendly view for strategic decision making.

-------

# Dataset Description

The dataset contains historical retail sales transactions with information including:

* Order ID
* Order Date
* Ship Date
* Customer Segment
* Region
* State
* Category
* Sub-Category
* Sales
* Profit
* Discount
* Quantity
* Shipping Mode
* Return Flag

These fields were used to create business KPIs, visualizations, and interactive filters.

---

# Tableau Workbook Description

The Tableau workbook (`executive_dashboard.twbx`) contains:

* Sales Trend View
* Regional Performance View
* Category Profitability View
* Customer Segment View
* Shipping Performance View
* Discount vs Profit View
* Return Analysis View

These worksheets are combined into a single Executive Dashboard with KPI cards and interactive filters.

--------

# Calculated Fields Created

The following calculated fields were created in Tableau:

### 1. Profit Margin

```
SUM([Profit]) / SUM([Sales])
```

Calculates overall profitability.

------

### 2. Cost

```
SUM([Sales]) - SUM([Profit])
```

Calculates estimated product cost.

-------

### 3. Average Order Value

```
SUM([Sales]) / COUNTD([Order ID])
```

Calculates average sales per order.

--------

### 4. Return Rate

```
SUM([return_flag]) / COUNT([Order ID])
```

Measures the proportion of returned orders.

-------

### 5. Shipping Delay Bucket

```
IF [delivery_days] <= 2 THEN "Fast"
ELSEIF [delivery_days] <= 5 THEN "Standard"
ELSE "Delayed"
END
```

Groups deliveries based on shipping duration.

--------

# Dashboard Components

The executive dashboard includes:

* KPI Card – Total Sales
* KPI Card – Total Profit
* KPI Card – Profit Margin

Visualizations:

* Sales Trend
* Regional Performance
* Category Profitability
* Customer Segment Analysis
* Shipping Performance
* Discount vs Profit
* Return Analysis

-------

# Filters and Interactions Used

Interactive Filters:

* Region
* Category
* Customer Segment

Dashboard Actions:

* Selecting a region filters all dashboard charts.
* Category selections dynamically update related visualizations.
* Filters allow leadership to analyze specific business segments quickly.

------

# Key Business Insights

The dashboard highlights several important business findings:

* Sales trends reveal seasonal fluctuations across the reporting period.
* Some regions consistently outperform others in both sales and profitability.
* Certain product sub-categories generate high revenue but relatively low profit.
* Higher discounts generally reduce overall profitability.
* Customer segments contribute differently to revenue and profit generation.
* Shipping delays vary across shipping modes and may impact customer satisfaction.
* Return rates differ across categories and regions, indicating potential quality or fulfillment issues.
* Executive filters enable deeper investigation into specific markets and customer groups.

-------

# Dashboard Story Summary

The dashboard presents a complete business performance story by connecting multiple operational areas into one interactive view.

Leadership can begin with high-level KPIs before exploring sales trends, regional performance, product profitability, customer segments, shipping efficiency, discount impact, and return behavior.

Rather than viewing isolated charts, the dashboard allows users to identify relationships between different business metrics and uncover opportunities for operational improvement and revenue growth.

---

# Assumptions and Limitations

## Assumptions

* Source data is accurate and complete.
* Profit Margin is calculated using aggregated Sales and Profit.
* Return Flag contains binary values (0 = Not Returned, 1 = Returned).
* Average Order Value is based on unique Order IDs.

## Limitations

* The dashboard is descriptive and does not predict future sales.
* External factors such as marketing campaigns, inflation, competitor actions, and seasonal events are not included.
* Shipping delay categories are based on predefined thresholds.
* Results depend entirely on the quality of the provided dataset.

---

# Screenshots Included

The repository contains the following screenshots:

* `full_dashboard.png` — Complete Executive Dashboard
* `sales_trend_view.png` — Sales Trend Analysis
* `regional_performance_view.png` — Regional Performance
* `category_profitability_view.png` — Category & Sub-Category Profitability
* `filter_interaction_view.png` — Dashboard Filter Interaction

These screenshots demonstrate the functionality and layout of the final Tableau dashboard.

---

# Repository Structure

```
part4_tableau_dashboard/
│
├── data/
│   └── dashboard_sales_data.xlsx
│
├── tableau/
│   └── executive_dashboard.twbx
│
├── outputs/
│   ├── business_insights.md
│   ├── dashboard_story.md
│   └── chart_selection_justification.md
│
├── screenshots/
│   ├── full_dashboard.png
│   ├── sales_trend_view.png
│   ├── regional_performance_view.png
│   ├── category_profitability_view.png
│   └── filter_interaction_view.png
│
└── README.md
```

---

# Tools Used

* Tableau Desktop
* Microsoft Excel
* Git & GitHub
* Markdown
