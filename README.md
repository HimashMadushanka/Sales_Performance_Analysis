# Sales Data Analysis Project

## 📊 Project Overview
A comprehensive analysis of sales data to uncover business insights, identify trends, and provide data-driven recommendations for strategic decision-making.

## 🎯 Business Objectives
- Analyze sales performance across different dimensions
- Identify profitable products and customer segments
- Understand geographic distribution of sales
- Optimize shipping and operational efficiency
- Provide actionable insights for business growth

## 📁 Project Structure
sales_analysis/
├── data/
│ ├── raw/sales_data.csv # Original dataset
│ └── processed/cleaned_sales_data.csv # Processed data
├── notebooks/
│ └── sales_analysis.ipynb # Main analysis notebook
├── reports/
│ └── figures/ # Generated visualizations
└── README.md # Project documentation


## 📈 Dataset Information

### Basic Statistics
- **Total Records**: [Number of rows from df.shape]
- **Features**: 20+ columns including sales, profit, customer info, product details
- **Time Period**: 2011 data (as per year column)
- **Data Quality**: [Mention any missing values found]

### Key Columns Analyzed
- `order_id`, `order_date`, `ship_date`
- `customer_name`, `segment`, `state`, `country`, `region`
- `product_id`, `category`, `sub_category`, `product_name`
- `sales`, `quantity`, `discount`, `profit`, `shipping_cost`
- `order_priority`, `year`

## 🔧 Data Preprocessing

### Steps Performed
1. **Date Conversion**: Converted `order_date` and `ship_date` to datetime format
2. **Shipping Days Calculation**: Derived `shipping_days` from order and ship dates
3. **Data Cleaning**: Removed commas from sales column and converted to numeric
4. **Feature Engineering**: Created `order_month` for time series analysis

## 📊 Analysis Performed

### 1. Sales Analysis
- **Monthly Sales Trends**: Identified seasonal patterns and growth trends
- **Customer Segment Distribution**: Analyzed sales across Consumer, Corporate, and Home Office segments
- **Regional Performance**: Compared sales across different geographic regions
- **Product Category Analysis**: Breakdown of sales across Office Supplies, Furniture, and Technology

### 2. Profitability Analysis
- **Profit by Category**: Identified most and least profitable product categories
- **Profit Margins**: Calculated average profit margins per category
- **Discount Impact**: Analyzed relationship between discounts and profitability

### 3. Customer Insights
- **Top Customers**: Identified highest-spending customers
- **Customer Segmentation**: Analyzed buying patterns across different segments

### 4. Geographic Analysis
- **Top Countries**: Ranked countries by sales volume
- **Top States**: Identified highest-performing states/regions

### 5. Operational Analysis
- **Shipping Modes**: Distribution across Standard Class, Second Class, First Class, Same Day
- **Order Priorities**: Analysis of Critical, High, Medium, Low priority orders
- **Shipping Efficiency**: Correlation between shipping days and profitability

### 6. Advanced Analytics
- **Correlation Analysis**: Relationships between sales, quantity, discount, profit, shipping
- **Time Series Analysis**: Monthly trends for sales, profit, quantity, and order count
- **Market Analysis**: Performance across different markets (Africa, APAC, EMEA, EU, LATAM, US)

## 📈 Key Findings

### Performance Metrics
- **Total Sales**: $[Insert total sales from analysis]
- **Total Profit**: $[Insert total profit from analysis]
- **Average Order Value**: $[Insert AOV from analysis]
- **Profit Margin**: [Insert margin]%
- **Average Shipping Days**: [Insert average] days

### Top Insights
1. **Most Profitable Category**: [Category name] with [profit margin]% margin
2. **Best Performing Region**: [Region name] contributing [percentage]% of total sales
3. **Optimal Shipping**: [Shipping mode] provides best balance of cost and delivery time
4. **Customer Segments**: [Segment name] shows highest average order value
5. **Seasonal Trends**: [Month/Season] shows peak sales performance

## 📋 Key Performance Indicators (KPIs)

| Metric | Value | Insight |
|--------|-------|---------|
| Total Sales | $[Value] | Overall business volume |
| Total Profit | $[Value] | Business profitability |
| Order Count | [Value] | Transaction frequency |
| Average Order Value | $[Value] | Customer spending pattern |
| Profit Margin | [Value]% | Business efficiency |
| Shipping Efficiency | [Value] days | Operational performance |

## 🎨 Visualizations Generated

### Main Dashboard (3x3 Grid)
1. Monthly Sales Trend Line Chart
2. Customer Segment Distribution Pie Chart
3. Regional Sales Performance Bar Chart
4. Product Category Sales Bar Chart
5. Product Category Profit Bar Chart
6. Shipping Mode Distribution Bar Chart
7. Order Priority Distribution Bar Chart
8. Market Analysis Bar Chart
9. Shipping Days Distribution Histogram

### Advanced Analysis (2x3 Grid)
1. Profit vs Discount Scatter Plot
2. Sales vs Profit Scatter Plot
3. Quantity vs Sales Scatter Plot
4. Sales vs Shipping Cost Scatter Plot
5. Profit Margin by Category Bar Chart
6. Shipping Days vs Profit Scatter Plot

### Additional Visualizations
- Correlation Matrix Heatmap
- Time Series Trends (4-panel chart)

## 🛠️ Technical Implementation

### Libraries Used
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from datetime import datetime