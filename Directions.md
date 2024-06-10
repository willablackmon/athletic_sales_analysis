## Athletic Sales Analysis

#### 1. Combine and Clean the Data

1. Import the two CSV files, `athletic_sales_2020.csv` and `athletic_sales_2021.csv`, and read them into DataFrames.
2. Check that the columns in the two DataFrames have similar names and data types.
3. Combine the two DataFrames by the rows using an inner join, and reset the index.

Read over the instructions to determine if you should use `concat`, `join`, or `merge`.

4. After combining the DataFrames, do the following:

* Check if there are any null values.
* Check each column’s data type.
* Convert the "invoice_date" column to a datetime data type.
* Confirm that the data type has been changed.

#### 2. Determine which Region Sold the Most Products

1. Use either the `groupby` or `pivot_table` function to create a multi-index DataFrame with the "region", "state", and "city" columns.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Sort the results in descending order to show the top five regions, including the state and city that have the greatest number of products sold. Your final table should look like the following image:

![1717982388733](image/README/1717982388733.png)

#### 3. Determine which Region had the Most Sales

1. Use either the `groupby` or `pivot_table` function to create a multi-index DataFrame with the "region", "state", and "city" columns.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Sort the results in descending order to show the top five regions, including the state and city that generated the most sales. Your final table should look like the following image:

![1717982430401](image/README/1717982430401.png)

#### 4. Determine which Retailer had the Most Sales

1. Use either the `groupby` or `pivot_table` function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Sort the results in descending order to show the top five retailers along with their region, state, and city that generated the most sales. Your final table should look like the following image:

![1717982460379](image/README/1717982460379.png)

#### 5. Determine which Retailer Sold the Most Women's Athletic Footwear

1. Filter the combined DataFrame to create a DataFrame with only women's athletic footwear sales data.

Use `df[df["column_name"].str.contains("<value>")]` or `df.loc[(df["column_name"] =="<value>")]`.

2. Use either the `groupby` or `pivot_table` function to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns.
3. Rename the aggregated column to reflect the aggregation of the data in the column.
4. Sort the results in descending order to show the top five retailers along with their region, state, and city that sold the most women's athletic footwear. Your final table should look like the following image:

![1717982575096](image/README/1717982575096.png)

#### 6. Determine the Day with the Most Women's Athletic Footwear Sales

1. Create a pivot table with the "invoice_date" column as the index and the "total_sales" column as the `values` parameter.
2. Rename the aggregated column to reflect the aggregation of the data in the column.
3. Apply the `resample` function to the pivot table, place the data into daily bins, and get the total sales for each day.
4. Sort the resampled DataFrame in descending order to show the top 10 days that generated the most women's athletic footwear sales. Your final table should look like the following image:

![1717982617762](image/README/1717982617762.png)

#### 7. Determine the Week with the Most Women's Athletic Footwear Sales

1. Apply `resample` to the pivot table above, place the data into weekly bins, and get the total sales for each week.
2. Sort the resampled DataFrame in descending order to show the top 10 weeks that generated the most women's athletic footwear sales. Your final table should look like the following image:

![1717982652120](image/README/1717982652120.png)

---

#### Combine and Clean the Data (15 points)

* The two DataFrames have been combined on the rows using an inner join and the index has been reset. (10 points)
* The "invoice_date" column has been converted to a datetime data type. (5 points)

#### Determine which Region Sold the Most Products (15 points)

* A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "region", "state", and "city" columns. (10 points)
* The aggregated column has been renamed to reflect the aggregation of the data in the column. (1 point)
* The results are sorted in descending order to show the top five regions, including the state and city that sold the most products. (4 points)

#### Determine which Region had the Most Sales (15 points)

* A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "region", "state", and "city" columns. (10 points)
* The aggregated column has been renamed to reflect the aggregation of the data in the column. (1 point)
* The results are sorted in descending order to show the top five regions, including the state and city that generated the most sales. (4 points)

#### Determine which Retailer had the Most Sales (15 points)

* A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns. (10 points)
* The aggregated column has been renamed to reflect the aggregation of the data in the column. (1 point)
* The results are sorted in descending order to show the top five retailers along with their region, state, and city that generated the most sales. (4 points)

#### Determine which Retailer Sold the Most Women's Athletic Footwear (20 points)

* A filtered DataFrame is created that shows only women's athletic footwear sales data. (8 points)
* A `groupby` or `pivot_table` function has been used to create a multi-index DataFrame with the "retailer", "region", "state", and "city" columns. (7 points)
* The aggregated column has been renamed to reflect the aggregation of the data in the column. (1 point)
* The results are sorted in descending order to show the top five retailers along with their region, state, and city that had the most women's athletic footwear sales. (4 points)

#### Determine the Day with the Most Women's Athletic Footwear Sales (15 points)

* A pivot table is created that has the "invoice_date" column as the index and the "total_sales" column assigned to the `values` parameter. (10 points)
* The aggregated column has been renamed to reflect the aggregation of the data in the column. (1 point)
* The `resample` function is used on the pivot table, the data is placed into daily bins, and the total sales for each day is calculated. (2 points)
* The results are sorted in descending order to show the days that generated the most women's athletic footwear sales. (2 points)

#### Determine the Week with the Most Women's Athletic Footwear Sales (5 points)

* The `resample` function is used on the pivot table, the data is placed into weekly bins, and the total sales for each week is calculated. (3 points)
* The results are sorted in descending order to show the weeks that generated the most women's athletic footwear sales. (2 points)

new repository project: **athletic_sales_analysis**
