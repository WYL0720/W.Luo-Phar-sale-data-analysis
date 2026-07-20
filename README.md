# W.Luo-Phar-sale-data-analysis
### Project title:
Pharmaceutical Sales Trend Analysis (2014–2019)
### Objectives:
- Identify drug categories with strong seasonal patterns (e.g., winter peaks for respiratory and allergy medications).
- Evaluate long‑term growth or decline across therapeutic classes.
- Examine weekday vs weekend sales behavior.
- Compare volatility across categories to understand stability vs event‑driven demand.
- Build visualizations and a dashboard to support business

### Dataset Overview

The dataset originates from ~600,000 pharmacy transactions recorded between **2014 and 2019**.  
Raw data was pre‑processed (outlier handling, missing value imputation) and resampled into four granularities:

- **Hourly**
- **Daily**
- **Weekly**
- **Monthly**

Drug brands were grouped into the following ATC categories:

- **M01AE** – Anti‑inflammatory and antirheumatic products (non‑steroidal)
- **N02BA** – Analgesics/antipyretics (salicylic acid derivatives)
- **N02BE/B** – Analgesics/antipyretics (pyrazolones & anilides)
- **N05B** – Psycholeptics (anxiolytics)
- **N05C** – Psycholeptics (hypnotics & sedatives)
- **R03** – Drugs for obstructive airway diseases
- **R06** – Antihistamines for systemic use

### Methods & Tools

#### **Data Processing**
- Python (Pandas)
- SQLite (SQL queries)
- Time‑series resampling (hourly/daily/weekly/monthly)

#### **Analysis Techniques**
- Trend analysis  
- Seasonal decomposition  
- Month‑over‑month growth  
- Volatility measurement  
- Weekday/weekend comparison  
- Multi‑category visualization (facet plots, heatmaps, rolling averages)

#### **Visualization**
- Matplotlib  
- Seaborn  

#### **Dashboard**
A Power BI dashboard is included for interactive exploration 

### Structure

```text
pharma-sales-analysis/
│
├── README.md
│
├── notebook/
│   └── pharma_sales_analysis.ipynb
│
├── data/
│   ├── pharma_sales.db
│   ├── salesmonthly.csv
│   ├── salesweekly.csv
│   ├── salesdaily.csv
│   └── saleshourly.csv
│
├── figures/
│   ├── monthly_trend_all.png
│   ├── monthly_trend_by_category.png
│   ├── monthly_trend_summary.png
│   ├── seasonality_heatmap.png
│   ├── volatility_by_category.png
│   ├── mom_growth_multiplr.png
│   ├── seasonal_pattern_by_category.png
│   ├── weekday_vs_weekend_sales.png
│   └── yearly_trends_by_category.png
│
├── report/
│   └── pharma_sales_analysis_report.md
│
└── dashboard/
    └── pharma_sales.pbix

