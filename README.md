# Stock-Price-Predictor

# 📈 Stock Price Movement Predictor – S&P 500

This project explores time series modeling by predicting **whether the S&P 500 index will go up or down** using historical stock market data. The emphasis is on **directionality prediction**, which is more actionable in financial decisions than predicting exact price values.

## 🔍 Overview

- **Goal**: Predict if the S&P 500 (^GSPC) will increase or decrease on the next trading day.
- **Data Source**: Yahoo Finance API via `yfinance` package
- **Model Type**: Binary classification (Up vs. Down)
- **Focus**: Time series preparation, directional prediction, and visual exploration

## 🧠 Key Highlights

- Collected historical daily prices for S&P 500 using `yfinance`
- Engineered features for ML classification: % change, moving averages, momentum indicators
- Set up a **classification target** instead of price regression to align with real-world trading logic
- Emphasized that in financial forecasting, **directional accuracy > absolute accuracy**
- Visualized data trends and movements to understand the underlying time series structure

## 🛠 Technologies Used

| Tool/Library       | Purpose                              |
|--------------------|--------------------------------------|
| `yfinance`         | Downloading stock market data        |
| `pandas`           | Data manipulation                    |
| `matplotlib`       | Visualization                        |
| `NumPy`            | Numeric operations                   |
| `scikit-learn`     | ML preprocessing and classification  |

## 📊 Data Strategy

- Target: `1` if the stock closes higher than the previous day, else `0`
- Focus on relative movement (up/down), not absolute stock price
- Cleaned and validated data to remove anomalies and missing values

## 📈 Modeling Philosophy

Instead of predicting the exact closing price (which may be accurate but not useful), this project prioritizes **"up or down" prediction**, which aligns more closely with:
- Investment decisions
- Portfolio hedging
- Risk assessment

## 📂 Project Structure

```bash
├── StockPredictor.ipynb      # Full analysis and modeling notebook
├── README.md                 # Project overview
