# ACC102 Track 2: Comprehensive Stock Performance Quantitative Analysis Project
## GitHub Data Analysis Project

---

## 1. Project Purpose & Target User
This project builds a universal, reusable, and user-friendly Python stock analysis framework for individual investors, finance students, and long-term portfolio builders. It helps users objectively compare stock performance, risk characteristics, and risk-adjusted returns using standardized quantitative methods and clear visualizations.

The framework is fully customizable: users can input any valid U.S. stock tickers and any time period to conduct analysis. The stocks AAPL, MSFT, GOOGL and the period 2018–2023 are used only as demonstration examples.

---

## 2. Data Source & Description
- Data Platform: WRDS (Wharton Research Data Services)
- Database: CRSP Daily Stock File & CRSP Value-Weighted Market Index
- Access Date: April 2026
- Main Variables Used:
  - Date: Trading date
  - Price: Adjusted daily stock price
  - Return: Daily stock return
  - Market return: Value-weighted market index return (as benchmark)

---

## 3. Analytical Methods & Workflow
This project implements a complete quantitative stock analysis workflow in Python:

1. Data Extraction
Retrieve daily stock prices and returns from the WRDS database using SQL queries.

2. Data Cleaning & Preprocessing
Filter data by user-defined time period, convert dates to datetime format, remove missing values, and sort observations by date to ensure data quality and reliability.

3. Unified Standardization
All stock price series are rebased to a starting value of 1 to ensure fair and intuitive comparison regardless of original price levels.

4. Visualization & Risk-Return Analysis
Generate standardized charts including:
- Rebased price trend
- Cumulative return
- Rolling volatility
- Historical drawdown
- Rolling Sharpe ratio
- Return correlation heatmap
- Return distribution

5. Financial Indicator Calculation
Compute key investment metrics:
- Annualized return
- Annualized volatility
- Sharpe ratio
- Maximum drawdown
- Alpha and Beta (CAPM model)

6. Summary & Investment Scoring
Provide a structured summary of stock performance and a simple investment scorecard for decision support.

---

## 4. Key Findings
- Unified rebasing allows users to directly compare the performance of different stocks on the same timeline.
- Risk-adjusted returns measured by the Sharpe ratio effectively distinguish stock quality.
- Drawdown and volatility clearly reflect downside risk and stability during market fluctuations.
- Large-cap technology stocks typically show high return correlation and strong market sensitivity.
- In the demonstration case, AAPL presents the best overall balance between return and risk control.

---

## 5. How to Run the Project
1. Install all required Python libraries by running the following command:
pip install -r requirements.txt

2. Open the main Jupyter notebook file of this project.

3. Locate the parameter-setting cell at the beginning of the notebook.
Modify the following items as needed:
- Stock tickers
- Start year
- End year
- WRDS username

4. Run all cells in sequential order from top to bottom.

5. View the automatically generated charts, quantitative indicators, summary tables, and investment conclusions.

---

## 6. Product & Demo Link
- GitHub Repository: https://github.com/Xinyisong24/Comprehensive-Stock-Performance-Quantitative-Analysis
- Demo Video: https://video.xjtlu.edu.cn/mediasite/LTI/Assignment/Launch?id=5518ddc9499d4ccf84b15ce7472da44c
---

## 7. Limitations
- The analysis is based entirely on historical data, which cannot guarantee future performance.
- The project does not include company fundamental data such as revenue, profit, or valuation ratios.
- Real-world factors including transaction costs, taxes, and liquidity risk are not considered.
- The analysis does not incorporate macroeconomic conditions or external shocks.
- All outputs are for educational and analytical purposes only and do not constitute investment advice.

---

## 8. Future Improvements
- Add fundamental financial ratio analysis.
- Develop an interactive user interface for easier operation.
- Include portfolio optimization functionality.
- Support automated PDF report export.
- Expand data sources to support more global markets.

---

## 9. File Structure
- `Comprehensive Stock Performance Quantitative Analysis.ipynb`: Main Jupyter notebook with full analysis code
- `README.md`: Project documentation and user guide
- `requirements.txt`: List of required Python packages
