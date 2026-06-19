<div align="center">
  <h1>URL Shortener Bot</h1>
  <p><strong>A Powerful Telegram Bot for Shortening URLs with Full Admin Panel</strong></p>
  
  <p>
    <a href="#english"><strong>English</strong></a> •
    <a href="#persian"><strong>فارسی</strong></a>
  </p>
  
  <p>
    <img src="https://img.shields.io/badge/PHP-7.0%2B-blue.svg" alt="PHP Version">
    <img src="https://img.shields.io/badge/Python-3.7%2B-green.svg" alt="Python Version">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License">
    <img src="https://img.shields.io/badge/Telegram-Bot-0088cc.svg" alt="Telegram Bot">
  </p>
</div>

---

<a id="english"></a>
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
