# Volatility Regime Prediction – Supervised Learning Final Project
*Predicting VIX spikes using S&P 500 (GSPC) financial time series*

## Contributors
- Clémence Marco  
- Alzira Ferreira

# 1. Business Challenge

Volatility is one of the most important dimensions of financial risk.  
Sudden jumps in volatility, commonly measured through the VIX Index, impact:

- derivative pricing,
- portfolio hedging costs,
- margin requirements,
- risk management decisions,
- trading strategies.

**Business problem**  
We aim to predict **whether the VIX will spike tomorrow** (binary classification) using information derived from the S&P 500 (SPX/GSPC) and VIX historical data.  
A “spike” is defined as a VIX return in the **top 10% percentile**, i.e. extreme volatility events.

**Why it matters**
Being able to anticipate volatility explosions matters for:

- equity and derivatives traders (hedging timing),
- asset managers (risk exposure adjustment),
- market makers (inventory management),
- risk management teams (VaR breaches, stress tests).

This is a real-world business challenge routinely addressed in quantitative finance.


# 2. Dataset Description

We use daily historical (01-01-2000 to 01-09-2025) data for:

- **S&P 500 Index (GSPC)** from Yahoo Finance  
  - Features: Open, High, Low, Close, Volume  
- **VIX Index**, also from Yahoo Finance  
  - Feature: Close

**Period:** [Specify the start and end date used]

**Source:**  
Downloaded using `yfinance`. Data is real-world (not synthetic), publicly accessible, and updated daily.