# Financial Transaction Analytics Pipeline

## Overview
An end-to-end financial transaction analytics pipeline that generates 
synthetic payment data, runs automated analysis, and visualizes insights 
through an interactive Power BI dashboard.

## Tools Used
- Python — data generation, cleaning, segmentation, anomaly detection
- Pandas & NumPy — data manipulation and statistical analysis
- Power BI — interactive dashboard and visualizations

## Pipeline Steps
1. Data Generation — 1,000 synthetic transactions across 6 categories
2. Data Cleaning — removed nulls, fixed formats, extracted time features
3. Segmentation — grouped by category, merchant and month
4. Anomaly Detection — flagged 53 transactions using standard deviation
5. Export — 4 CSV files ready for Power BI consumption

## Key Insights
- Travel is the highest spend category at $39,940
- Tech has the highest average transaction value at $163
- 53 anomalies detected representing 5.3% of all transactions
- Spending peaks in May across all categories

## Production Considerations
In a production environment this pipeline would be orchestrated using 
Azure Data Factory or Apache Airflow, scheduling automatic runs and 
triggering Power BI refresh via API to deliver real-time dashboards.

## Project Structure
financial-transaction-analytics
The project contains three folders:
- data — contains all CSV files exported from the pipeline
- notebooks — contains the Python pipeline script
- dashboard — contains the Power BI dashboard file
