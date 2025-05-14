# 📊 Portfolio Risk Analysis and VaR Backtesting

This project is a comprehensive portfolio risk analysis framework implemented in Python. It calculates Value at Risk (VaR), Conditional VaR (CVaR), and multiple other risk metrics using various industry-standard models. The framework also features extensive backtesting with Kupiec’s test, stress testing, 10-day VaR analysis, and risk contribution decomposition.

---

## 🚀 Features

- ✅ Historical, Parametric (Normal & Student-t), GARCH, Filtered Historical, and Monte Carlo VaR
- 📉 CVaR calculation (Expected Shortfall)
- 📊 10-day VaR via square-root-of-time and true Monte Carlo simulation
- 📈 Sharpe Ratio, Maximum Drawdown, and Stress Testing
- 📤 Incremental (Marginal) VaR per asset
- 🧪 Kupiec’s Proportion of Failures (POF) test for backtesting VaR
- 📁 Modular and production-ready design with logging and result tracking

---

## 📘 Methods Implemented

1. **VaR Models**
   - Historical Simulation
   - Parametric Normal
   - Parametric Student-t
   - GARCH (Volatility modeling)
   - Filtered Historical Simulation (FHS)
   - Monte Carlo Simulation

2. **Risk Metrics**
   - Conditional VaR (CVaR)
   - 10-day VaR (sqrt scaling & true MC)
   - Sharpe Ratio
   - Max Drawdown
   - Stress Testing under 5% portfolio shock
   - Incremental VaR per asset

3. **Backtesting**
   - Kupiec POF test on multiple VaR models
   - Reporting breaches and statistical significance

---

## 📊 Results Summary

### VaR @ 95% Confidence Level

| Model                  | VaR ($)     |
|------------------------|-------------|
| Historical             | 0.0331      |
| Parametric Normal      | 0.0547      |
| Parametric Student-t   | 0.0349      |
| GARCH                  | 0.0501      |
| Filtered Historical    | 0.0371      |
| Monte Carlo            | 0.0499      |
| CVaR                   | 0.0466      |
| 10-day VaR (sqrt)      | 0.1103      |
| True 10-day MC VaR     | 0.0875      |

### VaR @ 99% Confidence Level

| Model                  | VaR ($)     |
|------------------------|-------------|
| Historical             | 0.0533      |
| Parametric Normal      | 0.0779      |
| Parametric Student-t   | 0.0559      |
| GARCH                  | 0.0714      |
| Filtered Historical    | 0.0604      |
| Monte Carlo            | 0.0710      |
| CVaR                   | 0.0703      |
| 10-day VaR (sqrt)      | 0.1767      |
| True 10-day MC VaR     | 0.1363      |

### Portfolio Risk Metrics

- **Sharpe Ratio**: 0.0600  
- **Max Drawdown**: -49.05%  
- **Stress Test (5% Shock)**: $-0.04877  

### Incremental VaR @ 95% Level

| Ticker | Incremental VaR ($) |
|--------|---------------------|
| AAPL   | -0.000099           |
| MSFT   | -0.000094           |
| GOOGL  | -0.000067           |
| AMZN   | -0.000005           |
| TSLA   |  0.000274           |

### VaR Backtesting (Kupiec Test @ 95%)

| Model                  | Breaches | Expected | p-value   | Acceptable |
|------------------------|----------|----------|-----------|------------|
| Parametric Normal      | 67       | 54.45    | 0.0916    | ✅         |
| Parametric Student-t   | 52       | 54.45    | 0.7315    | ✅         |
| GARCH                  | 57       | 54.45    | 0.7249    | ✅         |
| Filtered Historical    | 50       | 54.45    | 0.5307    | ✅         |
| Monte Carlo            | 60       | 54.45    | 0.4474    | ✅         |

---

## 🛠️ Installation & Setup

# Clone the repository
git clone https://github.com/yourusername/portfolio-risk-analysis.git
cd portfolio-risk-analysis

# (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install required packages
pip install -r requirements.txt


## 🙌 About Me

If you're working on financial risk modeling, portfolio risk analysis — let’s connect!

👤 **Surajit Biswas, Ph.D.**  

🔗  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/surajit-biswas-phd/)

📫 surajitbiswas.iiserb@gmail.com

---

## 🏷️ Tags

`VaR Analysis` `Portfolio Risk Modeling` `Tenso `Data Science` `Finance`
