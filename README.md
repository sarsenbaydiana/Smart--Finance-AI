# Smart Finance AI Assistant

AI-powered Telegram bot for personal finance tracking and analysis.

---

## Project Overview

Smart Finance AI Assistant is a Telegram-based chatbot designed to assist users in managing personal finances through natural language input.

The system interprets informal user messages and converts them into structured financial records without requiring strict input formats.

---

## Key Features

- Income tracking  
- Expense tracking  
- Balance calculation  
- Percentage-based calculations  
- Financial advice generation  
- Multi-command message processing  
- Natural language understanding  

---

## Example Inputs

```text
my income is 50000
I spent 10000 rent
show balance
show table
50% of 50000
advice
I earned 50000 and spent 10000 and show balance
```
---

## Technologies Used
- Python — core programming language
- Telegram Bot API — chatbot integration
- JSON — lightweight data storage system
- Regular Expressions (Regex) — text pattern recognition
- Google Colab — development environment
- GitHub — version control and project hosting

---

## Installation and Setup

The project is implemented as a Telegram-based bot executed in Google Colab.

# 1. Install dependencies
```
!pip install pyTelegramBotAPI
```

---

# 2. Data storage system

A JSON-based local storage system is used for saving user financial data.
```
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

---

# 3. Telegram Bot Token configuration

The bot requires a valid Telegram Bot API token:
```
TOKEN = "YOUR_TELEGRAM_BOT_TOKEN"
```
The token must be obtained from BotFather.

---

# 4. Running the system

All notebook cells must be executed sequentially in Google Colab:

Library installation
Data storage initialization
Bot logic execution

Upon successful execution, the system enters an active state.

