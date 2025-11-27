# Crypto Trader Behavior & Market Sentiment Analysis

##  assignment Overview

This assignment analyzes the relationship between Bitcoin market sentiment (Fear & Greed Index) and trader performance on Hyperliquid, a decentralized perpetual futures exchange. The analysis explores how market psychology influences trading outcomes and identifies actionable patterns for smarter trading strategies.

**Assignment for:** Junior Data Scientist - Trader Behavior Insights Position

---

##  Objectives

- Analyze trader performance across different market sentiment conditions
- Identify correlations between Fear & Greed Index and profitability
- Uncover hidden patterns in position sizing and win rates
- Provide data-driven insights for trading strategy optimization

---

##  Dataset Description

### 1. Bitcoin Fear & Greed Index (2018-2025)
- **Size:** 2,644 daily records
- **Features:** Date, Sentiment Score (0-100), Classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)
- **Source:** Historical Bitcoin market sentiment data

### 2. Hyperliquid Trader Data
- **Size:** 211,224+ trades
- **Features:** Account, Coin, Execution Price, Size (USD), Side, Timestamp, Closed PnL, Direction, Fee, Leverage
- **Period:** Multi-year trading history across various cryptocurrencies

---

## 🔧 Methodology

### Data Processing
1. **Data Cleaning:** Removed incomplete records, handled malformed CSV rows
2. **Timestamp Conversion:** Unified date formats for merging (milliseconds to datetime)
3. **Feature Engineering:** Created Win/Loss/Breakeven flags, calculated metrics per sentiment
4. **Data Merging:** Joined trader data with daily sentiment classifications

### Analysis Techniques
- Exploratory Data Analysis (EDA)
- Groupby aggregations for sentiment-based performance
- Statistical analysis of win rates, PnL distributions, and position sizing
- Time series analysis of cumulative PnL trends
- Correlation analysis between sentiment scores and trading outcomes

---

##  Key Findings

### 1. Sentiment Impact on Performance
- **Best Performing Sentiment:** Greed periods show higher average PnL
- **Highest Win Rate:** Specific sentiment categories demonstrate superior performance
- **Risk Patterns:** Extreme Fear correlates with smaller position sizes and defensive trading

### 2. Position Sizing Behavior
- Traders take larger positions during Greed phases
- Risk aversion increases significantly during Extreme Fear
- Position sizing directly correlates with sentiment confidence

### 3. Coin-Specific Patterns
- Top 10 coins analyzed across all sentiment categories
- Certain assets perform better during specific market conditions
- Volatility-dependent trading patterns identified

### 4. Temporal Trends
- Cumulative PnL shows divergence across sentiment categories
- Trading volume spikes during extreme sentiment periods
- Long-term profitability varies significantly by sentiment exposure

---

##  Visualizations

1. **Performance Overview:** 4-panel comparison of PnL, win rates, trade volume, and position sizing
2. **PnL Distribution:** Box plots showing profitability spread across sentiments
3. **Time Series Analysis:** Cumulative PnL trends and daily trading volume
4. **Heatmap:** Top 10 coins performance matrix by sentiment
5. **Correlation Analysis:** Sentiment score vs trading outcomes

---

##  Tech Stack

- **Python 3.12+**
- **Libraries:** pandas, numpy, matplotlib, seaborn
- **Environment:** Google Colab
- **Data Processing:** Error-tolerant CSV parsing, datetime handling

---

## 📂 Repository Structure

