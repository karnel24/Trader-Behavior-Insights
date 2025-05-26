# 🧠 Trader Behavior Insights Using KMeans & Market Sentiment

This project uncovers hidden trading patterns by combining **historical trader data** from Hyperliquid with the **Bitcoin Fear & Greed Index**. By clustering trades based on size, fee, sentiment, and PnL, we reveal what really drives profitable strategies in volatile crypto markets.

---

## 📈 Project Highlights

- ✅ **Unsupervised Clustering** with `KMeans` to group trades by behavioral patterns
- ✅ Integration of **Sentiment Data** (Fear, Greed) to understand emotional drivers
- ✅ Deep dive into the **most profitable cluster** — and why BTC surprisingly didn’t make the cut
- ✅ Coin-wise breakdowns and visual insights for high-conviction strategy building

---

## 📊 Key Findings (No Spoilers)

- One cluster outperformed the rest with ~30k avg PnL
- Top-performing trades weren't driven by Bitcoin
- Sentiment had a powerful influence — but not how you'd expect
- Retail vs. Whale trade behaviors clearly separated

👉 Full analysis and visuals are available in the [Jupyter Notebook](./Trader_Behavior_Insights.ipynb).

---

## 🔍 Data Used

### 1. Historical Trader Data (from Hyperliquid)
- Fields: `Coin`, `Size USD`, `Fee`, `Side`, `Closed PnL`, `Timestamp`, etc.

### 2. Bitcoin Fear & Greed Index
- Daily sentiment score (`0–100`) with labels like `Fear`, `Greed`, etc.

---

## 📦 Clustering Features

The following were used to train the `KMeans` model:
- `Size USD`
- `Fee`
- `Sentiment Value`
- `Closed PnL`

We use `StandardScaler` for normalization before clustering.

