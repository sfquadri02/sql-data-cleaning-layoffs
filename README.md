# sql-data-cleaning-layoffs
SQL project focused on cleaning and preparing a global layoffs dataset using window functions, CTEs, and data standardization techniques.

## Project Overview
This project focuses on cleaning and preparing a real-world global layoffs dataset using SQL.
The objective was to improve data quality and consistency by removing duplicate records, standardizing inconsistent values, handling nulls, and correcting data types to produce an analysis-ready dataset.

A structured staging-table approach was used to preserve raw data while safely applying transformations, mirroring real-world data preparation workflows.

## Dataset
- Source: Kaggle – World Layoffs Dataset (2022)
- Link: https://www.kaggle.com/datasets/swaptr/layoffs-2022
- Format: CSV
- Description: Company-level layoff data including industry, location, date, funding, and company stage information

## Data Cleaning Steps

- Created staging tables to retain original raw data and perform transformations safely
- Identified and removed duplicate records using ROW_NUMBER() window functions
- Standardized industry and country values to ensure consistency
- Replaced blank values with NULL for accurate analysis
- Populated missing industry data using self-joins on company names
- Converted date fields from text format to proper DATE data type
- Removed records with insufficient layoff information
- Dropped helper columns after cleaning to finalize the dataset

## SQL Concepts Used

- Window Functions (ROW_NUMBER)
- Common Table Expressions (CTEs)
- Joins
- Data Type Conversion
- NULL Handling
- Data Standardization
- Staging Tables & Data Integrity

## Outcome

The final cleaned dataset is consistent, reliable, and ready for exploratory data analysis or visualization.
This project demonstrates practical SQL data-cleaning techniques commonly used in real-world data analyst and business analyst roles.

## How to Use

1. Import the raw layoffs dataset into your SQL environment
2. Run the SQL script step-by-step to reproduce the cleaning process
3. Use the cleaned table for analysis, reporting, or visualization
