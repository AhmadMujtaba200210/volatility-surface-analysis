# Volatility Surface Analysis

**Quantitative Finance Project** – Construction of implied volatility surfaces, calibration of stochastic volatility models (Black–Scholes, Heston, SABR), and detection of option mispricing for volatility arbitrage strategies.  
This repository integrates **data engineering, mathematical finance, statistical modeling, and backtesting** to reflect industrial quant research standards.

---

## 📌 Overview
Volatility surfaces are a cornerstone of modern options markets.  
They encode the market’s expectations of risk and are essential for pricing, risk management, and trading strategies.  

This project aims to:
- Build implied volatility surfaces from real-world option chain data.
- Compare model-generated volatility (Black–Scholes, Heston, SABR) with observed market prices.
- Detect arbitrage opportunities and mispricings.
- Backtest volatility trading strategies (e.g., delta-hedged straddles, calendar spreads).
- Provide interactive visualization tools for analysis.

---

## 🚀 Features
- **Data Pipeline**
  - Automated fetching of option chain data (via `yfinance` and scraping APIs).
  - Storage in CSV/SQLite for reproducibility.

- **Implied Volatility Engine**
  - Newton–Raphson solver + `py_vollib` and `QuantLib` validation.
  - Greeks calculation for sensitivity analysis.

- **Exploratory Analysis**
  - Volatility smiles and skews across maturities.
  - Term structure visualization.

- **Surface Construction**
  - Spline-based interpolation for strikes/maturities.
  - Stochastic model calibration (Heston, SABR).

- **Arbitrage & Mispricing Detection**
  - Put–call parity validation.
  - Mispricing heatmaps.

- **Backtesting Framework**
  - PnL analysis of volatility-based trading strategies.
  - Greeks exposure tracking.

- **Interactive Dashboard**
  - 3D volatility surface visualization with Plotly/Dash.

---

## 📅 Roadmap
**Phase 1 (Weeks 1–2): Foundations & Data Pipeline**  
- Review Black–Scholes, volatility smile/skew, stochastic vol models.  
- Implement option chain scraper (Yahoo Finance, CBOE, Quandl).  

**Phase 2 (Weeks 3–4): EDA & IV Calculation**  
- Compute implied volatility numerically.  
- Plot smiles, skews, and term structures.  

**Phase 3 (Weeks 5–6): Surface Construction & Calibration**  
- Fit volatility surfaces using splines.  
- Calibrate SABR and Heston models.  

**Phase 4 (Weeks 7–9): Mispricing & Strategy Backtest**  
- Detect arbitrage violations and anomalies.  
- Backtest delta-hedged straddles / calendar spreads.  

**Phase 5 (Weeks 10–12): Dashboard & Final Report**  
- Build interactive volatility surface dashboard.  
- Deliver final report with methodology, results, and insights.  

---

## 📚 Resources

### **Mathematical Finance**
- Hull, *Options, Futures, and Other Derivatives* (Ch. 14–15, 19).  
- Joshi, *The Concepts and Practice of Mathematical Finance*.  
- Heston (1993), *A Closed-Form Solution for Options with Stochastic Volatility*.  
- Andersen & Piterbarg, *Interest Rate Modeling* Vol. 3 (SABR).  

### **Python Libraries**
- Core: `numpy`, `pandas`, `scipy`, `matplotlib`, `seaborn`  
- Options: `py_vollib`, `QuantLib`, `lmfit`  
- Data: `yfinance`, `requests`, `BeautifulSoup`  
- Backtesting: `backtrader`  
- Visualization: `plotly`, `dash`  

### **Data Sources**
- [Yahoo Finance API](https://pypi.org/project/yfinance/) – live option chains.  
- [CBOE DataShop](https://datashop.cboe.com/) – historical volatility and options data.  
- [Quandl / Nasdaq Data Link](https://data.nasdaq.com/) – EOD options & equity data.  
- [Kaggle Options Datasets](https://www.kaggle.com/) – pre-cleaned historical chains.  

---

## 📂 Repository Structure
