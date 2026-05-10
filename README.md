# Portfolio Optimization & CAPM Analysis

A quantitative finance project analyzing 10 equities using Python, CAPM regression, and Fama-French market factors.

## Overview
This project builds and evaluates an equally weighted portfolio of 10 stocks over a 10-year period (2015–2025). It pulls real market data, computes returns, runs CAPM regressions, and exports everything to Excel for verification.

## Stocks Analyzed
`AWK` `CVE` `DG` `ES` `EXPE` `HUBB` `KHC` `NTRS` `STZ` `WTW`

## What the Code Does
- Downloads monthly adjusted closing prices from **Yahoo Finance**
- Loads risk-free rate and market risk premium from **WRDS Fama-French factors**
- Computes monthly returns for each stock and an equally weighted portfolio
- Calculates excess returns (Equity Risk Premiums) for each stock and the portfolio
- Runs **CAPM regressions** using `statsmodels.OLS` to estimate alpha, beta, and R²
- Generates scatter plots with regression lines for each stock and the portfolio
- Exports all results to a structured Excel workbook

## Libraries Used
- `pandas` — data manipulation
- `yfinance` — stock price data
- `statsmodels` — OLS regression
- `matplotlib` — scatter plots
- `openpyxl` — Excel export

## How to Run
1. Place `fama_french_factors.xlsx` in the same folder as the notebook
2. Install dependencies: `pip install yfinance statsmodels openpyxl`
3. Run all cells top to bottom in Jupyter Notebook
