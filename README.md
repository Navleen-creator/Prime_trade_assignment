# Prime_trade_assignment
This project analyzes how Bitcoin market sentiment (Fear/Greed Index) influences trader behavior and profitability on Hyperliquid.
The goal is to identify behavioral patterns, segment traders, and evaluate whether sentiment can help predict trading performance.

# Trader Performance vs Market Sentiment (Primetrade.ai Assignment)

## Objective
This project analyzes how Bitcoin market sentiment (Fear/Greed) impacts trader behavior and profitability on Hyperliquid.

## Dataset
- Bitcoin Fear & Greed Index (daily sentiment)
- Hyperliquid historical trades (account-level transactions)

## Methodology

1. Data Cleaning
   - Converted timestamps to daily format
   - Removed duplicates and handled missing values

2. Feature Engineering
   - Daily PnL per account
   - Trade frequency
   - Win rate
   - Average trade size
   - Long/short bias
   - Sentiment alignment (Fear/Greed)

3. Clustering
   - KMeans used to identify trader archetypes:
     - High-frequency traders
     - High-risk high-reward traders
     - Conservative traders

4. Predictive Model
   - Random Forest classifier used
   - Target: next-day profitability (positive/negative PnL)
   - Features: trading behavior + sentiment

## Key Insights

- Traders show higher activity during Fear periods
- Greed days have higher trade sizes but lower win consistency
- High-frequency traders are less sensitive to sentiment changes
- Sentiment has predictive value when combined with behavioral features


## Strategy Recommendations

- Reduce leverage exposure during Extreme Greed conditions
- High-frequency traders perform better in Fear regimes
- Low-frequency traders should avoid trading during high volatility sentiment shifts


## Tech Stack
- Python (Pandas, NumPy)
- Scikit-learn
- Matplotlib / Seaborn
- Streamlit
  ## How to Run

```bash
pip install -r requirements.txt
python analysis.py
streamlit run appp.py



python analysis.py
streamlit run app.py
