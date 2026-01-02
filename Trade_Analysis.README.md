# 📈 Trading Opportunities in Cryptocurrency Markets: An Hourly Analysis of Bitcoin and Ethereum

## 🎯 Project Overview
A comprehensive quantitative analysis of hourly price movements in Bitcoin and Ethereum markets to identify statistically significant trading opportunities. This project employs advanced time series econometrics, rolling window analysis, and hypothesis testing to uncover intraday patterns in cryptocurrency returns.

## 📊 Research Objectives
1. **Hourly Trend Analysis:** Identify statistically significant patterns in cryptocurrency returns by hour-of-week
2. **Rolling Window Analysis:** Examine long-term trends using 1-year rolling windows (8,760 hours)
3. **Statistical Validation:** Apply hypothesis testing to distinguish meaningful patterns from random noise
4. **Trading Strategy Insights:** Provide data-driven recommendations for intraday cryptocurrency trading

## 🔬 Methodology

### **1. Data Processing Pipeline**
- **Data Sources:** 
  - Ethereum: `ETH_1H.csv` (May 2016 - April 2020)
  - Bitcoin: `coinbaseUSD_1-min_data.csv` (December 2014 - May 2023)
- **Data Wrangling:**
  - Bitcoin minute data aggregated to hourly frequency
  - Log-returns calculation: `log(P_t/P_{t-1})`
  - Hour-of-week indexing for cyclical analysis

### **2. Statistical Framework**
```r
# Core Analytical Techniques
1. Descriptive Statistics & Time Series Visualization
2. Log-Return Computation & Volatility Analysis
3. Rolling Mean Analysis (8,760-hour windows)
4. One-Sample T-Tests: H₀: μ = 0 vs H₁: μ > 0
5. Binomial Tests: H₀: p = 0.5 vs H₁: p > 0.5
6. Multiple Hypothesis Testing with 5% and 10% significance levels
