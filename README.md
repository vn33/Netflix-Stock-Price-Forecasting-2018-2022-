# Netflix Stock Price Forecasting (2018–2022) 📈

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![RMSE](https://img.shields.io/badge/Best%20RMSE-8.86-green)]()

*A time-series forecasting project analyzing Netflix (NFLX) stock data to predict future prices using statistical models.*

---

## Table of Contents
- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Installation](#installation)
- [Usage](#usage)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Building](#model-building)
- [Key Findings](#key-findings)
- [Results](#results)
- [Tools & Technologies](#tools--technologies)
- [License](#license)
---

## Project Overview
This project analyzes **5 years of Netflix stock prices** (2018–2022) to forecast future trends using time-series models. Key steps include:
- **Exploratory Data Analysis (EDA)** with decomposition and stationarity checks.
- Implementation and comparison of **10+ forecasting models** (SARIMA, ARIMA, Holt-Winters, etc.).
- Hyperparameter tuning using AIC/BIC criteria.

**Best Model**: SARIMA achieved an **RMSE of 8.86**, outperforming baseline models by **23%**.

---

## Key Features
- ✅ **EDA**: Box plots, seasonal decomposition, and Augmented Dickey-Fuller (ADF) tests.
- ✅ **Stationarity Handling**: Differencing and log transformations.
- ✅ **Model Suite**: AR, MA, ARMA, ARIMA, SARIMA, and exponential smoothing variants.
- ✅ **Diagnostics**: ACF/PACF plots, residual analysis, and model robustness checks.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/vn33/Netflix-Stock-Price-Forecasting-2018-2022-.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
---

## Usage
1. Run Jupyter Notebook for EDA and model training:
   ```bash
   jupyter notebook TimeSeries_analysis.ipynb
   ```
---

## Exploratory Data Analysis (EDA)
- **Time-Series Decomposition:** Trend, seasonality, and residuals visualized.
- **Stationarity Tests:** ADF test with p-value thresholds.
- **Visualizations:** Box plots for volatility analysis and rolling statistics.

---

## Model Building
- **Baseline Models:** Naive, Moving Average, Exponential Smoothing.
- **Advanced Models:** ARIMA (grid-searched parameters), SARIMA (seasonal adjustment).
- **Validation:** RMSE comparison and residual diagnostics.

---

## Key Findings
1. **SARIMA Dominance:** Outperformed all models due to seasonal adjustment (RMSE: 8.86).
2. **ARIMA Overfitting:** Poor performance (RMSE: 13.62) resolved via hyperparameter tuning.
3. **Trend vs. Seasonality:** Netflix stock showed significant seasonal patterns.

---

## Results

| Model                           | RMSE  | Improvement vs. Baseline |
|---------------------------------|-------|--------------------------|
| Naive Model                     | 11.05 | -                        |
| Moving Average                  | 9.81  | 11%                      |
| Single Exponential Smoothing    | 11.07 | -0.2%                   |
| Double Exponential Smoothing    | 11.17 | -1.1%                   |
| Triple Exponential Smoothing    | 11.26 | -1.9%                   |
| Autoregression                  | 10.18 | 7.9%                    |
| ARMA                            | 10.97 | 0.7%                    |
| ARIMA                           | 13.62 | -23.2%                  |
| SARIMA                          | 8.86  | 19.8%                   |
| SARIMAX                         | 8.86  | 19.8%                   |

---

## Tools & Technologies
- **Languages:** Python
- **Libraries:** Pandas, NumPy, statsmodels, Matplotlib, Seaborn
- **Methods:** ADF Test, ACF/PACF, SARIMA, SARIMAX

---

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
