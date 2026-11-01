# Retail Inventory & Demand Analysis Using Python

A Python-based retail analytics project exploring sales performance, product demand, inventory levels, seasonal trends, promotional activity, and regional revenue patterns to identify business insights and support better inventory management decisions.

## 1. Project Overview

This project analyzes retail store inventory and demand data to understand sales performance and inventory management patterns across different products, categories, stores, and regions.

The analysis focuses on identifying high-performing product categories, evaluating regional revenue contributions, examining seasonal demand patterns, and highlighting potential inventory shortages and surpluses.

Using Python, the project applies data cleaning, feature engineering, exploratory data analysis (EDA), statistical analysis, and data visualization to translate raw retail data into meaningful business insights.

## 2. Business Objectives

- Analyze overall retail revenue and sales performance.
- Identify top-performing and low-performing product categories.
- Compare revenue contributions across regions and stores.
- Examine inventory levels against customer demand.
- Identify products and categories with potential inventory shortages.
- Understand seasonal variations in demand.
- Explore the relationship between promotions, discounts, and sales.
- Provide data-driven recommendations for inventory planning and business decisions.

## 3. Dataset Information

| Attribute | Details |
|---|---|
| Dataset Name | Retail Store Inventory Forecasting Dataset |
| Source | Kaggle |
| Domain | Retail Analytics and Inventory Management |
| File Format | CSV |
| Number of Records | 76,000 |
| Original Columns | 16 |
| Date Range | January 2022 – January 2024 |

**Key Features:**

- Date
- Store ID
- Product ID
- Category
- Region
- Inventory Level
- Units Sold
- Units Ordered
- Price
- Discount
- Weather Condition
- Promotion
- Competitor Pricing
- Seasonality
- Epidemic
- Demand

*Note: The dataset is synthetic and is used for analytical and educational purposes. Findings represent patterns within the supplied dataset and should not be interpreted as actual retail business performance.*

## 4. Tools and Technologies

- **Python** – Data analysis and processing
- **Pandas** – Data manipulation and cleaning
- **NumPy** – Numerical operations and feature engineering
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Google Colab** – Development environment

## 5. Project Workflow

### Stage 1: Data Understanding
- Imported the dataset into Python.
- Examined dataset dimensions, column names, and data types.
- Reviewed numerical and categorical variables.
- Used descriptive statistics to understand data distributions.

### Stage 2: Data Cleaning and Preprocessing
- Checked for missing values.
- Identified duplicate records.
- Converted the Date column into datetime format.
- Extracted year, month, and day features.
- Standardized categorical text values.
- Checked numerical columns for negative and invalid values.
- Identified potential outliers using the Interquartile Range (IQR) method.
- Retained valid extreme observations rather than removing them automatically.

### Stage 3: Feature Engineering

Created additional variables to support business analysis:

- **Gross Revenue:** Units Sold × Price
- **Discount Amount:** Gross Revenue × Discount Percentage
- **Net Revenue:** Gross Revenue − Discount Amount
- **Inventory Gap:** Inventory Level − Demand
- **Potential Shortfall:** Demand exceeding Inventory Level
- **Inventory Surplus:** Inventory exceeding Demand
- **Inventory Status:** Classified records into Potential Shortage, Inventory Balanced, and Inventory Surplus.
- Extracted month names for seasonal analysis.

### Stage 4: Exploratory Data Analysis (EDA)

Analyzed:
- Overall revenue and sales performance.
- Yearly and monthly revenue trends.
- Category-wise and product-wise performance.
- Regional and store-level revenue.
- Inventory levels and demand patterns.
- Seasonal demand variations.
- Promotional and discount performance.
- Competitor pricing comparisons.
- Correlations between numerical variables.
- Distribution, skewness, kurtosis, and outliers.

## 6. Key Business Findings

### Overall Performance

| KPI | Result |
|---|---:|
| Total Net Revenue | Approximately 412.59 Million |
| Total Units Sold | 6,750,876 |
| Total Demand | 7,928,104 |
| Average Product Price | 67.73 |
| Average Discount | 9.09% |
| Total Records | 76,000 |

### Category Performance

- **Groceries** generated the highest net revenue of approximately 152.96 million, contributing 37.07% of total revenue.
- **Furniture** ranked second with approximately 100.89 million in revenue.
- **Toys** recorded the lowest category revenue at approximately 21.66 million.
- Groceries also recorded the highest sales volume.

### Regional Performance

- **North** was the leading region, contributing approximately 154.14 million or 37.36% of total revenue.
- East contributed 21.63%.
- West contributed 20.75%.
- South recorded the lowest revenue contribution at 20.26%.

### Product Performance

- Product P0014 generated the highest revenue at approximately 33.54 million.
- Product P0007 recorded the highest sales volume, with 379,709 units sold.
- Product P0001 recorded the lowest revenue at approximately 12.67 million.

### Inventory and Demand Analysis

- 86.06% of records were classified as Inventory Surplus.
- 13.68% were classified as Potential Shortage.
- 0.26% were classified as Inventory Balanced.
- Groceries recorded the highest cumulative potential inventory shortfall, followed by Clothing.

### Seasonal Demand

- Summer recorded the highest average demand at approximately 112.86 units.
- Spring recorded the lowest average demand at approximately 97.70 units.
- August had the highest monthly average demand at approximately 119.80 units.

### Promotion Analysis

- Records with promotions had average sales of approximately 103.10 units.
- Records without promotions had average sales of approximately 81.83 units.
- Promotional records also had higher average demand.

These are observational differences and do not establish that promotions caused higher sales.

## 7. Business Recommendations

1. **Improve Inventory Planning:** Monitor products with recurring potential inventory shortages and review replenishment requirements.
2. **Optimize Category-Level Stock:** Pay particular attention to Groceries and Clothing, which showed higher cumulative potential shortfalls.
3. **Strengthen Regional Strategies:** Investigate the factors contributing to North's stronger revenue performance and identify opportunities to improve South's performance.
4. **Plan for Seasonal Demand:** Consider increasing inventory readiness ahead of periods with higher observed demand, particularly summer.
5. **Evaluate Promotional Performance:** Monitor sales and revenue during promotional periods to assess whether discounts are commercially beneficial.
6. **Review Inventory Surplus:** Investigate products with consistently high inventory relative to demand to reduce potential overstocking.

## 8. Limitations

- The dataset is synthetic and may not represent actual retail business conditions.
- The analysis identifies associations and patterns, not causal relationships.
- Potential inventory shortages are calculated by comparing inventory

  👩‍💻 Author

Maathangi

Aspiring Data Analyst | Microsoft Excel | SQL | Power BI | Python

🔗 GitHub: https://github.com/Maathangi1412

🔗 LinkedIn: www.linkedin.com/in/maathangip
