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

## 1. Install dependencies
```
!pip install pyTelegramBotAPI
```

---

## 2. Data storage system

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

## 3. Telegram Bot Token configuration

The bot requires a valid Telegram Bot API token:
```
TOKEN = "YOUR_TELEGRAM_BOT_TOKEN"
```
The token must be obtained from BotFather.

---

## 4. Running the system

All notebook cells must be executed sequentially in Google Colab:

Library installation
Data storage initialization
Bot logic execution

Upon successful execution, the system enters an active state.

---

# Usage

After activation, the bot operates through Telegram and processes natural language financial commands such as:

```
my income is 50000
I spent 10000 rent
show balance
show table
50% of 50000
advice
```

---

# System Behavior

The system automatically performs the following operations:

- Identification of income and expense statements
- Extraction of numerical values using pattern recognition
- Storage of structured financial data in JSON format
- Real-time calculation of balances and percentages
- Generation of rule-based financial recommendations
- Processing of multiple commands within a single input

---

# System Architecture

The system is based on a rule-based natural language processing approach. No external AI API is used. Instead, logic-based parsing and keyword detection simulate intelligent behavior.

Core mechanisms include:

- Text preprocessing
- Keyword classification
- Regular expression parsing
- Conditional logic for decision-making

---

# Future Improvements
- Integration with external AI models for enhanced natural language understanding
- Data visualization through charts and graphs
- User authentication system
- Persistent cloud database integration
- Mobile application extension

---

# Project Summary

The project demonstrates the application of Python programming, data processing techniques, and natural language processing principles in the development of a functional financial assistant system.

The system is designed to simulate intelligent behavior through structured logic and rule-based processing.

---

# Author

Diana Sarsenbay
