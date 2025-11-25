# ***Trader Behavior Analysis***
**Project Overview**

This project is part of the Data Science hiring assignment for the Web3 Trading Team.
The objective is to analyze trader behaviour using Hyperliquid historical trading data and explore whether it aligns with market sentiment (Fear/Greed).

**Project Structure**

| **Folder / File**              | **Description**                                                              |
| ------------------------------ | ---------------------------------------------------------------------------- |
| **ds_Yashika/**                | Main project folder                                                          |
| ├── `notebook_1.ipynb`         | Google Colab notebook containing full analysis                               |
| **csv_files/**                 | Folder containing generated dataset outputs                                  |
| ├── `cleaned_trading_data.csv` | Cleaned full trading dataset (may exceed 25MB)                               |
| ├── `accounts_summary.csv`     | Per-account KPIs                                                             |
| ├── `coin_level_summary.csv`   | Per-symbol KPIs                                                              |
| **outputs/**                   | Folder containing generated plots                                            |
| ├── `trades_per_day.png`       | Daily trade frequency plot                                                   |
| ├── `volume_per_day.png`       | Daily trading volume plot                                                    |
| ├── `pnl_distribution.png`     | Distribution of closedPnL                                                    |
| ├── `other_EDA_charts/`        | All other visual outputs from EDA                                            |
| **ds_report.pdf**              | Final detailed report (Problem statement → Analysis → Findings → Conclusion) |
| **README.md**                  | Repository documentation                                                     |


**Assignment Overview**

This project analyzes trader behaviour, using:

Hyperliquid Historical Trader Data - https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing 

Bitcoin Fear & Greed Index - https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing

The official goal (from the instructions) was to explore:
- profitability patterns
- risk-taking behavior
- trade volume dynamics
- how traders behave in fear vs greed environments

However, due to a date mismatch (sentiment data 2018–2023 vs trades in 2024–2025), sentiment mapping was not possible.
Therefore, the analysis focuses on trader behavior only, as documenting and justifying this is acceptable.

**What This Prjoct does**

*1. Cleaning & Preparing the Dataset*

Standardized column names

Parsed timestamps (IST → datetime)

Created trade_date, trade_time, trade_hour

Generated profitable flag

Cleaned numeric fields

*2. Exploratory Data Analysis*

Includes:

Daily trade activity

Daily trading volume

PnL distribution

Buy vs Sell behaviour

Hour-of-day analysis

Coin-level summary

Per-account behaviour

Correlation between size & PnL

*3. Per-Account Behaviour Profiling*

For each account, we analyze:

Number of trades

Total volume

Average PnL

Win-rate

Trading pattern consistency

*4. Sentiment Decision*

Sentiment dataset (2018–2023) had no overlap with trading dates (2024–2025).

Therefore sentiment analysis was not used.

This is clearly mentioned in both the notebook and report.

**Google Colab Notebook Link**

https://colab.research.google.com/drive/13QAEktO0eP-d3fUpSMewV3bBtAqhhDSG?usp=sharing

**Summary of Findings**

A short summary you can include:

1.The dataset contains 211,224 trades across 32 accounts.

2.Trading activity increases significantly in 2024–2025.

3.A mix of high-frequency small trades and rare large trades exists.

4.PnL distribution is highly skewed with a few large positive outliers.

5.Win rate ≈ 41%, typical of speculative, frequent trading.

6.No time-of-day advantage — trades occur continuously.

7.Sentiment analysis was excluded due to non-overlapping timelines.

**How to Run**

- Open the Colab notebook

- Upload the CSV files

- Run all cells in sequence

- View generated CSVs and plots in the csv_files/ and outputs/ folders


