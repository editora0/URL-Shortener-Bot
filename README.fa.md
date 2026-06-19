<div align="center">
  <h1>🤖 ربات کوتاه‌کننده لینک تلگرام</h1>
  <p><strong>یک ربات قدرتمند تلگرام برای کوتاه‌سازی لینک‌ها با پنل مدیریت کامل</strong></p>
  
  <p>
    <img src="https://img.shields.io/badge/PHP-7.0%2B-blue.svg" alt="PHP Version">
    <img src="https://img.shields.io/badge/Python-3.7%2B-green.svg" alt="Python Version">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License">
    <img src="https://img.shields.io/badge/Telegram-Bot-0088cc.svg" alt="Telegram Bot">
  </p>
</div>

---

## ✨ ویژگی‌ها

<table dir="rtl">
  <tr>
    <td>🔗 <b>کوتاه‌سازی لینک</b></td>
    <td>کوتاه‌سازی لینک‌ها با استفاده از API TinyURL</td>
  </tr>
  <tr>
    <td>👑 <b>پنل مدیریت</b></td>
    <td>دستورات کامل مدیریتی</td>
  </tr>
  <tr>
    <td>📢 <b>جوین اجباری</b></td>
    <td>الزام کاربران به عضویت در کانال</td>
  </tr>
  <tr>
    <td>⏱️ <b>محدودیت نرخ</b></td>
    <td>جلوگیری از اسپم با محدودیت‌های هوشمند</td>
  </tr>
  <tr>
    <td>💬 <b>سیستم پشتیبانی</b></td>
    <td>ارسال پیام کاربران به ادمین</td>
  </tr>
  <tr>
    <td>📨 <b>پیام همگانی</b></td>
    <td>ارسال پیام به همه کاربران</td>
  </tr>
  <tr>
    <td>🚫 <b>مدیریت کاربران</b></td>
    <td>مسدودسازی و لغو مسدودیت آسان کاربران</td>
  </tr>
  <tr>
    <td>💾 <b>دیتابیس SQLite</b></td>
    <td>ذخیره‌سازی سبک و سریع</td>
  </tr>
</table>

---

## 🚀 نسخه‌ها

| نسخه | زبان | مناسب برای | روش دریافت آپدیت |
|------|------|------------|------------------|
| **PHP** | PHP 7.0+ | هاست اشتراکی | Webhook |
| **Python** | Python 3.7+ | VPS/سرور اختصاصی | Polling |

---

## 📋 پیش‌نیازها

### نسخه PHP
- PHP 7.0 یا بالاتر
- افزونه SQLite3
- دسترسی به API تلگرام

### نسخه Python
- Python 3.7 یا بالاتر
- کتابخانه‌های مورد نیاز:
  - `python-telegram-bot`
  - `requests`

---

## 🔧 نصب و راه‌اندازی

### 🐘 نسخه PHP

1. فایل `bot.php` را روی هاست خود آپلود کنید.

2. توکن ربات و آیدی ادمین را تنظیم کنید:
```php
define('BOT_TOKEN', 'توکن_ربات_خود_را_وارد_کنید');
define('ADMIN_ID', 123456789);
