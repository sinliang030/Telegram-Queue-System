# 🤖 Telegram Queue Bot

A lightweight, asynchronous Telegram queue management bot built with Python and the [`python-telegram-bot`](https://github.com/python-telegram-bot/python-telegram-bot) library (v22+). Perfect for managing waiting lists, support queues, or event sign-ups directly inside Telegram chats.

---

## ✨ Features

* **User Management:** Users can easily join or leave the queue with a single command and track their live position.
* **Automatic Position Updates:** When someone leaves or is called, all remaining participants are automatically notified of their updated position in line.
* **Admin Controls:** Dedicated commands for administrators to call the next person in line or completely wipe/reset the queue.
* **Robust Logging:** Full console logging for tracking user actions, join timestamps, and admin calls.

---

## 📋 Commands Reference

### 👤 User Commands
| Command | Description |
| :--- | :--- |
| `/start` | Welcome message and introduction to the bot |
| `/join` | Add yourself to the end of the queue |
| `/leave` | Remove yourself from the queue |
| `/queue` | View the current live list of participants |
| `/help` | Display the list of available commands |

### 🛠️ Admin Commands
| Command | Description |
| :--- | :--- |
| `/next` | Call the next person, remove them from the queue, and notify everyone |
| `/clear` | Wipe the entire queue and notify all active participants |

---

## ⚙️ Installation & Setup

### 1. Prerequisites
Make sure you have **Python 3.10+** installed on your system.

### 2. Clone the Repository
```bash
git clone [https://github.com/sinliang030/Telegram-Queue-System.git](https://github.com/sinliang030/Telegram-Queue-System.git)
cd Telegram-Queue-System
3. Install Dependencies
Install the required version of python-telegram-bot:

Bash
pip install "python-telegram-bot>=22.0"
4. Configure the Bot
Open your script and update the configuration section at the top with your credentials:

Python
BOT_TOKEN = "YOUR_BOT_TOKEN_HERE"   # Get this from @BotFather on Telegram
ADMIN_IDS = {123456789}             # Replace with your Telegram user ID (as an integer) Get this from @Userinfokbot on Telegram
🚀 Running the Bot
Start your bot by running the Python script:

Bash
python queue_bot.py
You should see log output indicating that the bot has started polling for updates.

---
