# Investment Portfolio Monte Carlo Simulation

This project performs a Monte Carlo simulation to analyze the long-term effects of borrowing to invest, with an emphasis on modeling investment returns, debt repayment, and portfolio growth over time.

## Project Overview

The simulation is designed to:
- Model monthly investments from a student loan over a 3-year period.
- Account for monthly compounding returns, leveraging historical ETF data for realistic daily returns.
- Calculate the final portfolio value over a long-term horizon, incorporating both investment growth and debt repayment dynamics.

The analysis reveals the probability of profitable outcomes, providing insights into potential risks and rewards associated with borrowing to invest.

## Simulation Details

1. **Initial Investment Phase**:
    - Duration: 36 months
    - Monthly Contribution: $500 (Note: The currency is USD)
    - Monthly Compounding: Uses randomly sampled daily returns from historical ETF data to estimate monthly returns.
    - Debt Accumulation: Loan balance accrues monthly interest based on an annual rate.

2. **Debt Repayment Phase**:
    - Duration: 13 years (156 months)
    - Monthly Payment: Minimum required, based on guidelines from SU.dk
    - Portfolio Continues to Grow: Monthly returns are applied to the portfolio, with debt gradually paid off.

3. **Result Analysis**:
    - Statistical summary of outcomes, including mean, median, standard deviation, and percentiles.
    - Insights into profitability: probability of positive returns, long-term growth potential, and optimal debt servicing considerations.

## Key Results

- **Median Portfolio Value**: $172,761 after 192 months.
- **Mean Portfolio Value**: $223,228, suggesting that, on average, this strategy leads to favorable outcomes.
- **Profitability**: All simulated scenarios yielded positive portfolio values, with a minimum of $53,605 (5th percentile). However, this is without considering the cost of servicing the debt

## Getting Started

### Prerequisites

- **Python 3.8+**
- Libraries: `numpy`, `pandas` for data manipulation, `matplotlib` (optional) for visualization. `yfinance` if you want to extract the data yourself (optional)

* Install required libraries:
    ```
    pip install -r requirements.txt
    ```
