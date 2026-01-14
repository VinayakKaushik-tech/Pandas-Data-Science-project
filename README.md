# Pandas-Data-Science-project
## Sales Data Analysis with Pandas & Matplotlib

In this project, I conduct a comprehensive analysis of 12 months of electronics store sales data. With hundreds of thousands of transactions to sift through, I use Python Pandas for data wrangling and Matplotlib for visualization to uncover trends, optimize advertising schedules, and identify product relationships.

## Project Overview

The dataset contains information such as Order ID, Product, Quantity Ordered, Price Each, Order Date, and Purchase Address. The goal is to clean this data and answer five key business questions to drive strategic decision-making.

## Technical Workflow

1. Data Cleaning & Preparation
Before analysis, I performed several preprocessing steps to ensure data integrity:

Merging Data: Combined 12 individual CSV files into a single master DataFrame using pd.concat.

Handling Missing Values: Identified and dropped NaN rows that would interfere with calculations.

Filtering: Removed "dirty" data, such as rows where headers were repeated within the dataset.

Type Conversion: Used pd.to_numeric and pd.to_datetime to ensure columns were in the correct format for mathematical operations and time-series analysis.

2. Feature Engineering
I extracted specific details from the raw data to enable more granular analysis:

Added a Month column by parsing the "Order Date."

Added a City column using the .apply() method to extract the city name and state from the "Purchase Address."

Added Sales and Hour columns to facilitate revenue and timing analysis.
