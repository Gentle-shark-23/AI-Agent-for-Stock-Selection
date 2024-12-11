# AI-Agent-for-Stock-Selection
The project aimed to develop a robust investment decision-making framework integrating Agentic AI. It covers the creation of agents that assess client risk profiles, generate tailored strategies, and perform backtesting using S&P 500 data. The system incorporates LLM models like GPT-4, leveraging libraries such as Langchain, to engage clients, assess risk, and optimize strategies. Key challenges include integrating agent components, improving strategy performance, and refining the backtesting workflow.


Strategy:
- Strategy.ipynb is the main code file, which is mainly based on Mean Variance Strategy. By running it, you can get the results which is already shown in the file named 'summary_results_with_risk_score.csv'.

- summary_results_with_risk_score.csv contains these columns:
	1) hist_lag
	2) rebalancing_frequency
	3) risk_tolerance
	4) Return
	5) Volatility
	6) Sharpe Ratio
	7) Portfolio Combination
	8) risk_score

Back-testing:
Backtesting_single_strategy shows the strategy and backtesting process. Backtesting_single_strategy.ipynb is a sample code showing the backtesting process for a simgle strategy of S&P 500 stock data. In the sample, we demonstrated the portfolio optimization, portfolio relabance and backtesting results with key metrics such as sharpe ratio/ max drawdown/ cumulated return of the portfolio and so on.

Data:
Overview
This repository contains code for cleaning, processing, and analyzing historical S&P 500 stock data (2013-2024). The goal is to build a robust dataset that accounts for changes in S&P 500 membership, IPO dates, and data quality issues, serving as a foundation for integrating Agentic-AI into portfolio management and optimization.

Data Cleaning:
Filters data within 2013-2024.
Handles missing values using forward-fill and interpolation.
Excludes stock prices outside valid S&P 500 membership or IPO periods.
S&P 500 Membership Adjustments:
Aligns stock data with membership periods and IPO dates.
Filters out non-member or pre-IPO data.
Outlier Detection and Smoothing
Identifies and smooths anomalies using Z-scores and MAD.
Statistical Analysis:
Computes mean, variance, and cumulative returns.
Provides sector-based and risk-adjusted metrics (e.g., Sharpe Ratios).
Visualization:
Generates insights with:
Stock price trends.
Mean/variance distributions.
Cumulative returns with IPO dates marked.
