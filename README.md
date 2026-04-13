# European Stock Risk-Return Analysis 🇪🇺

## 1. Problem Definition
This project investigates the risk-return tradeoff of three major European stocks (ASML, SAP, LVMH) using Python. It aims to help beginner investors understand how different sectors (Semiconductors, Software, Luxury) perform in terms of volatility and daily growth.

## 2. Target User
- **Beginner Investors:** Looking to understand how to diversify across different European sectors.
- **Finance Students:** Seeking a practical Python implementation of risk metrics (Standard Deviation) vs. Performance.

## 3. Data Description
- **Source:** Yahoo Finance (via `yfinance` library)
- **Assets:** - **ASML** (Netherlands, Tech/Semiconductors)
  - **SAP** (Germany, Software)
  - **LVMH** (France, Consumer Luxury)
- **Period:** Last 1 year (Daily frequency as of April 2026)

## 4. Methodology & Python Workflow
The analysis follows a robust data pipeline:
1. **Data Acquisition:** Automated download using `yfinance`.
2. **Cleaning:** Handling missing values and calculating Percentage Change for daily returns.
3. **Statistical Analysis:** Computing Mean Returns and Annualized Volatility (Standard Deviation).
4. **Visualization:** - Interactive Price Trends (Matplotlib)
   - Risk-Return Scatter Plot to visualize the "Efficient Frontier" logic.

## 5. Key Findings
- **ASML:** Exhibits high growth potential but with the highest volatility among the three, suitable for aggressive portfolios.
- **SAP:** Shows the most stable price movement, acting as a defensive asset in this selection.
- **LVMH:** Provides a balanced profile, reflecting the steady demand in the luxury sector.
- **Correlation:** Risk and return are generally positively related, confirming that compensation is required for higher uncertainty.

## 6. AI Disclosure & Attribution (Academic Integrity)
- **Tool:** Gemini (Google), accessed 13 April 2026.
- **Role of AI:** Used to generate the initial structure of the Python notebook.
- **Student Contribution:** - Defined the specific European stock tickers and business context.
  - Debugged the `yfinance` data calling function.
  - Interpreted the statistical results to provide sector-specific insights (Tech vs Luxury).
  - Designed the user-facing README structure to ensure clarity for beginner investors.
  - Provided the financial interpretation of the results.

## 7. How to Run
1. Clone this repo: `git clone https://github.com/[Your-Username]/europe-stock-analysis.git`
2. Install dependencies: `pip install pandas matplotlib yfinance`
3. Open `notebook.ipynb` and Run All cells.

---
*Note: This is a student project for XJTLU-ACC102. Not financial advice.*
