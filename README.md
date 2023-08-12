# Home Sales Analysis with PySpark
This repository contains a Jupyter Notebook (Home_Sales.ipynb) that demonstrates the analysis of home sales data using PySpark SQL functions. In this project, we perform various queries on the provided home_sales_revised.csv dataset and answer specific questions regarding home prices and attributes.

Instructions
File Renaming: Start by renaming the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.

PySpark Setup: Ensure that the necessary PySpark SQL functions are imported. This is crucial for executing Spark SQL queries.

Data Loading: Read the home_sales_revised.csv data from the starter code into a Spark DataFrame. This dataset will be the foundation of our analysis.

Temporary Table: Create a temporary table named home_sales to facilitate SparkSQL operations on the dataset.

Query 1: Average Price for Four-Bedroom Houses: Use SparkSQL to calculate the average price for a four-bedroom house sold each year. Round off your answer to two decimal places.

Query 2: Average Price for Specific Home Attributes: Calculate the average price of homes based on their attributes, such as the year they were built, having three bedrooms and three bathrooms. Round off your answer to two decimal places.

Query 3: Average Price for Homes with Specific Attributes: Determine the average price of homes with specific attributes, such as three bedrooms, three bathrooms, two floors, and a minimum size of 2,000 square feet. Round off your answer to two decimal places.

Query 4: View Rating for Expensive Homes: Find the "view" rating for homes costing more than or equal to $350,000. Measure the query runtime and round off your answer to two decimal places.

Caching Data: Cache the home_sales temporary table to improve query performance.

Caching Verification: Check if the home_sales temporary table is successfully cached.

Query 5: Cached Data Analysis: Utilize the cached data to execute the query filtering out view ratings with an average price greater than or equal to $350,000. Compare the runtime with the uncached runtime.

Data Partitioning: Partition the formatted Parquet home sales data by the "date_built" field.

Parquet Data Temporary Table: Create a temporary table for the Parquet data to facilitate further analysis.

Query 6: Parquet Data Analysis: Run a query on the Parquet data, filtering out view ratings with an average price greater than or equal to $350,000. Compare the runtime with the uncached runtime.

Uncaching Data: Uncache the home_sales temporary table.

Uncaching Verification: Verify that the home_sales temporary table is no longer cached using PySpark.

Repository Upload: Download the completed Home_Sales.ipynb file and upload it to your "Home_Sales" GitHub repository for submission.
