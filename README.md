# Data-Analysis
Analysis and Insights on Amazon Sales Data
Sure! Here’s a comprehensive report summarizing the steps taken, key findings, and insights from the initial data analysis:

---
# Amazon Sales Report Analysis

## Introduction
This report provides a comprehensive analysis of the Amazon sales dataset, focusing on sales performance, product distribution, fulfillment methods, customer segmentation, and geographical analysis. The objective is to extract actionable insights to support business decision-making.

## Data Cleaning

### Initial Inspection
The dataset contains various columns including order details, product information, shipping details, and fulfillment methods. The initial inspection revealed several columns with missing values, particularly:
- `currency` and `Amount`
- `ship-city`, `ship-state`, `ship-postal-code`, and `ship-country`
- `fulfilled-by`
- `New` and `PendingS`

### Cleaning Steps
1. **Dropped Irrelevant Columns**: Columns `New` and `PendingS` were dropped due to a very high number of missing values.
2. **Handled Missing Values**:
   - Investigated the relationship between missing `currency`/`Amount` and order `Status`. Most missing values corresponded to `Cancelled` orders.
   - Removed rows with missing shipping details.
3. **Removed `Cancelled` Orders**: These orders do not contribute to sales and were removed from the dataset.

## Exploratory Data Analysis (EDA)
### Summary Statistics
The cleaned dataset was summarized to understand the distribution and key characteristics of the data. Here are some initial findings:

- **Order Status**: Orders are primarily in `Shipped`, `Shipped - Delivered to Buyer`, and a few in `Pending`.
- **Fulfillment Methods**: The dataset includes orders fulfilled by both Amazon and merchants, with various shipping service levels (Standard, Expedited).

### Sales Overview
An analysis of sales performance over time is crucial to identify trends and patterns. This involves:
- **Monthly/Quarterly Sales Trends**: Identifying peak sales periods.
- **Revenue Analysis**: Understanding revenue contributions from different products and categories.

### Product Analysis
Understanding product preferences involves analyzing:
- **Product Categories**: Identifying popular product categories.
- **Sizes and Quantities**: Determining which sizes and quantities are most frequently sold.

### Fulfillment Analysis
Investigating fulfillment methods includes:
- **Effectiveness of Fulfillment Methods**: Comparing delivery times and order accuracy between Amazon and merchant fulfillment.
- **Shipping Service Levels**: Analyzing the distribution and performance of different shipping service levels.

### Customer Segmentation
Segmenting customers based on:
- **Buying Behavior**: Frequency of purchases, average order value.
- **Geographical Location**: Sales distribution across cities and states to identify key markets.

### Geographical Analysis
Exploring the geographical distribution of sales:
- **Top Cities and States**: Identifying regions with the highest sales volume.
- **Regional Preferences**: Understanding product preferences by region.

## Insights and Recommendations

### Key Insights
1. **Sales Trends**: Identify peak sales periods to optimize inventory and marketing strategies.
2. **Popular Products**: Focus on high-demand product categories and sizes to enhance inventory management.
3. **Fulfillment Efficiency**: Improve fulfillment methods and shipping service levels to ensure timely and accurate deliveries.
4. **Customer Segmentation**: Tailor marketing efforts based on customer buying behavior and geographical location.

### Recommendations
1. **Optimize Sales Strategies**: Utilize sales trends to plan promotions and discounts during peak periods.
2. **Improve Inventory Management**: Ensure sufficient stock of popular products and sizes to meet demand.
3. **Enhance Customer Service**: Focus on improving delivery times and accuracy to increase customer satisfaction.
4. **Targeted Marketing**: Develop targeted marketing campaigns based on customer segments and regional preferences.

---

By conducting this analysis, valuable insights can be leveraged to optimize business operations, enhance customer experience, and drive revenue growth. This report provides a foundation for further detailed analysis and strategic planning.
