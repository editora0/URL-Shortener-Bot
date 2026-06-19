<div align="center">
  <h1>🤖 Telegram URL Shortener Bot</h1>
  <p><strong>A Powerful Telegram Bot for Shortening URLs with Full Admin Panel</strong></p>
  
  <p>
    <img src="https://img.shields.io/badge/PHP-7.0%2B-blue.svg" alt="PHP Version">
    <img src="https://img.shields.io/badge/Python-3.7%2B-green.svg" alt="Python Version">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License">
    <img src="https://img.shields.io/badge/Telegram-Bot-0088cc.svg" alt="Telegram Bot">
  </p>
</div>

---

## ✨ Features

<table>
  <tr>
    <td>🔗 <b>URL Shortener</b></td>
    <td>Shorten URLs using TinyURL API</td>
  </tr>
  <tr>
    <td>👑 <b>Admin Panel</b></td>
    <td>Complete management commands</td>
  </tr>
  <tr>
    <td>📢 <b>Force Join</b></td>
    <td>Require users to join a channel</td>
  </tr>
  <tr>
    <td>⏱️ <b>Rate Limiting</b></td>
    <td>Prevent spam with smart limits</td>
  </tr>
  <tr>
    <td>💬 <b>Support System</b></td>
    <td>Users can send messages to admin</td>
  </tr>
  <tr>
    <td>📨 <b>Broadcast</b></td>
    <td>Send messages to all users</td>
  </tr>
  <tr>
    <td>🚫 <b>User Management</b></td>
    <td>Ban/Unban users easily</td>
  </tr>
  <tr>
    <td>💾 <b>SQLite Database</b></td>
    <td>Lightweight and fast storage</td>
  </tr>
</table>

---

## 🚀 Versions

| Version | Language | Best For | Method |
|---------|----------|----------|--------|
| **PHP** | PHP 7.0+ | Shared Hosting | Webhook |
| **Python** | Python 3.7+ | VPS/Dedicated Server | Polling |

---

## 📋 Requirements

### PHP Version
- PHP 7.0 or higher
- SQLite3 extension
- Telegram API access

### Python Version
- Python 3.7 or higher
- Required libraries:
  - `python-telegram-bot`
  - `requests`

---

## 🔧 Installation

### 🐘 PHP Version

1. Upload `bot.php` to your hosting

2. Configure bot token and admin ID:
```php
define('BOT_TOKEN', 'YOUR_BOT_TOKEN');
define('ADMIN_ID', 123456789);
