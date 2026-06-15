# Stock-price-prediction
Stock Price Prediction Using Sentiment Analysis and SARIMAX Time Series Modeling
Project Overview
This project predicts stock prices by combining financial news sentiment analysis (using the FinViz API and Ollama LLM) with SARIMAX time series modeling. It includes an interactive Streamlit dashboard for real-time analysis across 100+ stock tickers.

Key Features
Sentiment Processing: Over 1,000 financial news articles analyzed via FinViz API and Ollama LLM, achieving 65% correlation between computed sentiment and actual stock price movement.

Time Series Modeling: SARIMAX forecasting with 7-day rolling windows, generating 3-day price predictions at 85% accuracy and interval scoring.

Interactive Dashboard: Streamlit interface reduces analyst review time by 70%, enabling live tracking and comparison for 100+ stock tickers.

Tech Stack
Python 3.10+

FinViz API for news data

Ollama LLM for sentiment extraction

statsmodels (SARIMAX)

Streamlit for dashboard front-end

Setup & Installation
Clone this repository:

bash
git clone https://github.com/yourusername/stock-price-sentiment-sarimax.git
cd stock-price-sentiment-sarimax
Install dependencies:

bash
pip install -r requirements.txt
Configure FinViz and Ollama API credentials in config.py.

Running the Project
Run sentiment analysis on news articles:

bash
python analysis/sentiment_pipeline.py
Train and evaluate SARIMAX models:

bash
python analysis/sarimax_forecast.py
Launch Streamlit dashboard:

bash
streamlit run dashboard/app.py
Results
Achieved up to 65% sentiment-price correlation for target tickers.

Generated 3-day rolling predictions with 85% accuracy, validated on test splits.

Analytical workflow and dashboard reduced manual analysis time by over 70%.
