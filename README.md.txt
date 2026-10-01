# Telegram Confession System

An open-source, anonymous confession management platform powered by Telegram bots, moderation channels, and SQLite persistence.

## Features
- **Anonymous Submissions**: Submissions are routed to an admin group with zero identifying markers.
- **Admin Inline Moderation**: Approve or Reject confessions with a single click.
- **Auto-Incrementing Sequence**: Posts are cleanly numbered (`#Confession_1`, `#Confession_2`, ...) using SQLite.
- **Spam Cooldown**: Built-in per-user cooldown timers.

## Installation

1. Clone repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/telegram-confession-bot.git
   cd telegram-confession-bot
   ```

2. Create virtual environment and install packages:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Setup environment variables:
   - Copy `.env.example` to `.env`
   - Fill in `BOT_TOKEN`, `ADMIN_CHAT_ID`, and `CHANNEL_ID`.

4. Run the bot:
   ```bash
   python bot.py
   ```