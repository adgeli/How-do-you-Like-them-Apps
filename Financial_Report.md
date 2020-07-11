# Financial Report

This financial report provides the Consumer App Team income analysis and retirement portfolio projections. 
The use of the PLAID API developer sandbox and ALPACA historical trade data provides the team with the selected retirement portfolio's projected thirty year performance based on the budget and investment simulations presented in the Account Summary and Portfolio Planner files.

---
## Report Outline

- [Account Summary](#Account-Summary)
    - [Budget Analysis](#Budget-Analysis)
    - [Income Summary](#Income-Summary)

- [Retirement Portfolio](#Retirement-Portfolio)
    - [Monte Carlo Simulation](#Monte-Carlo-Simulation)
    - [Performance Analysis](#Performance-Analysis)
    - [Challenge 1: Retirement Analysis]
    - [Challenge 2: Early Retirement]

---

## Account Summary

This section uses the PLAID API key to retireve transaction and account data for a 90 day period to complile a budget analysis and income summary. 

### Budget Analysis

Through the use of a transactions dataframe, consumer spending was calculated to produce a tabular and graphical representation of expenses per spending category. Observed in the "Expenses Pie Graph", a significant percentage of consumer spending originates from the "Transfer" expense category. Additionally, based on the retireved data, it is evident that the three month spending habits are fairly consistent ranging from $10 560.06 to $10 645.24. The final displayed month (7) is believed to be incomplete data. The spending data for this month was $101.51, therefore, does not produce a complete bar in the "Spending per Month Bar Chart."

* The budget analysis is displayed through an "Expenses Chart", "Expenses Pie Graph", and a "Spending per Month Bar Chart."

#### Expenses Chart
| Category      | Amount |
| ----------- | ----------- |
| Food and Drink | 3317.19
Payment      |   6310.50
Recreation   |     235.50
Shops        |    1500.00
Transfer    |    20537.34
Travel       |     35.19 

#### Expenses Pie Graph

![Expenses_Pie_Chart](Images/Expenses_pie_chart.png)

#### Spending per Month Bar Chart

![Bar_Chart](Images/Spending_barchart.png)

### Income Summary

The income data fetched through the PLAID sandbox is; 

- Previous year gross income: $7285

- Current monthly income: $500

- Projected yearly income pre tax: $7389

- Projected yearly income post tax: $6085

---

## Retirement Portfolio

In the Retirement Portfolio section, the use of an ALPACA API retrieves the historical closing prices for a retirement portfolio; SPY (SPDR S&P 500 ETF) and AGG (iShares Core U.S. Aggregate Bond ETF). Through the use of Monte Carlo simulations, the portfolio's performance is projected over a 30 year time period. Based on 500 iterations, the portfolio analysis suggests investment in the selected portfolio will yield a potential profit at the end of the period. 

The retirement portfolio consists of a 60% stock, "SPY", and 40% bond, "AGG" allocation. 

* Portfolio Volatility: 
    * SPY: 0.00782
    * AGG: 0.00208

* Portfolio Average Daily Returns: 
    * SPY: 0.00104
    * AGG: 0.00021 

### Monte Carlo Simulation

The Monte Carlo simulation consists of 500 simulations throughout the 30 year timeframe. 

![monte_carlo](Images/monte-carlo.png)

At a 90% confidence interval, the investment dollar yield ranges from $34.50 to $92.24. Most likely providing a return at $63.37.

![Frequency](Images/frequency.png)

### Performance Analysis

#### Cumulative Returns at the End of 30 Years

| Percentile      | Cumulative Return |
| ----------- | ----------- |
| 10th Percentile |  41.261998
50th Percentile   |    57.734117
90th Percentile   |    82.333470

#### Portfolio Returns Given a $20 000 Initial Investment

| Percentile      | Cumulative Return |
| ----------- | ----------- |
| 10th Percentile |  $845240.0
50th Percentile   |    $1174682.0
90th Percentile   |    $1666669.0

#### Portfolio Returns Given a $30 000 Initial Investment

| Percentile      | Cumulative Return |
| ----------- | ----------- |
| 10th Percentile |  $1267860.0
50th Percentile   |    $1762024.0
90th Percentile   |    $2500004.0

The historical data for the retirement portfolio consisting of 60% "SPY" stocks and 40% "AGG" bonds returned high equities for retrieved 2019 period. Thus, a 4% retirement withdrawl at either a $20 000 or $30 000 principal investment does not affect the current post tax annual income of $6085. 