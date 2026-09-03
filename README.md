Cafe Sales Data Analysis

A complete data cleaning and exploratory data analysis (EDA) project using real-world messy cafe sales data to uncover actionable business insights with Python.

The Idea

The goal was to transform raw cafe transaction data into a clean, analysis-ready dataset and use it to identify sales patterns, customer spending behavior, top-selling products, and high-performing periods.

The Problem

The raw dataset dirty_cafe_sales.csv contained several data quality issues:

* Wrong data types in numerical and date columns
* Missing values, including 2,579 in Payment Method and 3,265 in Location
* Corrupted entries containing ERROR
* Inconsistent categorical labels
* 232 outliers in Total Spent

The Solution

Built a data cleaning pipeline using Pandas:

* Converted numerical columns and Transaction Date to appropriate data types
* Removed records with missing critical fields
* Imputed missing numerical values using mean/median based on distribution
* Imputed categorical values using the mode
* Standardized categorical labels using strip() and title()
* Converted ERROR values to NaN and handled them using appropriate imputation methods
* Detected and capped outliers in Total Spent using the IQR method
* Verified the dataset contained zero null values and no remaining errors
* Exported the cleaned dataset as clean_cafe_sales.csv

Exploratory Data Analysis

Performed EDA using Matplotlib and Seaborn to analyze:

* Descriptive statistics and spending distributions
* Outliers across numerical variables
* Correlations between Quantity, Price, and Total Spent
* Monthly and quarterly sales trends
* Top-selling products by month
* Average spending by product
* Price vs. Quantity relationship
* Sales performance by day of the week

Key Findings

* Quantity and Total Spent showed a positive correlation of 0.69
* October was the strongest month, while February was the weakest
* Salad was the top-selling item in most months
* Weekends showed the strongest sales performance
* Price and quantity showed no strong linear relationship

Business Insights

The findings can support sales forecasting, inventory planning, and staffing decisions.

* Increase staffing and inventory during weekends
* Consider targeted promotions during weaker periods such as February
* Maintain sufficient inventory of high-demand products such as Salad
* Use the identified sales patterns as a foundation for future forecasting models

Tech Stack

Python | Pandas | Matplotlib | Seaborn

Key Takeaway

This project demonstrates an end-to-end Data Analyst workflow: identifying data quality issues, applying appropriate cleaning techniques, handling outliers, performing EDA, and translating data into actionable business insights.
