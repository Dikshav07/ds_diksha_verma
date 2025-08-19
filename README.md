# Data Science Report: Bitcoin Market Sentiment & Trader Performance Analysis

## 📌 Introduction
This project analyzes the relationship between **Bitcoin Market Sentiment (Fear & Greed Index)** and **Trader Performance** using historical trading data.  
The objective is to merge sentiment data with trader records, perform exploratory analysis, and uncover insights into how market psychology influences trading outcomes.

---

## 📊 Data Sources
### 1. Fear & Greed Index Dataset
- **Columns**: `timestamp`, `value`, `classification`, `date`  
- Provides a daily classification of market mood as **Fear** or **Greed**.

### 2. Historical Trader Data (Hyperliquid)
- **Columns include**: `account`, `coin`, `execution price`, `size tokens`, `size USD`, `side`, `timestamp IST`, `start position`, `closed PnL`, `direction`, etc.  
- Records trader-level performance and detailed trade activity.

**Dataset Links**  
- [Historical Trader Data](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)  
- [Fear & Greed Index](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)  

---

## ⚙️ Data Preprocessing (Notebook 1)
- Cleaned column names for consistency.  
- Converted timestamp columns into proper datetime objects.  
- Mapped sentiment classification to each trader record using date alignment.  
- Merged the two datasets into a single file: **`merged_data.csv`**.  

**Output**:  
- `csv_files/merged_data.csv`
- [merged data](https://drive.google.com/file/d/1BTSvI_0y1IQk84w_1lcTISbmE-Xz7yCb/view?usp=sharing)
---

## 🔍 Exploratory Data Analysis (Notebook 2)
- Analyzed daily **PnL trends** by sentiment (Fear vs. Greed).  
- Computed summary metrics:
  - Average PnL  
  - Total trades  
  - Win/Loss ratio  
- Visualized:
  - Distribution of trades across Fear vs. Greed days  
  - Trader performance trends under different sentiment regimes  

**Outputs**:  
- `csv_files/daily_pnl_by_sentiment.csv`  
- `csv_files/sentiment_summary_metrics.csv`  
- Charts and visualizations in the `outputs/` folder  

---

## 📈 Key Insights
- Traders showed **higher average PnL during Greed days** compared to Fear days.  
- **More trades** occurred during Greed sentiment, suggesting increased market participation.  
- Losses were generally **more severe on Fear days**, likely due to volatility and uncertainty.  

---

## 📂 Deliverables
- **Notebook 1** → Data preprocessing & merging (`merged_data.csv`)  
- **Notebook 2** → Exploratory analysis & insights (`daily_pnl_by_sentiment.csv`, `sentiment_summary_metrics.csv`, visualizations)  
- **Report** → [`ds_report.pdf`](./ds_report.pdf)  
- **README** → This file  

---

## 📝 Conclusion
This project successfully combines sentiment and trader datasets to analyze the relationship between **market psychology (Fear/Greed)** and **trading performance**.  
Findings indicate a positive correlation between **Greed sentiment and profitable trades**, while **Fear periods** are associated with higher volatility and losses.  

### 🚀 Future Work
- Extend analysis to **multiple timeframes** (hourly, weekly).  
- Apply **machine learning models** to predict PnL based on sentiment and trade features.  
- Evaluate **risk-adjusted performance metrics** (e.g., Sharpe ratio).  

---

## 🧑‍💻 Author
**Diksha Verma**  

---



📌 *This repo demonstrates the end-to-end workflow: from data preprocessing, merging, analysis, visualization, to insights.*  

