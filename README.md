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
Backtesting_single_strategy shows the strategy and backtesting process.

Data:
This repository contains code and documentation for cleaning, processing, and analyzing historical S&P 500 stock data from 2013 to 2024. The primary focus is on creating a robust dataset that accounts for changes in S&P 500 membership, IPO dates, and handling of missing or noisy data. The processed dataset is foundational for integrating Agentic-AI into portfolio management systems and optimizing investment strategies.

Data Cleaning:
Filters data within the time range 2013-2024.
Handles missing values using forward-fill and interpolation techniques.
Removes invalid stock prices outside valid S&P 500 membership or IPO periods.

S&P 500 Membership Adjustments:
Incorporates historical membership changes, ensuring only relevant stocks are included during valid periods.
Filters out data for stocks pre-IPO or post-removal from the S&P 500.
Outlier Detection and Smoothing:

Identifies and smooths high spikes or anomalies in stock price data using Z-scores and Median Absolute Deviation (MAD).
Statistical Analysis: 
Calculates mean, variance, and cumulative returns for individual stocks.
Provides sector-based analysis and risk-adjusted performance metrics like Sharpe Ratios.

Visualization:
Generates clear, actionable visualizations, including:
Stock price trends over time.
Mean and variance distributions.
Cumulative returns with IPO start dates marked.
How It Works

Input Data:
Historical S&P 500 stock data, including adjusted closing prices, membership details, and IPO information (manually sourced from Bloomberg or other financial sources).

Code Workflow:
Data Cleaning: Filters and aligns data based on IPO and membership periods.
Outlier Handling: Detects and mitigates high variance or pinpoint spikes.
Analysis: Computes statistical metrics like mean, variance, and cumulative returns.
Visualization: Produces visual outputs to support portfolio optimization.

Output:
A cleaned, validated dataset ready for analysis or integration into machine learning models for portfolio optimization.
Insightful charts and summaries for exploratory data analysis.
