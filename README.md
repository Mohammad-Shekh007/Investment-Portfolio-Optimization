# Investment-Portfolio-Optimization

# Portfolio Optimization using Linear Optimization and Monte Carlo Simulation

## Overview

This project develops a wealth management portfolio optimization model using historical market data, Excel Solver, and Monte Carlo simulation techniques.

The objective is to identify the portfolio that maximizes expected monthly return while satisfying a set of investment policy and diversification constraints.

---

## Data

Historical monthly return data (2010–2025) were collected for eight asset classes:

* SPY (S&P 500 ETF)
* QQQ (NASDAQ 100 ETF)
* IWM (Russell 2000 ETF)
* VEA (Developed International Markets ETF)
* VNQ (Real Estate ETF)
* GLD (Gold ETF)
* BND (Total Bond Market ETF)
* TB3MS (3-Month Treasury Bills)

Expected return was estimated using historical average monthly returns, while risk was measured using the historical standard deviation of monthly returns.

---

## Methodology

### Portfolio Optimization

The portfolio was constructed subject to the following constraints:

* Exactly 5 asset classes must be selected.
* No more than 2 Growth assets may be selected.
* At least 1 Income asset must be selected.
* Defensive assets must be greater than or equal to Growth assets.

Excel Solver was used to identify the portfolio that maximizes expected monthly return.

### Alternative Portfolio Construction

A second optimization model was created by introducing an additional diversification constraint:

* No more than 3 of the 5 assets selected in Portfolio 1 may appear in Portfolio 2.

This produced an alternative optimal portfolio for comparison.

### Monte Carlo Simulation

A Monte Carlo simulation consisting of 1,000 randomly generated scenarios was performed to evaluate the robustness of both portfolios under uncertainty.

---

## Results

### Portfolio 1 (Optimal Portfolio)

Assets Selected:

* SPY
* QQQ
* VNQ
* GLD
* BND

Expected Monthly Return:

* 4.68%

### Portfolio 2 (Alternative Portfolio)

Assets Selected:

* QQQ
* IWM
* VNQ
* GLD
* TB3MS

Expected Monthly Return:

* 4.45%

### Monte Carlo Analysis

Across 1,000 simulated market scenarios:


Portfolio 1 : Average Simulated Return =	4.23%
Portfolio 1 : Standarad Deviation = 9.59%
Portfolio 2 : Average Simulated Return =	4.15%
Portfolio 2 : Standarad Deviation = 10.35%
Probability of (Portfolio 1 Return > Portfolio 2 Return) = 51.20% out of 1000 uncertain scenarios


* Portfolio 1 generated a slightly higher average return.
* Risk levels were similar across both portfolios.
* Portfolio 1 outperformed Portfolio 2 by a narrow margin.

---

## Conclusion

Portfolio 1 is recommended because it achieved the higher expected return and marginally outperformed Portfolio 2 in the Monte Carlo simulations. However, the small performance difference suggests that both portfolios are viable investment choices and demonstrate similar behavior under uncertainty.

---

## Files

* Portfolio Optimization Report (PDF)
* Excel Optimization & Monte Carlo Model
* Supporting Screenshots

---

**Tools Used:** Excel Solver, Monte Carlo Simulation, Portfolio Optimization, Financial Analytics

## Practical Applications

This framework can support portfolio construction, asset allocation analysis, diversification assessment, and investment decision-making. The model can be adapted to different investor objectives, risk tolerances, and market assumptions while providing a structured approach to evaluating portfolio performance under uncertainty.
