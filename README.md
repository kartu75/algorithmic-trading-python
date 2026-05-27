# Algorithmic Trading with Python

Three quantitative trading strategies built with Python and yFinance.

## Projects

### 1. Equal Weight S&P 500
Builds an equal-weight version of the S&P 500 index. Instead of weighting stocks by market cap (like the actual index), this strategy allocates equal dollar amounts to each of the 500 stocks. Given a portfolio size, it calculates the number of shares to buy for each stock.

### 2. Quantitative Momentum Strategy
Identifies the 50 highest-momentum stocks in the S&P 500 using a High Quality Momentum (HQM) score. Rather than relying on a single return period, the HQM score averages momentum percentiles across four timeframes (1-year, 6-month, 3-month, 1-month) to find stocks with consistent momentum across all periods.

### 3. Quantitative Value Strategy
Identifies the 50 most undervalued stocks in the S&P 500 using a Robust Value (RV) score. The RV score averages valuation percentiles across five metrics (P/E, P/B, P/S, EV/EBITDA, EV/GP) to avoid relying on any single valuation measure.

## Tech Stack
- Python
- Pandas
- yFinance
- NumPy
- SciPy
- XlsxWriter

## Output
Each strategy outputs a formatted Excel file with recommended trades and number of shares to buy based on a given portfolio size.

## Notes
- Data sourced from Yahoo Finance via yFinance
- S&P 500 ticker list from `sp_500_stocks.csv`
