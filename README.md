# 📈 Stock Alert System 🚨

A Python-based alerting system that monitors **any company's stock** and sends real-time SMS alerts with relevant news when significant price fluctuations occur.

---

## 🧠 Features

- ✅ Monitors **any stock** using [Alpha Vantage](https://www.alphavantage.co/)
- ✅ Calculates daily price changes and percentage difference
- ✅ Gets the **top 3 relevant news articles** using [NewsAPI](https://newsapi.org/)
- ✅ Sends SMS alerts via [Twilio](https://www.twilio.com/) if the change exceeds a defined threshold

---

## ⚙️ Tech Stack

- **Python 3**
- `requests` – For API calls
- `twilio` – For sending SMS messages

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/stock-alert-system.git
cd stock-alert-system
```

### 2. Install Dependencies
```bash
pip install requests twilio
```

### 3. Configuration

Open `main.py` and update the following variables:

```python
STOCK_NAME = "TSLA"           # Ticker symbol of the stock
COMPANY_NAME = "Tesla Inc"    # Name of the company
STOCK_API_KEY = "your_alpha_vantage_api_key"
NEWS_API_KEY = "your_news_api_key"
TWILIO_SID = "your_twilio_sid"
TWILIO_AUTH_TOKEN = "your_twilio_auth_token"
TWILIO_PHONE_NUMBER = "+1234567890"
USER_PHONE_NUMBER = "+919999999999"
```

You can change `PRICE_CHANGE_THRESHOLD` to adjust sensitivity:
```python
PRICE_CHANGE_THRESHOLD = 2  # percent
```

### 4. Run the Script
```bash
python main.py
```

---

## 📱 Sample Alert

```
AAPL: 🔺2.56%
Headline: Apple beats expectations with strong iPhone sales.
Brief: Apple reported better-than-expected quarterly results, pushing shares higher.
```

---

## 📁 Project Structure

```
.
├── main.py           # Main script
├── README.md         # Project documentation
├── .gitignore        # Standard Git ignore file
```

---

## 🛡️ Disclaimer

This project is intended for educational and demo purposes only. Use responsibly. Never share your API keys publicly.

---

## ⭐ Show Some Love

If you found this project helpful, consider giving it a ⭐ on GitHub and sharing it with others!
