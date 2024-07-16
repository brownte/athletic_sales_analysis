# Module 5 Challenge - Athletic Sales Analysis

This repository contains a Jupyter Notebook that analyzes athletic sales data for 2020 and 2021. The analysis involves combining data from multiple sources, cleaning the data, and answering key business questions related to sales performance across different regions, retailers, and product categories.

## Analysis Overview

### Combine and Clean the Data
- Combine the 2020 and 2021 sales DataFrames.
- Convert the "invoice_date" column to a datetime data type.

### Determine which Region Sold the Most Products
- Use `groupby` to create a multi-index DataFrame with "region", "state", and "city".
- Rename the aggregated column to reflect the aggregation.
- Sort the results to show the top five regions, states, and cities that sold the most products.

### Determine which Region had the Most Sales
- Use `pivot_table` to create a multi-index DataFrame with "region", "state", and "city".
- Rename the aggregated column to reflect the aggregation.
- Sort the results to show the top five regions, states, and cities that generated the most sales.

### Determine which Retailer had the Most Sales
- Use `pivot_table` to create a multi-index DataFrame with "retailer", "region", "state", and "city".
- Rename the aggregated column to reflect the aggregation.
- Sort the results to show the top five retailers, regions, states, and cities that generated the most sales.

### Determine which Retailer Sold the Most Women's Athletic Footwear
- Filter the DataFrame to show only women's athletic footwear sales data.
- Use `groupby` to create a multi-index DataFrame with "retailer", "region", "state", and "city".
- Rename the aggregated column to reflect the aggregation.
- Sort the results to show the top five retailers, regions, states, and cities that had the most women's athletic footwear sales.

### Determine the Day with the Most Women's Athletic Footwear Sales
- Create a `pivot_table` with "invoice_date" as the index and "total_sales" as the values.
- Rename the aggregated column to reflect the aggregation.
- Resample the data into daily bins and calculate total sales for each day.
- Sort the results to show the days with the most women's athletic footwear sales.

### Determine the Week with the Most Women's Athletic Footwear Sales
- Resample the data into weekly bins and calculate total sales for each week.
- Sort the results to show the weeks with the most women's athletic footwear sales.

## Files

- `athletic_sales_analysis.ipynb`: Jupyter Notebook containing the complete analysis.