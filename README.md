# AQUA GARCH PROJECT — Quantitative Stock Analysis & Volatility Forecasting

## Overview

AQUA GARCH Project is a **quantitative finance analysis framework** built in Python for **Indian equity markets**.

The project performs:

* Multi-sector stock data collection
* Feature engineering & technical indicator generation
* Risk-adjusted performance screening
* Diversification analysis using correlations
* Defensive stock identification
* Volatility modeling using **GARCH**
* Time-series diagnostics using **ARIMA / Statistical Tests**

The objective is to support **portfolio construction, risk management, and volatility forecasting** through data-driven financial analysis.

---

## Features

### 1. Multi-Sector Market Data Collection

Collects historical stock data across **30 Indian equities** from multiple sectors.

**Sectors Covered:**

* Auto
* Banking
* IT
* Pharma
* FMCG
* Energy

**Data Source:** Yahoo Finance (`yfinance`)

**Time Period:** 2010-01-01 → 2021-05-01

---

### 2. Feature Engineering

Generated financial indicators include:

* Daily Returns
* Log Returns
* Rolling Volatility (21-day)
* Monthly Volatility
* Annualized Volatility
* OHLC Prices
* Trading Volume

---

### 3. Risk Metrics & Stock Screening

Computes advanced portfolio evaluation metrics:

#### Beta (β)

Measures systematic risk relative to market benchmark (`^NSEI`).

#### Sharpe Ratio

Evaluates risk-adjusted return.

#### Sortino Ratio

Measures return adjusted for downside volatility.

#### Maximum Drawdown

Captures worst historical portfolio decline.

#### Win Rate

Percentage of profitable trading days.

#### Annualized Return

Long-term performance estimation.

---

### 4. Diversification Analysis

Sector-wise correlation matrices are generated to identify:

* Low-correlation stock combinations
* Diversification opportunities
* Highly dependent sectors

Outputs include:

* Correlation heatmaps
* Recommended stock pairs
* Sector diversification assessment

---

### 5. Defensive Stock Classification

Filters equities with:

β < 1

These stocks are considered less volatile than the broader market and may suit conservative investors.

---

### 6. GARCH Volatility Modeling

Implements **ARCH/GARCH models** for conditional volatility estimation.

Applications:

* Volatility forecasting
* Risk management
* Value at Risk (VaR)
* Dynamic hedging
* Option pricing support

---

### 7. Time Series Diagnostics

Includes statistical analysis tools such as:

* ACF Plots
* PACF Plots
* Augmented Dickey-Fuller Test (ADF)
* KPSS Test
* Ljung-Box Test
* Jarque-Bera Test

---

### 8. Visualization

The notebook produces:

* Correlation Heatmaps
* Price Time Series Charts
* Return Distribution Plots
* Rolling Volatility Charts
* ACF / PACF Plots
* Q-Q Plots

---

## Project Structure

```text
AQUA-GARCH-PROJECT/
│
├── Aqua_Code_Final.ipynb
├── README.md
├── requirements.txt
└── outputs/
    ├── heatmaps/
    ├── volatility_plots/
    └── reports/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/AQUA-GARCH-PROJECT.git
cd AQUA-GARCH-PROJECT
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Run the Jupyter notebook:

```bash
jupyter notebook Aqua_Code_Final.ipynb
```

The notebook will:

1. Download stock data
2. Engineer features
3. Calculate risk metrics
4. Generate correlation analysis
5. Build volatility models
6. Produce visualizations

---

## Key Findings

| Finding                         | Result        |
| ------------------------------- | ------------- |
| Best Overall Stock              | Britannia     |
| Most Diversified Sector         | FMCG          |
| Lowest Beta Stock               | Dr. Reddy's   |
| Strongest Risk-Adjusted Returns | Pharma & FMCG |
| Highest Correlation Sector      | Banking       |

---

## Technology Stack

**Language:** Python 3.12

**Libraries:**

* pandas
* numpy
* scipy
* matplotlib
* seaborn
* statsmodels
* arch
* pmdarima
* scikit-learn
* yfinance

---

## Applications

### Portfolio Managers

* Portfolio screening
* Diversification planning
* Risk monitoring

### Risk Analysts

* VaR analysis
* Volatility forecasting
* Drawdown assessment

### Traders

* Volatility regime analysis
* Hedging support
* Signal evaluation

### Investors

* Defensive stock discovery
* Risk-adjusted performance comparison

---

## Future Improvements

Potential enhancements:

* LSTM volatility forecasting
* Portfolio optimization (Markowitz / Black-Litterman)
* Interactive dashboard deployment
* Real-time market streaming
* Monte Carlo simulation integration

---

## License

This project is intended for **educational and research purposes**.
