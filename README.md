# 📊 Portfolio Optimization using Python

This project implements a portfolio optimization model using Python. It calculates the optimal asset allocation that maximizes the **Sharpe Ratio**, balancing return and risk based on Modern Portfolio Theory (MPT).

---

## 🚀 Project Summary

- 📅 Data Source: Yahoo Finance (`yfinance`)
- 🧮 Technique: Modern Portfolio Theory (Mean-Variance Optimization)
- 🎯 Goal: Maximize Sharpe Ratio under diversification constraints
- 📉 Risk-Free Rate Assumed: 6% (India RBI Bonds)

---

## 🔧 Tools & Libraries Used

- `Python`
- `pandas`, `numpy` for data handling and math
- `matplotlib` for visualization
- `scipy.optimize` for portfolio optimization
- `yfinance` for fetching live stock data

---

## 📁 Workflow

1. **Fetch Historical Stock Prices**  
   Using `yfinance` for selected Indian stocks like TCS, Infosys, Reliance, etc.

2. **Calculate Daily Returns & Covariance Matrix**

3. **Define Portfolio Performance Metrics**  
   - Annual Expected Return  
   - Annual Volatility (Standard Deviation)  
   - Sharpe Ratio  

4. **Optimize Asset Weights**  
   - Objective: Maximize Sharpe Ratio  
   - Constraints:
     - Weights sum to 1 (100% invested)
     - Individual weights between 5% and 40% (diversification enforced)

5. **Output**  
   - Optimal weights for each stock
   - Expected return, risk, and Sharpe Ratio
   - Visualization via pie chart

---

## 📈 Sample Output

```text
TCS.NS: 27.89%
INFY.NS: 5.00%
RELIANCE.NS: 40.00%
HDFCBANK.NS: 22.11%
ITC.NS: 5.00%

Expected Annual Return: 17.50%
Annual Volatility (Risk): 13.20%
Sharpe Ratio: 0.86
