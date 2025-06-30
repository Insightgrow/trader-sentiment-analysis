# Trader Behavior vs. Market Sentiment Analysis

This project analyzes how Bitcoin trader performance changes under different market sentiment conditions (Fear vs. Greed). 
By combining a sentiment dataset with historical trader data, we uncover insights that drive smarter trading strategies.

---

##  Datasets Used
- **Hyperliquid Historical Trader Data**
- **Fear-Greed Index (Sentiment Classification)**

---

## Key Findings from EDA
- Traders were **slightly more profitable during Greed** (41.3%) than Fear (40.8%)
- However, **losses were larger and overtrading more common** in Greed
- Traders showed **more discipline during Fear**, paying higher fees but trading more cautiously

---

## ML Model Summary
Trained a logistic regression model to predict if a trade would be profitable based on:
- Market sentiment (Greed/Fear)
- Execution price
- Trade size
- Fee
- Starting position

### Results:
- Accuracy: ~59%
- Strong at predicting unprofitable trades
- Weak at detecting profitable ones (due to class imbalance)
- Most important factors: **Sentiment score** and **Fee**

---

##  Strategy Recommendations
- Limit trading frequency during Greed to avoid emotional overtrading
- Use tighter stop-losses in Greed to reduce large losses
- Stay selective and cautious in Fear — data shows this leads to better outcomes
- Future models can include volatility, trader history, and time-series patterns

---

## Project Files
- `Trader_Sentiment_Analysis.ipynb`: Complete notebook with EDA, modeling, and insights
- `README.md`: Summary of the project




