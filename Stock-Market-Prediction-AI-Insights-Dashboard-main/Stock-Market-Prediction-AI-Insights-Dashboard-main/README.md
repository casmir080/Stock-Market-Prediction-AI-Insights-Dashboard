📊 Stock Market Prediction & AI Insights Dashboard  
Technologies: Python • Pandas • Scikit-learn • Power BI  

🧩 Project Overview  
This project analyzes and predicts stock trends for five major tech companies — AAPL, AMZN, GOOGL, MSFT, and TSLA — using Python for machine learning and Power BI for visualization.  
It demonstrates a full end-to-end data analytics and AI workflow — from model training to business dashboard delivery.

Python Analysis (Google Colab)
Goal  
Build predictive models and extract key performance metrics for selected tech stocks.
Process
1. Data Collection
   - Fetched historical stock data (AAPL, AMZN, GOOGL, MSFT, TSLA).
   - Calculated `daily_return` and `volatility_20` (20-day rolling standard deviation).

2. Feature Engineering
   - Created lag features for past returns.
   - Labeled data for classification (“Up” or “Down”).

3. Model Training & Evaluation
   - Used `RandomForestClassifier` from Scikit-learn.
   - Computed confusion matrix and accuracy for each stock.

| Symbol | Accuracy | TP | FP | TN | FN |
|---------|-----------|----|----|----|----|
| AAPL | 0.4476 | 16 | 5 | 155 | 206 |
| AMZN | 0.4791 | 13 | 13 | 170 | 186 |
| GOOGL | 0.5524 | 141 | 97 | 70 | 74 |
| MSFT | 0.4346 | 27 | 29 | 139 | 187 |
| TSLA | 0.5288 | 91 | 73 | 111 | 107 |

4. Output Files
   - `stock_predictions.csv` — Cleaned dataset for Power BI.
   - `AI_Metrics` — DAX table for confusion matrix results.

## 📈 Power BI Dashboard  

The Power BI report contains two pages:

1️⃣ Market Overview  
Goal: Track market movement and volatility patterns.  

Visuals
- Line Chart: Daily returns over time by symbol.  
- Area Chart: 20-day volatility trend by date.  
- Cards: Average return, total volatility, and trading range.  
- Slicers: Symbol and Date Range filters.  

2️⃣ AI Insights  
Goal: Show machine learning performance and interpret model metrics visually.  

Visuals
- Clustered Bar Chart: Accuracy by Symbol.  
- Table: TP, FP, TN, FN for each symbol.  
- Cards:
  - Best-performing model (GOOGL)  
  - Average accuracy across all models  
- Slicers: Symbol, Accuracy Range
 Key Insights  
- GOOGL achieved the highest predictive accuracy (55.24%).  
- Accuracy tends to drop during periods of high volatility.  
- The AI Insights dashboard bridges **machine learning and business intelligence, allowing both technical and non-technical users to interpret results clearly.

 Future Enhancements  
- Introduce LSTM or XGBoost for improved prediction accuracy.  
- Automate daily data refresh using Power BI dataflows.  
- Integrate sentiment analysis from financial news for deeper insights.

👤 Author  
Imeobong Monday
Senior Data Analyst | SQL • Python • Power BI  
📧 (mondayimeobong@gmail.com)  
🌐 [github.com/ImeMonday](https://github.com/ImeMonday)

---
