# AI-Powered Business Analytics Dashboard

## Overview
This project demonstrates the use of **AI and machine learning** techniques to analyze financial data and predict stock market trends. By leveraging financial data and news sentiment, the AI-Powered Business Analytics Dashboard provides real-time insights and visualizations for decision-making in business analytics and investment strategies.

The dashboard uses various machine learning models, including **Sentiment Analysis**, **Classification**, and **Regression Models**, to predict stock market behavior, visualize trends, and evaluate performance.

## Features
- **Stock Market Data**: Real-time stock price data fetched from Yahoo Finance using the `yfinance` library.
- **Sentiment Analysis**: News articles and stock-related headlines are analyzed using VADER Sentiment Analysis to classify news sentiment.
- **Prediction Models**: AI models (Random Forest, XGBoost) for trend prediction, classification (bullish/bearish), and regression (stock price prediction).
- **Data Visualizations**: Interactive charts and graphs that display stock prices, sentiment trends, and model predictions.
- **Feature Importance**: Visual representation of the importance of features in machine learning models like Random Forest.

## Technologies Used
- **Python 3.12.6**
- **Libraries**: 
  - `yfinance`: For fetching real-time stock market data.
  - `vaderSentiment`: For performing sentiment analysis on news and headlines.
  - `scikit-learn`: For implementing machine learning models (Random Forest, Logistic Regression, etc.).
  - `matplotlib`, `seaborn`: For creating visualizations like feature importance, confusion matrix, and ROC curves.
  - `pandas`, `numpy`: For data manipulation and preprocessing.
  - `xgboost`: For enhanced machine learning models.

## Installation Instructions

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/ai-business-analytics-dashboard.git
    ```

2. Navigate to the project folder:

    ```bash
    cd marketmaven
    ```

3. Create and activate a virtual environment (optional but recommended):

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use venv\Scripts\activate
    ```

4. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Fetch Stock Data
You can use the `yfinance` library to fetch historical stock data. Below is an example of how to fetch data for a specific stock (e.g., **Apple Inc.**):

```python
import yfinance as yf

# Fetch data for Apple Inc. (AAPL)
df = yf.download('AAPL', start='2010-01-01', end='2023-01-01')
print(df.head())
