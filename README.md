# Executive Business Performance Dashboard – Tableau Project

---

## 1. Business Problem Summary

Businesses generate large volumes of transactional, customer, and operational data, but decision-makers often struggle to convert this information into actionable insights. Revenue growth alone does not provide a complete picture of organizational performance, as profitability, customer behavior, returns, discounting strategies, and operational efficiency all influence business outcomes.

The objective of this Tableau Executive Dashboard is to provide leadership with a consolidated and interactive view of business performance to:

* Monitor sales and profitability trends
* Evaluate regional and product performance
* Analyze customer behavior and segmentation
* Assess the impact of discounting strategies
* Track returns and delivery performance
* Identify business risks and growth opportunities
* Support strategic decision-making using data-driven insights

---

## 2. Dataset Description

The dashboard utilizes transactional business data containing sales, customer, product, geographic, and operational information.

### Dataset Features

| Category  | Description                            |
| --------- | -------------------------------------- |
| Orders    | Individual customer transactions       |
| Sales     | Revenue generated from transactions    |
| Profit    | Profit earned on each transaction      |
| Products  | Product categories and sub-categories  |
| Customers | Customer information and segmentation  |
| Geography | Region, state, and market information  |
| Shipping  | Order fulfillment and delivery details |
| Returns   | Returned order information             |
| Discounts | Discounts applied to orders            |

### Key Fields Used

* Order ID
* Order Date
* Ship Date
* Customer ID
* Customer Segment
* Region
* State
* Category
* Sub-Category
* Sales
* Profit
* Quantity
* Discount
* Return Status

---

## 3. Tableau Workbook Description

The Tableau workbook was designed as an executive business intelligence dashboard that integrates multiple analytical perspectives into a single reporting environment.

### Workbook Objectives

The dashboard enables users to:

* Analyze business performance over time
* Compare regional and geographic performance
* Evaluate category and sub-category profitability
* Understand customer segment behavior
* Assess operational efficiency
* Monitor product returns
* Evaluate pricing and discount strategies

### Major Dashboard Sheets

* Executive KPI Dashboard
* Sales Trend Analysis
* Regional Performance Dashboard
* Geographic Sales Analysis
* Category Profitability Dashboard
* Customer Segment Analysis
* Discount Impact Analysis
* Return Analysis Dashboard
* Shipping Performance Dashboard

---

## 4. Calculated Fields Created

The following calculated fields were created to support advanced business analysis:

| Calculated Field      | Formula                                                                                          | Business Purpose                       |
| --------------------- | ------------------------------------------------------------------------------------------------ | -------------------------------------- |
| Profit Margin         | `([Profit]/[Sales])*100`                                                                         | Measure profitability efficiency       |
| Cost                  | `[Sales]-[Profit]`                                                                               | Estimate operating cost                |
| Average Order Value   | `SUM([Sales])/COUNT([Order ID])`                                                                 | Measure customer spending behavior     |
| Return Rate           | `SUM([Returned Orders])/COUNT([Order ID])`                                                       | Monitor return performance             |
| Delivery Days         | `DATEDIFF('day',[Order Date],[Ship Date])`                                                       | Calculate shipping duration            |
| Shipping Delay Bucket | `IF [Delivery Days]<=2 THEN "Fast" ELSEIF [Delivery Days]<=5 THEN "Standard" ELSE "Delayed" END` | Categorize delivery performance        |
| Discount Category     | Custom discount bands                                                                            | Analyze pricing strategy effectiveness |
| Profitability Segment | Profit grouping logic                                                                            | Classify business performance          |

---

## 5. Dashboard Components

The dashboard contains multiple visual components designed to answer specific business questions.

| Dashboard Component       | Visualization Type        |
| ------------------------- | ------------------------- |
| Sales Trend               | Line Chart                |
| Regional Performance      | Horizontal Bar Chart      |
| Geographic Analysis       | Filled Map                |
| Category Profitability    | Heatmap/Bubble Chart      |
| Customer Segment Analysis | Bar Chart                 |
| Discount Impact           | Scatter Plot              |
| Return Analysis           | Bar Chart                 |
| Shipping Performance      | Distribution/Bucket Chart |
| Executive KPIs            | KPI Cards                 |

### KPI Measures Displayed

* Total Sales
* Total Profit
* Profit Margin
* Total Orders
* Average Order Value
* Return Rate
* Average Delivery Time

---

## 6. Filters and Interactions Used

### Dashboard Filters

The dashboard includes interactive filters for:

* Date Range
* Region
* State
* Customer Segment
* Category
* Sub-Category
* Return Status
* Shipping Performance Category

### Interactive Features

The following Tableau interactions were implemented:

* Filter Actions
* Highlight Actions
* Cross-filtering
* Interactive Tooltips
* Drill-down Analysis
* Dynamic KPI Updates
* Dashboard Navigation Actions

---

## 7. Key Business Insights

### Sales Trend

Sales exhibit clear seasonal and temporal patterns that can support forecasting and inventory planning.

### Regional Performance

Certain regions generate substantial revenue but deliver lower profitability, indicating operational inefficiencies.

### Product Profitability

High-selling product categories are not always the most profitable categories.

### Customer Segment Behavior

Customer segments demonstrate varying levels of profitability and purchasing behavior.

### Discount Impact

Increasing discounts tend to reduce profit margins and overall business profitability.

### Shipping Performance

Shipping performance varies across customer groups and geographic regions.

### Return Patterns

Returns are concentrated within specific product groups, suggesting opportunities for quality improvement.

### Business Opportunities

High-performing customer segments and profitable categories represent strategic growth opportunities.

---

## 8. Dashboard Story Summary

The dashboard presents an integrated business narrative by connecting commercial performance, customer behavior, and operational efficiency.

The analysis demonstrates that:

* Revenue growth alone is insufficient to measure business success.
* Profitability differs significantly across regions, products, and customers.
* Discounting strategies influence overall financial performance.
* Operational performance impacts customer satisfaction and returns.
* Business risks emerge when profitability is concentrated in limited segments.
* Strategic investment should focus on profitable products, regions, and customer groups.

The dashboard supports executive decision-making by providing a holistic view of business performance and highlighting areas requiring intervention.

---

## 9. Assumptions and Limitations

### Assumptions

* Transactional data is complete and accurate.
* Profit values accurately represent business profitability.
* Return records are correctly maintained.
* Shipping dates reflect actual delivery performance.
* Customer segmentation is appropriately defined.

### Limitations

* The dashboard provides descriptive analytics only.
* Predictive forecasting models are not included.
* External market conditions are not considered.
* Customer lifetime value analysis is not performed.
* Supply chain performance metrics are limited.
* Competitive benchmarking data is unavailable.

---

## 10. Screenshots Included

The project submission includes screenshots of the following dashboard components:

1. Executive Dashboard Overview
2. Sales Trend Analysis
3. Regional Performance Dashboard
4. Geographic Sales Map
5. Category Profitability Dashboard
6. Customer Segment Analysis
7. Discount Impact Analysis
8. Return Analysis Dashboard
9. Shipping Performance Dashboard
10. Executive KPI Summary Panel

---

### Tools Used

* Tableau Desktop
* Tableau Calculated Fields
* Interactive Dashboard Actions
* Business Intelligence and Data Visualization Techniques
* Descriptive Analytics and KPI Analysis
