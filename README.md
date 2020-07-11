# How do you Like them Apps?

![FTimage](Images/ft_image.png)

*This repository contains the Unit 5 homework assignment, "How do you Like them Apps"  in the FinTech bootcamp course at the University of Toronto's School of Continuing Studies.*

---

## Table of Contents

- [Project Description](#Project-Description)
- [Installation Requirements](#Installation-Requirements)
- [File Contents](#File-Contents)

---

## Project Description 

The following assignment uses Plaid and Alpaca API keys to retireve historical stock data for "AGG" and "SPY" to conduct a retirement portfolio projection analysis.

### Part 1:

Part one of the assignment, "Budget Analysis with Plaid" provides a traditional budget analysis to determine the previous years' annual income, the current monthly income, and a projected income for the following year pre tax.

### Part 2:

The second assignment deliverable, "Retirement Portfolio Planner" provides an analysis and projection of a retirement portfolio based on the 2019 historical data for the tickers; "AGG" and "SPY." The analysis consists of a Monte Carlo simulation and a cumulative returns calculations based on a principle investment and thirty year expected returns period. 

*This section includes 2 bonus challenges* 

Both challenges provide different variables to determine the retirement portfolio's cumulative returns changes throughout the time period of the investment, and an alternate scenario for an earlier retirement. 

### Part 3:

In the final section of the assignment, a financial analysis is conducted to demo and display the results of the Budget Analysis and the Retirement Portfolio Planner.

---

## Installation Requirements 

* You will need API Keys from the following developer accounts to run and display the code created in this assignment; 
    * PLAID
    * ALPACA

```
pip install pandas
pip install numpy
pip install matplotlib
pip install plaid-python
pip install alpaca-trade-api
```

---

## Files
* [Assignment Instructions](Unit_5_Assignment_Instructions.md) 
* [Part 1: PLAID Budget Analysis](Budget_Analysis/account_summary.ipynb)
* [Part 2: Retirement Portfolio Planner](Retirement_Planner/portfolio_planner.ipynb)
* [Part 3: Financial Report](Financial_Report)
