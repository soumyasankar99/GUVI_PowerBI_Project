


# Power BI Dashboard for WalMart Sales Performance and Financial Metrics

## Overview
This project involves creating a comprehensive Power BI dashboard to analyze Sales Performance, and Financial Metrics of WalMart Data sample. The dashboard provides interactive visualizations and key insights to help drive data-driven business decisions.

## Features
### Sales Performance
1) Total Sales by Month: Track sales trends over time with a line chart.
2) Sales by Product Category: Visualize sales distribution across different product categories using a bar chart.
3) Top Selling Products: Identify the top-selling products with a sortable table.


### Financial Metrics

1) Revenue and Profit: Display total revenue and profit using KPI cards.
2) Profit Margins: Analyze profit margins with a gauge chart.

## Data Source
The data for this dashboard is sourced from a CSV file containing sales transaction records. Key columns include Order Date, Sales, Profit, Customer ID, Product Category, and more.

## Getting Started

### Prerequisites
* Power BI Desktop

## Steps to Recreate the Dashboard
### Clean The data By Running Python Script
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from warnings import filterwarnings
filterwarnings('ignore')

url = 'https://github.com/LokeshKumarChauhan/DE_with_powerBI/blob/main/Walmart.csv?raw=true'

df = pd.read_csv(url)

- Preprocessed and Transform The data While Handeling all the data Impurities and Handeling the Missing Data , Handeling Data Duplication, Null Value detection, Data Type Corection .
- After Commiting the Data Cleaning Part ,Exported the final Clean Data into a CSV file for further PowerBI DataVisualization Work.

### Import Data:

Open Power BI Desktop.
Click on "Get Data" and select "Text/CSV".
Browse to the CSV file and load the data.

### Data Preparation:

Ensure the "Order Date" column is in Date format.
Create a new column for Year-Month using the formula:

### DAX
YearMonth = FORMAT('TableName'[Order Date], "YYYY-MM")

## Create Visualizations:

### Sales Performance:

1) Total Sales by Month
2) Sales by Product Category
3) Top Selling Products


### Financial Metrics:

1)Revenue and Profit
2)Profit Margins

## Enhance Dashboard:

Add slicers for dynamic filtering.
Enable drill-through for detailed data exploration.
Adjust visual interactions for better user experience.
Publish Dashboard:

Save your Power BI report.
Click on "Publish" and select your workspace in Power BI Service.
