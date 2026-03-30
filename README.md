# 📈 S&P 500 Market Direction Predictor

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11+-blue.svg" alt="Python 3.11+">
  <img src="https://img.shields.io/badge/ML-XGBoost%20%7C%20LightGBM%20%7C%20RandomForest-green.svg" alt="ML Models">
  <img src="https://img.shields.io/badge/Viz-Plotly-purple.svg" alt="Plotly">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License">
</p>

An advanced machine learning system for predicting S&P 500 market direction using ensemble methods, 30+ technical indicators, and professional-grade backtesting with portfolio simulation.

---

## 🎯 Project Highlights

| Feature | Description |
|---------|-------------|
| **30+ Technical Indicators** | RSI, MACD, Bollinger Bands, ATR, OBV, Stochastic, Williams %R, and more |
| **Ensemble ML Models** | XGBoost, LightGBM, and Random Forest with weighted voting |
| **Walk-Forward Backtesting** | Realistic evaluation that avoids look-ahead bias |
| **Portfolio Simulation** | Actual P&L tracking with transaction costs |
| **Model Explainability** | SHAP values and feature importance analysis |
| **Risk Metrics** | Sharpe ratio, max drawdown, win rate, annual returns |
| **Interactive Visualizations** | Beautiful Plotly charts with dark theme |

---

## 📊 Screenshots

### Technical Analysis Dashboard
Interactive candlestick charts with Bollinger Bands, MACD, RSI, and volume analysis.

### Portfolio Performance
Compare model strategies vs Buy & Hold with cumulative returns visualization.

### Model Explainability
SHAP values showing which features drive predictions.

---

## 🚀 Quick Start

```powershell
# Clone and enter directory
cd Stock-Predictor

# Create virtual environment
python -m venv venv
.\venv\Scripts\Activate.ps1  # Windows
# source venv/bin/activate   # Linux/Mac

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook sp500_predictor.ipynb
```

---

## 📁 Project Structure

```
Stock-Predictor/
├── sp500_predictor.ipynb   # Main notebook (run this!)
├── data.ipynb              # Original exploration notebook
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── venv/                   # Virtual environment
```

---

## 🔧 Technical Indicators

### Trend Indicators
- Simple Moving Averages (5, 10, 20, 50, 200 days)
- Exponential Moving Averages (12, 26, 50 days)
- MACD (Moving Average Convergence Divergence)
- Golden/Death Cross signals

### Momentum Indicators
- RSI (Relative Strength Index) - 7, 14, 21 periods
- Stochastic Oscillator (%K, %D)
- Rate of Change (ROC)
- Williams %R
- Momentum (10, 20 days)

### Volatility Indicators
- Bollinger Bands (Width, Position)
- ATR (Average True Range)
- Historical Volatility (20, 60 days)

### Volume Indicators
- On-Balance Volume (OBV)
- Volume Moving Averages
- Volume Ratio

### Price Patterns
- Candlestick body ratios
- Gap analysis
- Intraday range

---

## 🤖 Machine Learning Pipeline

```
Data Acquisition → Feature Engineering → Walk-Forward Backtest → Ensemble Prediction
      ↓                    ↓                      ↓                     ↓
  Yahoo Finance      30+ Indicators        Train/Test Splits      Weighted Voting
                                                  ↓
                                          Portfolio Simulation
                                                  ↓
                                          Risk Metrics & SHAP
```

### Models Used

| Model | Key Parameters |
|-------|----------------|
| **XGBoost** | n_estimators=200, max_depth=4, learning_rate=0.05 |
| **LightGBM** | n_estimators=200, num_leaves=15, learning_rate=0.05 |
| **Random Forest** | n_estimators=200, max_depth=6, min_samples_split=50 |
| **Ensemble** | Weighted average (XGB: 40%, LGBM: 35%, RF: 25%) |

---

## 📈 Performance Metrics

The notebook calculates:

- **Classification**: Precision, Recall, F1, AUC-ROC
- **Trading**: Annual Return, Sharpe Ratio, Max Drawdown, Win Rate
- **Portfolio**: Cumulative returns with transaction costs

---

## 🎨 Visualization Features

- Interactive Plotly charts with dark theme
- Candlestick charts with overlays
- ROC curves for model comparison
- Confusion matrices
- Drawdown analysis
- Portfolio growth comparison

---

## ⚠️ Disclaimer

This project is for **educational purposes only**. 

- Past performance does not guarantee future results
- This is not financial advice
- Always do your own research before making investment decisions
- The stock market involves significant risk of loss

---

## 📚 References

1. López de Prado, M. (2018). *Advances in Financial Machine Learning*
2. Murphy, J. J. (1999). *Technical Analysis of the Financial Markets*
3. Chen, T., & Guestrin, C. (2016). *XGBoost: A Scalable Tree Boosting System*

---

## 📄 License

MIT License - feel free to use this for your own projects!

---

<p align="center">
  <b>Built with 🐍 Python | 📊 XGBoost | 📈 Plotly</b>
</p>
