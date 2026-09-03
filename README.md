# Cafe Sales Data Analysis

## Project Overview

A data cleaning and **Exploratory Data Analysis (EDA)** project using real-world messy cafe sales data with **Python**, focused on uncovering sales patterns and actionable business insights.

## Project Goal

The goal was to transform raw transaction data into a clean, analysis-ready dataset and analyze:

* Sales patterns
* Customer spending behavior
* Top-selling products
* High-performing periods

## Data Quality Issues

The raw `dirty_cafe_sales.csv` dataset contained several data quality problems:

* Incorrect data types
* Missing values, including **2,579** in Payment Method and **3,265** in Location
* Corrupted `ERROR` entries
* Inconsistent categorical labels
* **232 outliers** in Total Spent

## Data Cleaning

Built a data cleaning workflow using **Pandas**:

* Converted numerical and date columns to appropriate data types
* Handled missing values using mean, median, or mode based on the data
* Converted `ERROR` values to `NaN` and handled them appropriately
* Standardized categorical labels using `strip()` and `title()`
* Detected and capped outliers in Total Spent using the **IQR method**
* Validated the final dataset to ensure there were no remaining null values or errors
* Exported the cleaned dataset as `clean_cafe_sales.csv`

## Exploratory Data Analysis

Performed EDA using **Matplotlib** and **Seaborn** to analyze:

* Descriptive statistics and spending distributions
* Numerical outliers
* Correlations between Quantity, Price, and Total Spent
* Monthly and quarterly sales trends
* Top-selling products by month
* Average spending by product
* Price vs. Quantity relationship
* Sales performance by day of the week

## Key Findings

* **Quantity and Total Spent** had a positive correlation of **0.69**
* **October** was the strongest month, while **February** was the weakest
* **Salad** was the top-selling product in most months
* **Weekends** showed the strongest sales performance
* Price and quantity showed **no strong linear relationship**

## Business Insights

The analysis can support business decisions related to sales, inventory, and staffing:

* Increase staffing and inventory during weekends
* Consider targeted promotions during weaker periods such as February
* Maintain sufficient inventory for high-demand products such as Salad
* Use the identified sales patterns as a foundation for future forecasting

## Tech Stack

**Python | Pandas | Matplotlib | Seaborn**

## Key Takeaway

This project demonstrates an end-to-end **Data Analyst workflow**: identifying data quality issues, cleaning and transforming data, handling outliers, performing EDA, and translating findings into actionable business insights.

