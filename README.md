# sql-global-layoffs-analysis
SQL project covering end-to-end data cleaning and exploratory data analysis (EDA) on a global layoffs dataset using window functions, CTEs, and analytical SQL techniques.

## Project Overview
This project performs an end-to-end analysis of a real-world global layoffs dataset using SQL (MySQL), covering both data cleaning & preparation and exploratory data analysis (EDA).
The objective was to improve data quality, create an analysis-ready dataset, and derive meaningful insights into layoff trends across industries, regions, company stages, and time periods.
A structured staging-table approach was used to preserve raw data while safely applying transformations, closely reflecting real-world data analyst workflows.

## Dataset
- Source: Kaggle – World Layoffs Dataset (2022)
- Link: https://www.kaggle.com/datasets/swaptr/layoffs-2022
- Format: CSV
- Description: Company-level layoff data including industry, location, date, funding, and company stage information

## Data Cleaning & Preparation

The first phase of the project focused on improving data quality and consistency:

- Created staging tables to retain raw data and apply transformations safely
- Identified and removed duplicate records using `ROW_NUMBER()` window functions
- Standardized company names, industry values, and country names
- Replaced blank values with NULL for accurate analysis
- Populated missing industry data using self-joins based on company names
- Converted date fields from text to proper `DATE` data types
- Removed records with insufficient or unusable layoff information
- Dropped helper columns to finalize clean, analysis-ready tables

## Exploratory Data Analysis (EDA)

Once the dataset was cleaned, exploratory analysis was performed to uncover trends and patterns:

- Analyzed layoffs by industry, geography, company stage, and year
- Identified industries and regions most impacted by layoffs
- Examined time-based trends to highlight peak layoff periods
- Aggregated total layoffs and company counts to support business-level insights

## SQL Concepts Used

- Window Functions (ROW_NUMBER)
- Common Table Expressions (CTEs)
- Joins
- Data Type Conversion
- NULL Handling
- Data Standardization
- Staging Tables & Data Integrity

## Outcome

The project delivers a clean, structured dataset along with data-driven insights into global layoff patterns.
It demonstrates practical SQL skills across the full data analysis lifecycle — from raw data preparation to insight generation — commonly expected in Data Analyst and Business Analyst roles.

## How to Use

1. Import the raw layoffs dataset into your SQL environment
2. Execute the data cleaning scripts to prepare the dataset
3. Run the analysis queries to explore trends and insights
4. Use the cleaned data for reporting, dashboards, or further analysis
