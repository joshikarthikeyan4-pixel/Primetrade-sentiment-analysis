# Primetrade-sentiment-analysis

# Trader Behavior vs Market Sentiment Analysis

## Objective
Analyze how Bitcoin market sentiment (Fear/Greed) influences trader behavior and performance on Hyperliquid. The goal is to identify actionable patterns that can inform smarter trading strategies.

---

## Datasets Used

1. **Bitcoin Fear & Greed Index**
   - Columns: Date, Classification
   - Daily market sentiment labels

2. **Hyperliquid Historical Trader Data**
   - Trade-level execution data
   - Includes PnL, size, side, timestamps, etc.

---

## Methodology

- Cleaned and validated both datasets.
- Converted timestamps and aligned data at daily level .
- Engineered key metrics:
  - Daily PnL per trader  
  - Win rate  
  - Trade frequency  
  - Average position size  
  - Long/short ratios  
- Merged trader metrics with market sentiment  
- Performed:
  - Sentiment regime analysis  
  - Trader segmentation  
  - Interaction analysis  
  - Volatility (drawdown proxy) analysis  

---

## Key Insights

- Frequent traders outperform infrequent traders on average daily PnL.
- Fear regimes tend to produce stronger trader profitability than greed regimes.
- Extreme Fear periods show the highest trading activity.
- Long bias increases slightly during fear regimes.
- Consistent winners maintain superior performance across regimes.
- PnL volatility spikes during extreme sentiment conditions.

---

## Strategy Recommendations

- **During Fear regimes:** Active traders may increase participation but should apply tight risk controls due to higher volatility.
- **During Extreme Greed:** Reduce position sizes and avoid overtrading as edge appears weaker.
- **For infrequent traders:** Focus on selective high-conviction trades rather than increasing frequency.
- **Risk management:** Volatility-aware position sizing is critical during sentiment extremes.

---

## How to Run

1. Clone the repository
2. Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn jupyter
