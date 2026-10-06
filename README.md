# 📊 Stock Market Prediction & AI Insights Dashboard

**Stock market analysis and machine learning prediction project combining Python, Scikit-learn, and Power BI.**

## 🧩 Project Overview

This project analyzes historical stock trends and builds classification models for five major technology companies:

* **AAPL** — Apple
* **AMZN** — Amazon
* **GOOGL** — Alphabet
* **MSFT** — Microsoft
* **TSLA** — Tesla

Python is used for data preparation, feature engineering, machine learning, and model evaluation, while Power BI is used to transform the results into interactive business dashboards.

The project demonstrates an end-to-end workflow from **data collection and machine learning to business intelligence and visual reporting**.

---

## 🛠️ Technologies

* Python
* Pandas
* Scikit-learn
* Google Colab
* Power BI
* DAX

---

# 🐍 Python Analysis

### Goal

Build predictive models and extract performance metrics for the selected technology stocks.

## 1. Data Collection

Historical stock data was collected for:

```text
AAPL | AMZN | GOOGL | MSFT | TSLA
```

Additional features were calculated, including:

* `daily_return`
* `volatility_20` — 20-day rolling standard deviation

---

## 2. Feature Engineering

The dataset was prepared for machine learning by:

* Creating lag features based on previous returns
* Generating classification labels
* Classifying future movement as **"Up"** or **"Down"**

---

## 3. Model Training & Evaluation

A **Random Forest Classifier** from Scikit-learn was used to predict stock direction.

Model performance was evaluated using:

* Accuracy
* Confusion matrix
* True Positives (TP)
* False Positives (FP)
* True Negatives (TN)
* False Negatives (FN)

### Model Results

| Symbol |   Accuracy |  TP | FP |  TN |  FN |
| ------ | ---------: | --: | -: | --: | --: |
| AAPL   |     44.76% |  16 |  5 | 155 | 206 |
| AMZN   |     47.91% |  13 | 13 | 170 | 186 |
| GOOGL  | **55.24%** | 141 | 97 |  70 |  74 |
| MSFT   |     43.46% |  27 | 29 | 139 | 187 |
| TSLA   |     52.88% |  91 | 73 | 111 | 107 |

**GOOGL recorded the highest accuracy at 55.24%**, while MSFT recorded the lowest at 43.46%.

---

# 📁 Output Files

The analysis produces files used to build the Power BI dashboard:

### `stock_predictions.csv`

Cleaned stock data containing the features and prediction-related results required for visualization.

### `AI_Metrics`

A DAX table containing the machine learning evaluation metrics used for the AI Insights dashboard.

---

# 📈 Power BI Dashboard

The Power BI report contains two main pages.

## 1️⃣ Market Overview

### Goal

Monitor stock performance, market movement, and volatility patterns across the selected companies.

### Visuals

* **Line Chart:** Daily returns over time by stock symbol
* **Area Chart:** 20-day volatility trends
* **Cards:** Average return, total volatility, and trading range
* **Slicers:** Stock symbol and date range

---

## 2️⃣ AI Insights

### Goal

Present the machine learning results in a format that is easy for both technical and non-technical users to understand.

### Visuals

* **Clustered Bar Chart:** Accuracy by stock symbol
* **Table:** TP, FP, TN, and FN by symbol
* **Cards:**

  * Best-performing model — GOOGL
  * Average accuracy across all models
* **Slicers:** Symbol and accuracy range

---

# 🔍 Key Insights

* **GOOGL achieved the highest predictive accuracy at 55.24%.**
* **MSFT recorded the lowest accuracy at 43.46%.**
* Model accuracy varied considerably across the five stocks.
* Accuracy tended to decrease during periods of higher volatility.
* The Power BI dashboard connects machine learning results with business intelligence, making model performance easier to interpret.

> **Note:** The results show that the Random Forest models have limited predictive accuracy for this dataset. The dashboard is therefore intended primarily as an analytical and demonstration project rather than a standalone trading system.

---

# 🔄 End-to-End Workflow

```text
Historical Stock Data
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Random Forest Classification
        ↓
Model Evaluation
        ↓
CSV / AI Metrics
        ↓
Power BI
        ↓
Interactive Dashboard
```

---

# 🚀 Future Enhancements

Several improvements could extend the project:

* Test **LSTM** models for time-series prediction.
* Evaluate **XGBoost** against the Random Forest baseline.
* Automate daily data refresh using Power BI Dataflows.
* Integrate financial-news sentiment analysis.
* Combine technical indicators with market sentiment.
* Expand the analysis to additional stocks and sectors.

---

# 🎯 Project Objective

The main objective of this project is to demonstrate how **data analytics, machine learning, and business intelligence can work together** to analyze financial market data and communicate model results effectively.

It combines the technical side of machine learning with the business-facing side of interactive dashboard development.

## 👨‍💻 Author

**Casmir Udeme**

Data Scientist/Analyst | AI/ML | Business Intelligence
