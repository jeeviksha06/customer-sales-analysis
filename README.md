# CUSTOMER SALES ANALYSIS

## Project Overview
An advanced data analysis project that merges sales and customer 
data to identify top customers, analyze purchasing patterns, and 
generate business insights using Pandas and Matplotlib.

## Objectives
- Merge multiple datasets (sales and customer data)
- Perform grouping and aggregation operations
- Handle datetime data for trend analysis
- Create pivot tables for data summarization
- Build visualizations to communicate insights

## Setup & Installation
1. Install Python 3.x
2. Install required libraries:
pip install pandas matplotlib jupyter
3. Clone this repository
4. Open `customer_analysis.ipynb` in Jupyter/VS Code
5. Run all cells in order

## Project Structure
- `customer_analysis.ipynb` — main analysis notebook
- `data/` — contains sales_data.csv and customer_churn.csv
- `visualizations/` — contains generated charts
- `analysis_report.pdf` — final report with insights

## Technical Approach
1. Loaded and explored both datasets
2. Checked for missing values (none found)
3. Merged datasets using Customer_ID (handled format mismatch using regex)
4. Performed 3 types of aggregations:
   - Total sales by region
   - Average sale by contract type
   - Top 5 customers by spending
5. Created a pivot table (Region vs Contract Type)
6. Converted date column to datetime and extracted monthly trends
7. Built 4 visualizations (bar, line, pie, and churn analysis charts)

## Key Findings

### Revenue & Customers
- Total Revenue: ₹12,365,048
- Total Customers: 100
- Average Order Value: ₹123,650.48

### Top Performers
- Top Customer: CUST016 (₹373,932 total spend)
- Top Region: North (₹3,983,635 in sales)
- Best Month: March

### Business Insights
- Customers on One-Year contracts spend the most on average
- North and South regions together generate over 60% of total revenue
- Overall churn rate is 10%
- Sales peaked in March and dropped significantly in April

## Charts Generated
1. Bar Chart — Total sales by region
2. Line Chart — Monthly sales trend
3. Pie Chart — Sales distribution by contract type
4. Bar Chart — Churn rate by contract type

## Recommendations
1. Focus retention efforts on Month-to-month customers (higher churn risk)
2. Investigate April's sales drop for seasonal patterns
3. Replicate North region's successful strategies in West region
4. Encourage One-Year contracts through incentives (higher average spend)

## What I Learned
- How to merge datasets with mismatched ID formats using regex
- Multiple types of groupby aggregations
- Creating and interpreting pivot tables
- Working with datetime data in Pandas
- Building a complete data analysis pipeline in Jupyter Notebook