# 📊 Fundamental Financial Screening & Analytics for Indian Equities
![Cover Image](nifty.jpg)
This project provides a comprehensive financial analysis of Indian equities to identify high-quality and stable companies using fundamental metrics. It includes metric-wise exploration, cross-metric analysis, feature engineering, and multi-metric insights to highlight financially strong businesses.

## 📝 Table of Contents

- 📌 Introduction
- 🎯 Aim
- 📂 Dataset Overview
- ❓ Problem Statement
- 🛠️ Tools & Technologies
- 🔍 Analysis Workflow
- 📈 Univariate Analysis
- 🔗 Bivariate Analysis
- 🔎 Feature Engineering
- 📊 Multivariate Analysis
- 💡 Key Takeaways

## 📌 Introduction
This project focuses on a comprehensive financial analysis of Indian equities to identify high-quality and stable companies using fundamental metrics.

The analysis includes:
* Individual metric analysis
* Relationship exploration
* Feature engineering
* Multivariate screeningfundamental metrics.

## 🎯 Aim
To analyze the financial performance of Indian companies and identify high-quality, stable stocks using key financial metrics through data-driven evaluation.

## 📂 Dataset Overview
The dataset contains financial information for major Indian companies, including:

| Column            | Meaning                          |
| ----------------- | -------------------------------- |
| **CMP**           | Current Market Price (₹)         |
| **PE**            | Price-to-Earnings ratio          |
| **MarketCap**     | Market capitalization (₹ Crores) |
| **DividendYield** | Annual dividend yield (%)        |
| **NPQtr**         | Latest quarterly net profit      |
| **QtrProfitVar**  | Quarterly profit variation (%)   |
| **SalesQtr**      | Latest quarterly sales           |
| **QtrSalesVar**   | Quarterly sales variation (%)    |
| **ROCE**          | Return on Capital Employed       |
| **PATAnn**        | Annualized Profit After Tax      |
📌 Source: Kaggle – Top Indian Stocks Market Insights Dataset (Stock_data.csv)

## ❓ Problem Statement
Investors struggle to identify stable and fundamentally strong companies from a large universe of stocks.
This project simplifies the process by:

- Analyzing key financial indicators
- Studying valuation, profitability, growth, and stability
- Identifying high-quality companies with consistent performance

## 🛠️ Tools & Technologies

- Python
- Jupyter Notebook
- Libraries Used:
 
      import pandas as pd
      import matplotlib.pyplot as plt
      import seaborn as sns
      import numpy as np
      import plotly.express as px
      import plotly.io as pio
      pio.renderers.default = 'notebook'  
  
  ## 🔍 Analysis Workflow
  -  ✔ Data Cleaning Performed
    - [x]Column renaming
    - [x]Removing unnecessary fields
    - [x]Handling missing values
    - [x]Checking outliers but keeping true market variability
    - [x]Converting datatypes
    - [x]Removing duplicates

  ## 📈 Univariate Analysis
  
  - 1. PE Ratio Distribution
       - Understanding valuation levels
       - Identifying expensive/cheap stocks
       - Spotting extreme outliers
  - 2. ROCE Distribution
       - Measuring efficiency of capital use
       - Understanding what ROCE levels are “good”
       - Finding exceptional companies
  - 3. Dividend Payout & Dividend Yield
       - % of companies paying dividends
       - Distribution of yields
       - Identifying yield-based investment opportunities

  ## 🔗 Bivariate Analysis

  - 1. ROCE vs Quarterly Profit Variation
       - Are efficient companies more stable?
       - Do high-ROCE firms show lower volatility?
  - 2. PE Ratio vs Quarterly Sales Growth
       - Does market valuation reward sales growth?
       - Detecting undervalued & overvalued companies
  - 3. MarketCap vs Dividend Yield
       - Do large companies pay consistent dividends?
       - Identifying stable dividend payers

  ## 🔎 Feature Engineering

  - 1. QARP: Quality at Reasonable Price
       - High ROCE
       - Low PE

  - 2. Profit Stability Metric
       - Lower variation = lower risk

  - 3. Sales Stability
       - Understanding operational consistency

  - 4. Dividend Categories
       - High Dividend (>1.5%)
       - Moderate (0–1.5%)
       - No Dividend (0%)

  - 5. Composite Quality Score
       - Weighted sum of:
       - ROCE (60%)
       - 1/PE (40%)

  - 6. Risk Index
       - Combination of:
       - Profit volatility
       - Sales volatility
      
  ## 📊 Multivariate Analysis
  
  - 1. High-ROCE + Low-Risk + Dividend-Paying Companies
       
       Finding companies that combine:
       - Efficiency
       - Stability
       - Income generation
         
  - 2.MarketCap vs RiskIndex
       - Large caps → more stable
       - Small caps → higher volatility
       - Mid caps → mixed behavior
         
   ## 💡 Key Takeaways
  
  - Most stocks trade at 20–40 PE
  - ROCE typically lies between 10–24%
  - 72% of companies pay dividends
  - Large caps are the most stable, small caps the most volatile
  - High ROCE + low volatility = high-quality stocks




