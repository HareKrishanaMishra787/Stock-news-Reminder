## 📈 Stock Price Alert System
An automated Python application that monitors stock price movements and sends SMS notifications with relevant news articles when significant changes occur.
## 🌟 Features

Stock Price Monitoring: Tracks daily closing prices of specified stocks
Percentage Change Calculation: Calculates day-to-day price movements
Threshold Alerts: Triggers notifications when price changes exceed defined thresholds
Automated News Collection: Fetches recent news articles related to the company
SMS Notifications: Delivers alerts with stock movement data and relevant news via SMS

## 🛠️ Technology Stack

Python 3.6+
Alpha Vantage API (stock market data)
News API (company news articles)
Twilio API (SMS messaging)

API Keys and Credentials
The application requires the following API keys and credentials:

STOCK_API_KEY: Your Alpha Vantage API key
NEWS_API_KEY: Your News API key
TWILIO_SID: Your Twilio account SID
TWILIO_AUTH_TOKEN: Your Twilio authentication token

## 🔍 How It Works

Stock Price Monitoring:

Fetches the closing stock prices for yesterday and the day before
Calculates the percentage difference between these prices


Alert System:

If the percentage change exceeds the threshold (default 2%) 

Fetches the 3 most recent news articles about the company
Formats the data with appropriate rise/fall indicators (🔺/🔻)


Notification Delivery:
<br>
<img src="https://github.com/user-attachments/assets/26fa0a58-197c-4661-8e2e-c8251d44679d" height="400" width="200" />


Sends individual SMS messages for each news article
Each message includes the stock symbol, percentage change, headline, and brief description
