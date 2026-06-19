<div align="center">
  <h1>🤖 ربات کوتاه‌کننده لینک</h1>
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
```

3. Webhook را تنظیم کنید:
   · آدرس Webhook را در تابع setWebhook() ویرایش کنید
   · یا از طریق مرورگر به آدرس زیر بروید:
   ```
   https://api.telegram.org/bot[TOKEN]/setWebhook?url=https://your-domain.com/bot.php
   ```
4. اطمینان حاصل کنید که پوشه دارای مجوز نوشتن است (برای دیتابیس SQLite)

نسخه Python

1. مخزن را کلون کنید:

```bash
git clone https://github.com/your-username/telegram-url-shortener-bot.git
cd telegram-url-shortener-bot
```

2. کتابخانه‌های مورد نیاز را نصب کنید:

```bash
pip install python-telegram-bot requests
```

3. توکن ربات و آیدی ادمین را در bot.py تنظیم کنید:

```python
TOKEN = "توکن_ربات_خود_را_وارد_کنید"
ADMIN_ID = 123456789
```

4. ربات را اجرا کنید:

```bash
python bot.py
```

---

دستورات

دستورات کاربران

دستور توضیحات
/start پیام خوش‌آمدگویی و شروع کار با ربات
/help دریافت راهنما و نحوه استفاده
/support [متن] ارسال پیام به پشتیبانی

دستورات مدیریت (فقط ادمین)

دستور توضیحات
/admin نمایش پنل مدیریت
/set_force_join [@کانال] فعال‌سازی جوین اجباری کانال
/remove_force_join غیرفعال‌سازی جوین اجباری
/set_start [متن] تغییر متن پیام استارت
/set_help [متن] تغییر متن پیام راهنما
/ban [آیدی] مسدود کردن کاربر
/unban [آیدی] لغو مسدودیت کاربر
/broadcast [متن] ارسال پیام همگانی به همه کاربران
/send [آیدی] [متن] ارسال پیام به کاربر خاص

---

ساختار دیتابیس

جدول کاربران

فیلد نوع توضیحات
user_id INTEGER PRIMARY KEY آیدی کاربر
blocked INTEGER DEFAULT 0 وضعیت مسدودیت
last_message_time REAL زمان آخرین پیام
message_count INTEGER DEFAULT 0 تعداد پیام‌ها در بازه زمانی
block_until REAL DEFAULT 0 زمان پایان مسدودیت

جدول تنظیمات

فیلد نوع توضیحات
key TEXT PRIMARY KEY کلید تنظیمات
value TEXT مقدار تنظیمات

جدول پیام‌ها

فیلد نوع توضیحات
user_id INTEGER آیدی کاربر
message TEXT متن پیام
timestamp REAL زمان ارسال

---

قوانین محدودیت نرخ

· حداکثر: ۳ پیام در هر ۳۰ ثانیه
· مسدودیت خودکار: ۵ دقیقه در صورت تجاوز از حد مجاز
· پیام مسدودیت: نمایش زمان باقی‌مانده

---

عیب‌یابی

ربات پاسخ نمی‌دهد

· تنظیمات Webhook را بررسی کنید (نسخه PHP)
· از اجرا بودن ربات اطمینان حاصل کنید (نسخه Python)
· لاگ‌های سرور را بررسی کنید

لینک کوتاه نمی‌شود

· سرویس TinyURL ممکن است موقتاً در دسترس نباشد
· مطمئن شوید لینک معتبر است (با http:// یا https:// شروع شود)

---

مشارکت

1. مخزن را Fork کنید
2. Branch جدید ایجاد کنید (git checkout -b feature/amazing-feature)
3. تغییرات را Commit کنید (git commit -m 'Add some amazing feature')
4. Push کنید (git push origin feature/amazing-feature)
5. Pull Request ارسال کنید

---

لایسنس

این پروژه تحت لایسنس MIT منتشر شده است - برای اطلاعات بیشتر فایل LICENSE را مشاهده کنید.

---

تماس با ما

توسعه‌دهنده: editor_a0
تلگرام: @editor_a0_ADM
کانال: @editor_a0

---

<div align="center">
  <sub>ساخته شده با ❤️ برای جامعه تلگرام</sub>
</div>

---

<div align="center">
  <a href="#top">⬆ بازگشت به بالا</a>
</div>
