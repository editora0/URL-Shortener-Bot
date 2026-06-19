<div align="center">
  <h1>ربات کوتاه‌کننده لینک </h1>
  <p><strong>یک ربات قدرتمند تلگرام برای کوتاه‌سازی لینک‌ها با پنل مدیریت کامل</strong></p>
  
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

<a id="persian"></a>
## فارسی

### ویژگی‌ها

| آیکون | ویژگی | توضیحات |
|-------|-------|----------|
| 🔗 | کوتاه‌سازی لینک | کوتاه‌سازی لینک‌ها با استفاده از API TinyURL |
| 👑 | پنل مدیریت | دستورات کامل مدیریتی |
| 📢 | جوین اجباری | الزام کاربران به عضویت در کانال |
| ⏱️ | محدودیت نرخ | جلوگیری از اسپم با محدودیت‌های هوشمند |
| 💬 | سیستم پشتیبانی | ارسال پیام کاربران به ادمین |
| 📨 | پیام همگانی | ارسال پیام به همه کاربران |
| 🚫 | مدیریت کاربران | مسدودسازی و لغو مسدودیت آسان کاربران |
| 💾 | دیتابیس SQLite | ذخیره‌سازی سبک و سریع |

---

### نسخه‌ها

| نسخه | زبان | مناسب برای | روش دریافت آپدیت |
|------|------|------------|------------------|
| PHP | PHP 7.0+ | هاست اشتراکی | Webhook |
| Python | Python 3.7+ | VPS/سرور اختصاصی | Polling |

---

### پیش‌نیازها

#### نسخه PHP
- PHP 7.0 یا بالاتر
- افزونه SQLite3
- دسترسی به API تلگرام

#### نسخه Python
- Python 3.7 یا بالاتر
- کتابخانه‌های مورد نیاز:
  - python-telegram-bot
  - requests

---

### نصب و راه‌اندازی

#### نسخه PHP

1. فایل `bot.php` را روی هاست خود آپلود کنید.

2. توکن ربات و آیدی ادمین را تنظیم کنید:
```php
define('BOT_TOKEN', 'توکن_ربات_خود_را_وارد_کنید');
define('ADMIN_ID', 123456789);
