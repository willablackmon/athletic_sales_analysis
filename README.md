# Athletic Sales Analysis

This project analyzes sales data from 2020 and 2021 to provide insights into sales trends across regions and retailers, with a focus on women's athletic footwear. The analysis leverages data cleaning, aggregation, and time-series methods to uncover key performance metrics.

**[Abstract](#abstract)** | **[Data](#data)** | **[Results](#results)** | **[Core Skills, Technologies, Tools](#core-skills-technologies-tools)** | **[License](#license)**

---

## Abstract

This project consolidates sales data from 2020 and 2021 to analyze performance by region and retailer, focusing on women's athletic footwear. Key steps include:

* **Data Cleaning** : Combined and standardized sales data from multiple years, ensuring consistency across columns and types.
* **Region and Retailer Analysis** : Identified top-performing regions and retailers in terms of total sales and specific product categories.
* **Time-Series Analysis** : Used date-based analysis to determine the most successful days and weeks for sales, especially of women's athletic footwear.
* **Pandas Methodologies** : Leveraged `groupby`, `pivot_table`, and filtering techniques to extract detailed insights from the dataset.

## Data

The application uses two CSV files:

* **athletic_sales_2020.csv**
* **athletic_sales_2021.csv**

### Data Processing Steps:

* Import and read both CSV files into Pandas DataFrames.
* Check that the columns in both DataFrames have consistent names and types.
* Combine the DataFrames by rows using an inner join, and reset the index.
* Perform various calculations and aggregations to extract sales insights.

## Results

The analysis helps to answer key questions:

* Which region sold the most products overall?
* Which region had the highest total sales?
* Which retailer performed best in terms of total sales and sales of specific products (women's athletic footwear)?
* When were the peak sales periods for women's athletic footwear (by day and week)?

## Core Skills, Technologies, Tools

* **Tools and Libraries** : Python, Pandas, and Jupyter Notebook for data analysis and reporting.
* **Data Cleaning and Preparation** : Merged, cleaned, and verified data consistency across CSV files from different years.
* **Data Aggregation and Analysis** : Aggregated and analyzed data, using `groupby` and `pivot_table` to extract sales insights.
* **Time-Series and Date Manipulation** : Manipulated date columns to identify peak sales periods and analyze time-based trends.
* **Data Organization and Transformation** : Sorted, filtered, and renamed data for clarity, focusing on specific products and performance metrics.
* **Python Programming** : Basic loops, conditionals, and string manipulation.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
