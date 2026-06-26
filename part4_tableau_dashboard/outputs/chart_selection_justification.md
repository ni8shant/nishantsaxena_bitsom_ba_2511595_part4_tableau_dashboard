# Task 6: Apply Visualization Design Principles

## Dashboard Objective

The executive dashboard is designed to help retail leadership monitor overall business performance, identify growth opportunities, detect operational risks, and support data-driven decision-making.

The dashboard follows visualization best practices by selecting chart types based on the business question rather than visual appearance.

---

# 1. Sales Trend View

### Business Question
How are sales changing over time?

### Chart Type
Line Chart

### Why this chart?
A line chart is the most appropriate visualization for time-series data because it clearly shows trends, seasonality, and fluctuations in sales across different months.

### Fields Used
- X-axis: Order Date (Month)
- Y-axis: Sales

### Design Principle Applied
- Chronological ordering
- Minimal visual clutter
- Continuous trend visualization

### Mistake Avoided
Did not use bar or pie charts, which are less effective for showing trends over time.

---

# 2. Regional Performance View

### Business Question
Which region generates the highest sales?

### Chart Type
Bar Chart

### Why this chart?
Bar charts make comparisons between regions simple and allow leadership to quickly identify the strongest and weakest performing regions.

### Fields Used
- X-axis: Region
- Y-axis: Sales
- Label: Total Profit
- Color: Region

### Design Principle Applied
- Sorted by Sales
- Clear comparison between categories
- Easy-to-read labels

### Mistake Avoided
Avoided pie charts because they make comparisons between regions more difficult.

---

# 3. Category Profitability View

### Business Question
Which categories and sub-categories contribute the most profit?

### Chart Type
Horizontal Bar Chart

### Why this chart?
Horizontal bars allow long category and sub-category names to remain readable while making profitability comparisons straightforward.

### Fields Used
- Rows: Category, Sub-Category
- Columns: Profit
- Color: Category

### Design Principle Applied
- Descending sort by Profit
- Consistent category colors
- Clear value labels

### Mistake Avoided
Avoided stacked bars and pie charts, which reduce readability for multiple categories.

---

# 4. Shipping Performance View

### Business Question
Which shipping modes experience longer delivery delays?

### Chart Type
Stacked Bar Chart

### Why this chart?
The stacked bar chart compares average delivery days across shipping modes while showing the contribution of different delay buckets.

### Fields Used
- X-axis: Ship Mode
- Y-axis: Average Delivery Days
- Color: Shipping Delay Bucket

### Design Principle Applied
- Consistent color coding
- Clear comparison of shipping modes
- Easy identification of delayed shipments

### Mistake Avoided
Avoided tables because charts communicate delivery performance more effectively.

---

# 5. Return Analysis View

### Business Question
Which categories and regions experience higher return rates?

### Chart Type
Bar Chart

### Why this chart?
Bar charts provide a simple comparison of returned orders across categories and regions, helping identify operational issues.

### Fields Used
- X-axis: Region
- Y-axis: Return Count
- Split by: Category
- Color: Category

### Design Principle Applied
- Easy comparison
- Consistent category colors
- Clear labels

### Mistake Avoided
Avoided pie charts because they are ineffective for comparing many groups.

---

# 6. Customer Segment View

### Business Question
Which customer segment contributes the highest sales and profit?

### Chart Type
Grouped Bar Chart

### Why this chart?
Grouped bars enable direct comparison of customer segments using key business metrics.

### Fields Used
- Customer Segment
- Sales
- Profit

### Design Principle Applied
- Side-by-side comparison
- Consistent formatting
- Clear labels

### Mistake Avoided
Avoided stacked bars that could hide differences between metrics.

---

# 7. Discount vs Profit View

### Business Question
How does discount affect profitability?

### Chart Type
Scatter Plot

### Why this chart?
Scatter plots are ideal for identifying relationships and patterns between two numerical variables.

### Fields Used
- X-axis: Discount
- Y-axis: Profit
- Detail: Order ID
- Color: Category

### Design Principle Applied
- Displays correlation clearly
- Highlights outliers
- Supports business investigation

### Mistake Avoided
Avoided line charts because discount values are not sequential over time.

---

# KPI Cards

### KPIs Displayed
- Total Sales
- Total Profit
- Profit Margin

### Why KPI Cards?
KPI cards provide executives with an immediate overview of business performance before exploring detailed visualizations.

---

# Filters Used

The dashboard includes interactive filters for:

- Region
- Category
- Customer Segment

These filters allow leadership to analyze specific business segments without creating separate dashboards.

---

# Dashboard Interaction

Action filters are enabled so that selecting a value in one visualization filters related charts across the dashboard.

This improves exploratory analysis and allows users to investigate business performance dynamically.

---

# Visualization Design Principles Applied

The dashboard follows several best practices:

- Appropriate chart selection based on business questions
- Clear visual hierarchy
- Minimal clutter
- Consistent color usage
- Readable titles and labels
- Sorted charts for easier comparison
- Interactive filtering
- No misleading scales or unnecessary visual effects
- Focus on business interpretation instead of decorative visuals

---------

# Task 10: Chart Selection 

## Dashboard Objective

The executive dashboard is designed to help retail leadership monitor sales performance, profitability, customer behavior, shipping efficiency, discount impact, and product returns. Each visualization was selected to answer a specific business question while following data visualization best practices.

---

# 1. Sales Trend View

### Business Question
How are sales changing over time?

### Chart Type
Line Chart

### Why this Chart?
A line chart is the best choice for displaying trends over time. It clearly highlights increases, decreases, and seasonal fluctuations in sales.

### Fields Used
- X-Axis: Order Date (Month)
- Y-Axis: Sales
- Filter: Region, Category, Customer Segment, Ship Mode

### Design Principles Applied
- Chronological ordering
- Minimal clutter
- Clear axis labels
- Easy comparison across months

### Mistake Avoided
Did not use a pie chart or stacked bars, which would make trend analysis difficult.

---

# 2. Regional Performance View

### Business Question
Which region generates the highest sales and profit?

### Chart Type
Horizontal Bar Chart

### Why this Chart?
Bar charts are ideal for comparing values across categories. A horizontal layout improves readability for region names.

### Fields Used
- Rows: Region
- Columns: Sales
- Color: Profit
- Label: Sales and Profit

### Design Principles Applied
- Sorted in descending order
- Consistent color scale
- Clear labels

### Mistake Avoided
Avoided using a map because the business goal is comparison rather than geographic navigation.

---

# 3. Category Profitability View

### Business Question
Which categories and sub-categories contribute the most profit?

### Chart Type
Horizontal Bar Chart

### Why this Chart?
Bar charts allow quick comparison of profitability across product categories and sub-categories.

### Fields Used
- Rows: Category / Sub-Category
- Columns: Profit
- Color: Profit
- Label: Profit

### Design Principles Applied
- Descending sort by profit
- Consistent color encoding
- Clear category labels

### Mistake Avoided
Avoided a pie chart because comparing many categories using angles is difficult.

---

# 4. Customer Segment View

### Business Question
Which customer segment contributes the most sales?

### Chart Type
Vertical Bar Chart

### Why this Chart?
Bar charts provide an easy comparison between customer segments.

### Fields Used
- Columns: Customer Segment
- Rows: Sales
- Color: Customer Segment

### Design Principles Applied
- Distinct colors
- Equal-width bars
- Clear labels

### Mistake Avoided
Avoided stacked bars because the goal is direct comparison rather than composition.

---

# 5. Shipping Performance View

### Business Question
Which shipping mode experiences longer delivery delays?

### Chart Type
Bar Chart

### Why this Chart?
A bar chart clearly compares the average shipping delay across different shipping modes.

### Fields Used
- Columns: Ship Mode
- Rows: Average Shipping Delay
- Color: Shipping Delay Bucket

### Design Principles Applied
- Consistent delay categories
- Clear labels
- Sorted values

### Mistake Avoided
Avoided a line chart because shipping modes are categorical, not time-based.

---

# 6. Discount vs Profit View

### Business Question
How does discount affect profitability?

### Chart Type
Scatter Plot

### Why this Chart?
Scatter plots are ideal for identifying relationships, clusters, and outliers between two numerical variables.

### Fields Used
- X-Axis: Discount
- Y-Axis: Profit
- Detail: Order ID
- Color: Category

### Design Principles Applied
- Individual marks for each order
- Color grouping by category
- No unnecessary trend distortions

### Mistake Avoided
Avoided line charts because discounts are independent observations, not sequential data.

---

# 7. Return Analysis View

### Business Question
Which regions, categories, or customer segments experience the highest return rate?

### Chart Type
Horizontal Bar Chart

### Why this Chart?
Bar charts allow quick comparison of return counts across business categories.

### Fields Used
- Rows: Category (or Region)
- Columns: Returned Orders
- Color: Return Rate

### Design Principles Applied
- Descending sorting
- Consistent color usage
- Easy comparison

### Mistake Avoided
Avoided pie charts because multiple categories are easier to compare using bars.

---

# KPI Cards

### Business Question
What are the most important business metrics at a glance?

### KPI Cards Included
- Total Sales
- Total Profit
- Average Profit Margin

### Why KPI Cards?
KPI cards provide executives with immediate access to high-level business performance without requiring interaction.

### Design Principles Applied
- Large readable font
- High visual hierarchy
- Positioned at the top of the dashboard

---

# Interactive Filters

The dashboard includes interactive filters for:

- Region
- Category
- Customer Segment

These filters allow users to analyze business performance across different dimensions while keeping all charts synchronized.

---

# Dashboard Action Filter

An action filter has been configured so that selecting a region in the Regional Performance chart updates the remaining dashboard views automatically.

This enables users to perform detailed regional analysis without navigating to separate dashboards.

---

# Overall Visualization Design Principles

The dashboard follows the following visualization best practices:

- Appropriate chart selection for each business question
- Clear visual hierarchy
- Minimal visual clutter
- Consistent color palette
- Readable titles and labels
- Logical sorting of categories
- Interactive filters for exploration
- Accurate scales without distortion
- Focus on business decision-making rather than decoration

These design choices ensure that leadership can quickly identify performance trends, operational risks, and business opportunities from a single executive dashboard.