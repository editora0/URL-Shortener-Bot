<div align="center">
  <h1>🤖 URL Shortener Bot</h1>
  <p><strong>A Powerful Telegram Bot for Shortening URLs with Full Admin Panel</strong></p>
  
  <p>
    <a href="#english-section"><strong>English</strong></a> •
    <a href="#persian-section"><strong>فارسی</strong></a>
  </p>
  
  <p>
    <img src="https://img.shields.io/badge/PHP-7.0%2B-blue.svg" alt="PHP Version">
    <img src="https://img.shields.io/badge/Python-3.7%2B-green.svg" alt="Python Version">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License">
    <img src="https://img.shields.io/badge/Telegram-Bot-0088cc.svg" alt="Telegram Bot">
  </p>
</div>

---

<div id="english-section"></div>

## English

### Features

| Icon | Feature | Description |
|------|---------|-------------|
| 🔗 | URL Shortener | Shorten URLs using TinyURL API |
| 👑 | Admin Panel | Complete management commands |
| 📢 | Force Join | Require users to join a channel |
| ⏱️ | Rate Limiting | Prevent spam with smart limits |
| 💬 | Support System | Users can send messages to admin |
| 📨 | Broadcast | Send messages to all users |
| 🚫 | User Management | Ban/Unban users easily |
| 💾 | SQLite Database | Lightweight and fast storage |

---

### Versions

| Version | Language | Best For | Method |
|---------|----------|----------|--------|
| PHP | PHP 7.0+ | Shared Hosting | Webhook |
| Python | Python 3.7+ | VPS/Dedicated Server | Polling |

---

### Requirements

#### PHP Version
- PHP 7.0 or higher
- SQLite3 extension
- Telegram API access

#### Python Version
- Python 3.7 or higher
- Required libraries:
  - python-telegram-bot
  - requests

---

### Installation

#### PHP Version

1. Upload `bot.php` to your hosting

2. Configure bot token and admin ID:
```php
define('BOT_TOKEN', 'YOUR_BOT_TOKEN');
define('ADMIN_ID', 123456789);
```

3. Set up webhook:
   · Edit webhook URL in the setWebhook() function
   · Or visit this URL in your browser:
   ```
   https://api.telegram.org/bot[TOKEN]/setWebhook?url=https://your-domain.com/bot.php
   ```
4. Ensure the directory has write permissions (for SQLite database)

Python Version

1. Clone the repository:

```bash
git clone https://github.com/your-username/telegram-url-shortener-bot.git
cd telegram-url-shortener-bot
```

2. Install dependencies:

```bash
pip install python-telegram-bot requests
```

3. Configure bot token and admin ID in bot.py:

```python
TOKEN = "YOUR_BOT_TOKEN"
ADMIN_ID = 123456789
```

4. Run the bot:

```bash
python bot.py
```

---

Commands

User Commands

Command Description
/start Welcome message and start using the bot
/help Get help and usage instructions
/support [message] Send a message to support

Admin Commands

Command Description
/admin Show admin panel
/set_force_join [@channel] Enable force join for a channel
/remove_force_join Disable force join
/set_start [text] Change start message
/set_help [text] Change help message
/ban [user_id] Ban a user
/unban [user_id] Unban a user
/broadcast [message] Send message to all users
/send [user_id] [message] Send message to specific user

---

Database Structure

Users Table

Field Type Description
user_id INTEGER PRIMARY KEY User ID
blocked INTEGER DEFAULT 0 Block status
last_message_time REAL Last message timestamp
message_count INTEGER DEFAULT 0 Messages in time window
block_until REAL DEFAULT 0 Block expiration time

Settings Table

Field Type Description
key TEXT PRIMARY KEY Setting key
value TEXT Setting value

Messages Table

Field Type Description
user_id INTEGER User ID
message TEXT Message content
timestamp REAL Message timestamp

---

Rate Limiting Rules

· Maximum: 3 messages per 30 seconds
· Auto-block: 5 minutes if limit exceeded
· Block message: Shows remaining time

---

Troubleshooting

Bot doesn't respond

· Check webhook configuration (PHP version)
· Verify bot is running (Python version)
· Check server logs

URLs not shortening

· TinyURL service might be temporarily unavailable
· Ensure URL is valid (starts with http:// or https://)

---

Contributing

1. Fork the repository
2. Create your feature branch (git checkout -b feature/amazing-feature)
3. Commit your changes (git commit -m 'Add some amazing feature')
4. Push to the branch (git push origin feature/amazing-feature)
5. Open a Pull Request

---

License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Contact

Developer: editor_a0
Telegram: @editor_a0_ADM
Channel: @editor_a0

---

<div align="center">
  <sub>Built with ❤️ for the Telegram community</sub>
</div>

---

<div align="center">
  <a href="#top">⬆ Back to Top</a>
</div>
