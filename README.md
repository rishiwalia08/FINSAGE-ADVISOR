
# 📊 FinSage: AI-Powered Multi-Strategy Stock Advisor

FinSage is a smart, AI-powered financial advisory platform that combines live stock market fundamentals, technical indicators, NLP-based sentiment analysis, and machine learning models to deliver comprehensive and actionable stock recommendations.

Whether you're a retail investor, a finance student, or an algorithmic trader, FinSage provides intelligent **Buy/Sell/Hold signals**, along with target prices, stop-loss suggestions, and confidence scores — all wrapped in a clean, interactive web interface built using **Streamlit**.

## 🧠 Key Highlights

- 🔍 Real-time fundamental data (Market Cap, PE Ratio, Sector, etc.)
- 📈 Technical strategy signals (RSI, MACD, SMA, Bollinger Bands)
- 📰 News sentiment analysis using NLP (VADER/TextBlob/FinBERT)
- 🤖 Machine Learning-based movement prediction (RandomForest/XGBoost/LSTM)
- 📌 Final recommendation combining all signals
- 📊 Interactive visualizations (charts, indicators, sentiment trends)
- 🖥️ Streamlit-based web interface for fast deployment and use

---

## 📂 Project Structure

finsage_project/
│
├── app.py # Main Streamlit App
├── utils.py # Stock data + fundamentals
├── strategies.py # Technical indicator functions
├── sentiment.py # News sentiment analysis
├── prediction.py # ML model prediction logic
├── models/ # Trained models (.pkl, .h5, etc.)
├── data/ # Sample datasets or downloaded data
└── README.md # This file


## 🔧 Technologies Used

| Area        | Tools / Libraries                                      |
|-------------|--------------------------------------------------------|
| Data        | yfinance, Alpha Vantage, pandas, NumPy                |
| NLP         | VADER, TextBlob, FinBERT, nltk                        |
| ML / DL     | scikit-learn, XGBoost, LSTM (TensorFlow/Keras)        |
| Web App     | Streamlit                                             |
| Charts      | matplotlib, seaborn, Plotly                           |
| Deployment  | Streamlit Cloud, Render, Docker (optional)            |

---

## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/finsage-advisor.git
cd finsage-advisor


### Installation 


pip install streamlit yfinance pandas numpy matplotlib seaborn scikit-learn nltk vaderSentiment textblob transformers torch plotly

### Running of Stramlit

streamlit run app.py


###📈 Features in Detail

###✅ Fundamentals Overview

Uses yfinance to fetch:
Current price
Market Cap
PE Ratio
52 Week High/Low
PB Ratio
Sector, Exchange, Currency

###✅ Technical Indicators

Implemented indicators:
RSI (Relative Strength Index)
MACD (Moving Average Convergence Divergence)
SMA/EMA (Simple/Exponential Moving Averages)
Bollinger Bands
Crossovers (Golden Cross, Death Cross)

###✅ Sentiment Analysis

You can fetch real-time or cached headlines and perform sentiment scoring using:
VADER (for rule-based sentiment)
TextBlob (simple polarity)
FinBERT (finance-specific BERT model)
Output includes:
Average compound sentiment score
Word cloud of positive/negative terms
Headline sentiment breakdown


###✅ Machine Learning Prediction

You can build or load models trained on:
Price history
Technical indicator features
Sentiment scores
Models supported:
Logistic Regression, Random Forest, XGBoost
LSTM (deep learning)
Output includes:
Predicted direction: "Up"/"Down"
Confidence probability (e.g., 87%)

###✅ Final Recommendation Engine

Based on:
Combined signal from strategy + ML + sentiment
If majority agrees, outputs:

✅ Final Call: BUY/SELL/HOLD
🎯 Target Price
🛑 Stop Loss
🔒 Confidence Score

###🧱 Planned Future Features

Here’s how FinSage can evolve into a full financial tech product:

###🔮 Short-Term Plans

Add stock screener for multiple tickers
Save past analyses and compare across time
Improve ML model training pipeline
Add candlestick chart visualizations

### 🧠 Mid-Term Plans

Backtesting engine for strategy validation
Add more sentiment sources (Reddit, Twitter, news sites)
Enable email alerts or Telegram bot integration
Integrate with broker APIs (like Zerodha, Alpaca)

###🏢 Long-Term Enterprise Vision

SaaS dashboard for multiple users (admin panel, logins)
Portfolio analysis and allocation suggestions
Risk management tools
Real-time alerts on technical/sentiment shifts
B2B version with API access for financial firms

###👤 Author
Rishi Walia
AI & ML Student, VIT
Finance + Tech Enthusiast | Quant + Algo Trading Learner
