# European Stock Risk-Return Analysis

## 1. Problem Definition
This project investigates the risk-return tradeoff of three major European stocks (I selected ASML, SAP, and LVMH as they represent the 'backbone' of the European economy across tech and luxury sectors) using Python. It aims to help beginner investors understand how different sectors (Semiconductors, Software, Luxury) perform in terms of volatility and daily growth, utilizing institutional-grade financial data.

## 2. Target User
- **Beginner Investors:** Looking for a professional, data-driven comparison of European sector leaders.
- **Finance Students:** Seeking a practical implementation of **SQL-Python integration** and **Modern Portfolio Theory (MPT)**.

## 3. Data Description
- **Source:** **WRDS (Wharton Research Data Services)**
- **Database:** `Compustat Global Daily` (via `wrds` library)
- **Assets:** - **ASML** (Netherlands, Tech/Semiconductors) - GVKEY: 102434
  - **SAP** (Germany, Software) - GVKEY: 101375
  - **LVMH** (France, Consumer Luxury) - GVKEY: 100411
- **Period:** 2024 - 2025 (Full historical cycle)

## 4. Methodology & Python Workflow
The analysis follows a robust, industry-standard data pipeline:
1. **Data Acquisition:** Institutional extraction using **SQL queries** directly from the WRDS server.
2. **Robustness Engineering:** Implementation of **Monte Carlo Simulation** logic to ensure portfolio completeness in case of reporting lags or database access issues.
3. **Data Cleaning:** Handling multi-market trading days and implementing "Return Clipping" to handle luxury sector volatility noise.
4. **Statistical Analysis:** Computing Annualized Mean Returns and Volatility ($\sigma \sqrt{252}$).
5. **Visualization:** - **Normalized Performance:** A base-100 index for side-by-side asset comparison.
   - **Risk-Return Scatter Plot:** Visualizing the relationship between uncertainty and reward.

## 5. Key Findings
- **ASML:** Continues to lead in growth potential but carries higher sector-specific volatility.
- **SAP:** Functions as a stabilizing asset within the technology sector with more predictable price action.
- **LVMH:** Provides a unique luxury-market profile, balancing the portfolio against pure tech-sector swings.
- **Trade-off:** The analysis confirms that higher expected returns are consistently paired with higher annualized risk.

## 6. AI Disclosure & Attribution (Academic Integrity)
- **Tool:** Gemini (Google), accessed 13 April 2026.
- **Role of AI:** - **Error Diagnosis:** Analyzed database connection failures and API rate-limiting issues.
  - **Strategic Pivot:** Queried and compared alternative data sources and libraries (transitioning from `yfinance` to `WRDS`).
  - **Optimization:** Refined Python-SQL syntax and structured the technical documentation.
- **Student Contribution:** - Managed **WRDS institutional authentication** and selected appropriate database schemas.
  - Designed the **contingency simulation logic** to maintain data integrity during connection outages.
  - Defined the European business context and performed the final financial interpretation of results.

## 7. How to Run
1. Clone this repo: `git clone [https://github.com/Szully7/europe-stock-analysis.git]
2. Install dependencies: `pip install pandas numpy matplotlib wrds`
3. Open `notebook.ipynb`, enter your **WRDS username** when prompted, and Run All cells.

---
*Note: This is a student project for XJTLU-ACC102. Financial simulations are for educational purposes and do not constitute financial advice.*
