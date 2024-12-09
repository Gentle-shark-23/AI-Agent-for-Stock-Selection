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
