# Project Description: Unsupervised Learning Trading Strategy Returns Over Time

This project aims to develop a trading strategy using unsupervised learning techniques to analyze and optimize returns of SP500 stocks. The steps involved in this project are as follows:

## Download/Load SP500 Stocks Prices Data:

1. Download historical price data for SP500 stocks using Yahoo Finance API.
2. Stack and clean the data for further processing.

## Calculate Features and Technical Indicators for Each Stock:

Calculate various features and technical indicators, including:
- Garman-Klass Volatility
- Relative Strength Index (RSI)
- Bollinger Bands
- Average True Range (ATR)
- Moving Average Convergence Divergence (MACD)
- Dollar Volume

## Aggregate Data to Monthly Level and Filter Top 150 Most Liquid Stocks:

1. Convert daily data to monthly-end frequency.
2. Calculate 5-year rolling averages of dollar volume to filter the top 150 most liquid stocks for each month.

## Calculate Monthly Returns for Different Time Horizons:

Compute historical returns over various monthly periods to capture time series dynamics such as momentum patterns.

## Download Fama-French Factors and Calculate Rolling Factor Betas:

Download Fama-French factors and estimate the exposure of assets to common risk factors using linear regression.

## Fit a K-Means Clustering Algorithm to Group Similar Assets:

For each month, fit a K-Means Clustering Algorithm to group assets based on calculated features.

## Select Assets and Form a Portfolio Based on Efficient Frontier Max Sharpe Ratio Optimization:

Select assets from clusters and form a portfolio optimized for maximum Sharpe ratio using Efficient Frontier techniques.

## Visualize Portfolio Returns and Compare to SP500 Returns:

Visualize the performance of the constructed portfolio and compare its returns to those of the SP500 index.
