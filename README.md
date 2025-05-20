# Home Sales Data Analysis with SparkSQL
**Creator**: Angelina Murdock  
**Date**: May 2025

## Overview 
This project analyzes home sales data using **Apache SparkSQL**. We answer key business questions, optimize performance through caching and partitioning, and evaluate query run times. The data is stored in Parquet format and analyzed using SparkSQL queries.

## Table of contents
- [Overview](#overview)
- [Usage Guide](#usage-guide)
- [Methodology](#methodology)
- [Resources](#resources)

## Usage Guide
**Open the Project**:

Open `Home_sales_colab.ipynb` in **Google Colab:**

- Go to https://colab.research.google.com

- Click **File > Open Notebook**

- Select the **GitHub** tab and enter your repository URL:
    `https://github.com/Angelinamurdock/Home_Sales`

- Click to open `Home_sales_colab.ipynb`

### Methodology 
1. **Load Data**: Read home_sales_revised.csv from AWS S3 into a Spark DataFrame and create a temporary SQL view.

2. **Run Queries:** Use SparkSQL to calculate average home prices by various filters (bedrooms, bathrooms, floors, sqft, view rating).

3. **Optimize Performance:** Cache the temporary table and compare query runtimes before and after caching.

4. **Partition Data**: Save data partitioned by date_built in Parquet format, read it back, and rerun queries to compare performance.

5. **Manage Cache**: Uncache the table and verify its status.

## Resources
- **DU Bootcamp Module 22:** Used challenge files and class materials from the bootcamp.
- **ChatGPT:** Assisted with code explanations and debugging.