# 💎 Smart Finance AI Assistant

AI-powered Telegram bot for personal finance tracking and analysis.

---

## 🚀 Project Overview

Smart Finance AI Assistant is a Telegram-based chatbot that helps users manage personal finances using natural language input.

Instead of strict formats, users can write messages naturally, and the bot understands them.

---

## ✨ Key Features

- 💰 Income tracking
- 💸 Expense tracking
- 📊 Balance calculation
- 🧮 Percentage calculator
- 🧠 AI-style financial advice
- 🔥 Multi-command message processing
- 💬 Natural language understanding

---

## 💬 Example Inputs

Users can interact naturally:

```text
my income is 50000
I spent 10000 rent
show balance
show table
```
## 🛠 Technologies Used

- 🐍 Python — core programming language  
- 🤖 Telegram Bot API — chatbot integration  
- 💾 JSON — lightweight data storage system  
- 🔍 Regex — natural language pattern recognition  
- 📓 Google Colab — development environment  
- 🧑‍💻 GitHub — version control and project hosting

## ⚙️ How to Run the Project

This project is a Telegram-based AI finance assistant running in Google Colab.

---

### 1. Install dependencies

Run this first cell in Google Colab:

```python
!pip install pyTelegramBotAPI
```

## 💾 2. Set up data storage system

Your second cell creates a local JSON-based database system.

```python
import json
from datetime import datetime

DATA_FILE = "data.json"

def load_data():
    try:
        with open(DATA_FILE, "r") as f:
            return json.load(f)
    except:
        return {}

def save_data(data):
    with open(DATA_FILE, "w") as f:
        json.dump(data, f, indent=4)
```

## 📌 Purpose of this system

This storage system is used to save user financial data locally:

💰 Income records  
💸 Expense records  
📊 Full financial history per user


## 3. Add Telegram Bot Token

In your main code cell:

```python
TOKEN = "YOUR_TELEGRAM_BOT_TOKEN"
```
Replace `YOUR_TELEGRAM_BOT_TOKEN` with your real token from BotFather.

### 4. Run the bot

In Google Colab:

Run ALL cells in order:

- Install libraries  
- Data storage functions  
- Main bot code  

After running all cells, the bot will start automatically and will show:

```text
💎 SMART FINANCE AI IS RUNNING...
```


## 💬 5. How to Use the Bot

After running the project, open Telegram and start chatting with your bot.

You can write natural language messages like:

```text
my income is 50000
I spent 10000 rent
show balance
show table
50% of 50000
advice
I earned 50000 and spent 10000 and show balance
```

## 🤖 Bot Behavior

The bot will automatically:

- 💰 detect income and expenses  
- 📊 calculate balance  
- 🧠 analyze spending patterns  
- 🧠 give AI-style financial advice  
- 🔥 handle multiple commands in one message  

---

## ⚠️ Important Notes

- Keep Google Colab session running while using the bot  
- If Colab stops, the bot will go offline  
- Data is stored temporarily in `data.json`  

## 📊 System Logic

The bot processes natural language inputs and converts them into structured financial records:

- Detects income and expenses using keyword recognition  
- Extracts numeric values using regex  
- Stores data in JSON format  
- Performs real-time calculations and summaries  

---

## 🧠 AI Concept

Although no external AI API is used, the bot simulates AI behavior using:

- Natural language parsing  
- Multi-command interpretation  
- Context-aware responses  
- Rule-based decision logic  

---

## 📌 Future Improvements

- Integration with real AI models (e.g., OpenAI API)  
- Data visualization (charts and graphs)  
- User authentication system  
- Mobile application version

## 📄 Project Summary

This project was developed as part of an Introduction to Programming course to demonstrate practical application of:

- Python programming  
- Data handling  
- Natural language processing concepts  
- Real-world problem solving  

---

## 👩‍💻 Author

Diana Sarsenbay
