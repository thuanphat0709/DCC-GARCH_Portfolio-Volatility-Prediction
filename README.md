# Volatility Forecasting for Equity Portfolio: From GARCH(1,1) to DCC-GARCH

This project aims to analyze and predict the volatility of a diversified stock portfolio using historical price data from different industries in the S&P 500. 
It involves time series analysis, portfolio construction, and model-based volatility forecasting.

## 1. Supervisor
Le Trung Thanh, PhD - Foreign Trade University, HCMC Campus

## 2. Timeline
Project start to end: January 2025

## 3. Scope of work

Construct an equally-weighted portfolio using stocks from three distinct sectors:
- American Express (AXP) – Financial Services
- PepsiCo (PEP) – Consumer Staples
- Marriott International (MAR) – Hospitality

Perform in-sample (IS) and out-of-sample (OS) analyses:

- IS: 2014-01-01 to 2021-01-01
- OS: 2021-01-01 to 2024-01-01

Predict and evaluate portfolio volatility using statistical and econometric models.

## 4. Methodology

### 4.1. Data Collection:

- Stock price data retrieved from Yahoo Finance or equivalent APIs.

### 4.2. Portfolio Construction:

- Equal weighting applied to AXP, PEP, and MAR.
- Returns, standard deviation, Sharpe Ratio, and correlation matrix calculated.

### 4.3. Statistical Analysis:

- Asset-wise return distributions analyzed.
- Portfolio return and volatility calculated using time series data.

### 4.4. Volatility Modeling:

- Volatility is estimated and predicted using models such as:
  + GARCH(1,1)
  + EWMA (Exponentially Weighted Moving Average)
  + DCC-GARCH
- Models compared using performance on out-of-sample data.

## 5. Key Results & Insights

### 5.1. Individual Asset Statistics (IS Period)
- MAR delivers the highest return but is the most volatile.
- PEP is the most stable, confirming its consumer-staples profile.
- AXP underperforms with low risk-adjusted return.

### 5.2. Correlation Matrix (IS Period)
- The relatively low correlation between PEP and MAR adds diversification.
- AXP-MAR correlation is moderate-high → limits diversification.

### 5.3. DCC-GARCH Insights

- DCC-GARCH is a two-step model:
  + Univariate GARCH(1,1) to estimate volatilities of individual assets.
  + Dynamic Conditional Correlation (DCC) to estimate time-varying correlations.
- This model outperforms static correlation methods in high-volatility periods (e.g., COVID-19 crash).
- Allows tracking shifting relationships between assets over time → critical for risk management.

## 6. Disclaimer
This project is intended for educational purposes only.
