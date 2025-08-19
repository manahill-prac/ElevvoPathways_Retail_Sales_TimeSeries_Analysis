# Time Series Breakdown of Retail Sales

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<your-username>/<your-repo-name>/blob/main/notebooks/Time_Series_Retail_Sales.ipynb)

This project performs a **time series analysis** on Walmart retail sales data. The goal is to analyze trends, seasonality, and patterns in sales across stores, departments, and regions, and to produce actionable insights with simple forecasting.



## Dataset

- **Train data:** Weekly sales for each store and department.  
- **Features data:** Weekly store features including temperature, fuel price, markdowns, CPI, unemployment, and holiday flags.  
- **Stores data:** Store metadata including type and size.  

**Source:** [Walmart Sales Forecasting Kaggle Dataset](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data)

>

## Steps Performed

1. **Data Loading & Cleaning**
   - Merge train, features, and store datasets
   - Handle missing values
   - Convert date column to datetime

2. **Exploratory Data Analysis (EDA)**
   - Overall sales trends
   - Holiday effect analysis
   - Top/bottom stores & departments
   - Store type comparison
   - Correlation heatmap

3. **Time Series Breakdown**
   - Monthly sales aggregation
   - Seasonal pattern analysis
   - Region / store size analysis

4. **Simple Forecasting**
   - Exponential Smoothing model for 12-month forecast

5. **Insights Summary**
   - Automatically computed key metrics:
     - Peak / lowest months for sales
     - Top / bottom stores
     - Store type impact
     - Holiday effect
     - Forecasted trend
   - Exported summary table (`insights_summary.csv`)

6. **Exported Data**
   - Monthly sales summary: `monthly_sales_summary.csv`
   - Region/store sales summary: `region_sales_summary.csv`
   - Insights summary: `insights_summary.csv`

---

## Libraries & Tools

- Python (3.x)
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Statsmodels (for Exponential Smoothing)
- gdown (for downloading datasets from Google Drive)

---

## How to Run

Clone the repository
```bash
git clone <your-repo-url>

Install dependencies

pip install -r requirements.txt


Open the notebook in Google Colab or locally.

All charts, insights summary, and CSV exports are generated automatically
