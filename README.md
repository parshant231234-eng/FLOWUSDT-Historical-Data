# FLOWUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **FLOWUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `FLOWUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `64` months
- **Total Candles:** `2,743,389` 1-minute candles
- **Historical Range:** `2021-07-30 13:00:00` to `2026-10-17 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
FLOWUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── FLOWUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/FLOWUSDT-Historical-Data/main/1m/2026/10/FLOWUSDT_1m_2026-10.csv"
df = pd.read_csv(url)
print(df.head())
```
