# Home Sales Analysis with PySpark
This repository contains a Jupyter Notebook (Home_Sales.ipynb) that demonstrates the analysis of home sales data using PySpark SQL functions. In this project, we perform various queries on the provided home_sales_revised.csv dataset and answer specific questions regarding home prices and attributes.

# Instructions
* File Renaming: Start by renaming the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.
* PySpark Setup: Ensure that the necessary PySpark SQL functions are imported. This is crucial for executing Spark SQL queries.
* Data Loading: Read the home_sales_revised.csv data from the starter code into a Spark DataFrame. This dataset will be the foundation of our analysis.
* Temporary Table: Create a temporary table named home_sales to facilitate SparkSQL operations on the dataset.

# Analysis
Query 1: Average Price for Four-Bedroom Houses: Use SparkSQL to calculate the average price for a four-bedroom house sold each year. Round off your answer to two decimal places.

<img width="161" alt="Screenshot 2023-08-11 at 10 10 37 PM" src="https://github.com/breeliu2/Home_Sales/assets/124847109/be49f795-a105-4145-9370-ee65865a17b7">


Query 2: Average Price for Specific Home Attributes: Calculate the average price of homes based on their attributes, such as the year they were built, having three bedrooms and three bathrooms. Round off your answer to two decimal places.


<img width="156" alt="Screenshot 2023-08-11 at 10 10 54 PM" src="https://github.com/breeliu2/Home_Sales/assets/124847109/30b909be-b2ef-4767-a2ae-bddcaeb3fe75">

Query 3: Average Price for Homes with Specific Attributes: Determine the average price of homes with specific attributes, such as three bedrooms, three bathrooms, two floors, and a minimum size of 2,000 square feet. Round off your answer to two decimal places.

<img width="199" alt="Screenshot 2023-08-11 at 10 11 07 PM" src="https://github.com/breeliu2/Home_Sales/assets/124847109/56db66dc-ec08-406f-ba02-31077cd1d30d">


Query 4: View Rating for Expensive Homes: Find the "view" rating for homes costing more than or equal to $350,000. Measure the query runtime and round off your answer to two decimal places.
<img width="266" alt="Screenshot 2023-08-11 at 10 11 23 PM" src="https://github.com/breeliu2/Home_Sales/assets/124847109/6771c2d2-d338-4ae2-a1c1-00ee78cef953">



* Caching Data: Cache the home_sales temporary table to improve query performance.

* Caching Verification: Check if the home_sales temporary table is successfully cached.

Query 5: Cached Data Analysis: Utilize the cached data to execute the query filtering out view ratings with an average price greater than or equal to $350,000. Compare the runtime with the uncached runtime.

<img width="280" alt="Screenshot 2023-08-11 at 10 11 54 PM" src="https://github.com/breeliu2/Home_Sales/assets/124847109/d09c0a7d-25bc-4716-a5f9-e93316d9f3c6">


* Data Partitioning: Partition the formatted Parquet home sales data by the "date_built" field.

* Parquet Data Temporary Table: Create a temporary table for the Parquet data to facilitate further analysis.

Query 6: Parquet Data Analysis: Run a query on the Parquet data, filtering out view ratings with an average price greater than or equal to $350,000. Compare the runtime with the uncached runtime.

<img width="290" alt="Screenshot 2023-08-11 at 10 12 20 PM" src="https://github.com/breeliu2/Home_Sales/assets/124847109/2efb0a8c-2c60-4d8b-a8c6-c440627fcc0b">



Uncaching Data: Uncache the home_sales temporary table.

Uncaching Verification: Verify that the home_sales temporary table is no longer cached using PySpark.

