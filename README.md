# Home Sales Analysis

# Overview
This project uses PySpark and SparkSQL to analyze home sales data and derive key insights such as average prices, trends over time, and optimized queries for better performance. By leveraging distributed data processing, the analysis efficiently handles large datasets, demonstrating the power of PySpark for big data tasks.

# Purpose

The main goals of this project include:

- Exploring and analyzing home sales data to answer specific business questions.

- Implementing SparkSQL to query and aggregate data efficiently.

- Optimizing performance using caching, partitioning, and runtime comparison techniques.

- Demonstrating the practicality of PySpark for real-world applications.

# Technologies Used

- PySpark: Used for data processing and SparkSQL queries.

- SparkSQL: Enables querying and creating temporary views for analytical insights.

- AWS S3: Source for the dataset (home_sales_revised.csv).

- JupyterLab/Google Colab: Environment for running the notebook.

- Parquet: Format used for partitioned and optimized storage.

# Analysis Tasks

1. Data Preprocessing:

- Imported and explored the dataset.

- Created a temporary SQL table (home_sales) for analysis.

2. Key Questions Answered:

- What is the average price for a four-bedroom house sold for each year?

- What is the average price of homes (3 bedrooms, 3 bathrooms) per year built?

- What is the average price of homes (3 bedrooms, 3 bathrooms, 2 floors, ≥ 2,000 sqft) per year built?

- What is the average home price per "view" rating for homes priced ≥ $350,000?

3. Optimizations:

- Cached the temporary table to improve query runtime.

- Verified the caching mechanism.

- Partitioned the data by date_built and analyzed runtime benefits.

# How to Use

1. Clone this repository.

2. Open the notebook (Home_Sales.ipynb) in your chosen environment (e.g., JupyterLab, Google Colab).

3. Ensure PySpark and dependencies are installed.

4. Run the notebook step-by-step to explore the data, query results, and optimizations.

# Results

Insights:

  - Highlighted trends in pricing based on house attributes like bedrooms, bathrooms, floors, and square footage.

  - Showed the performance impact of caching and partitioning on SparkSQL queries.

Performance Comparison:

  - Measured and compared runtimes for uncached, cached, and partitioned queries.

# Future Enhancements

- Introduce machine learning models for predicting home prices.

- Conduct geospatial analysis by integrating location-based data.

- Explore more advanced optimizations like broadcasting joins or using cluster computing.

# Acknowledgments

This project was created as part of a big data analysis challenge. Special thanks to the curriculum team for providing the dataset and guidance.

# License
Include a license here if applicable (e.g., MIT License).
