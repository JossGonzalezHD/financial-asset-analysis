# 📊 Financial Asset Analysis for AI Trading Bot

> Exploratory Data Analysis (EDA) and visual intelligence report to identify 
> the best-performing assets per industry sector, optimizing the watchlist 
> of an AI-assisted trading system.

---

## 🎯 Objective

Analyze 15 financial assets across 5 industry sectors over a 12-month period 
(May 2025 – May 2026) to determine which assets offer the best risk/return 
profile for an algorithmic trading bot based on technical confluence signals.

---

## 📁 Project Structure

```
financial-asset-analysis/
│
├── notebooks/
│   └── financial_asset_analysis.ipynb
│
├── images/
│   ├── grafica1_retorno_total.png
│   ├── grafica2_boxplot_industrias.png
│   ├── grafica3_evolucion_industrias.png
│   └── grafica4_senal_vs_retorno.png
│
└── README.md
```

## 🔬 Methodology

| Variable | Type | Description |
|---|---|---|
| `asset` | Nominal | Financial instrument ticker (BTC-USD, NVDA, GLD) |
| `trend` | Ordinal | Market direction via EMA20 (Bearish / Sideways / Bullish) |
| `signal_days` | Discrete | Days with extreme movement (±3% daily return) |
| `daily_return` | Continuous | Daily percentage price change |

**Data Source:** Yahoo Finance via `yfinance`  
**Universe:** 15 assets — Crypto, Technology, Commodities, Health, Broad Market  
**Period:** May 2025 – May 2026 (251 trading days)

---

## 📈 Key Findings

| Industry | Annual Return | Volatility (IQR) | Bot Priority |
|---|---|---|---|
| Commodities | +62.9% | 2.40% | ⭐ High |
| Broad Market | +32.8% | 1.06% | ⭐ High |
| Health | +31.2% | 1.35% | ⭐ High |
| Technology | +26.2% | 1.52% | ✅ Medium |
| Crypto | -20.1% | 3.73% | ⚠️ Conditional |

### Optimized Watchlist

```python
watchlist_bot = {
    "Commodities":    ["USO", "GLD"],
    "Broad Market":   ["IWM"],
    "Health":         ["JNJ"],
    "Technology":     ["NVDA"],
    "Crypto":         ["ETH-USD"]
}
```

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

---

## 🔗 Related Projects

- [trading-ai-bot](https://github.com/JossGonzalezHD/trading-ai-bot) — 
AI-assisted trading system this analysis was built for

---

## 👤 Author

**Joseph González**  
Operations & Automation Specialist | M.S. IT Management (Cloud Computing & Data Science)  
[LinkedIn](https://www.linkedin.com/in/joseph-gonzalez-2473b5216/) · 
[GitHub](https://github.com/JossGonzalezHD)
