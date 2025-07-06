# Dima CMS

[![GPL-3.0 License](https://img.shields.io/badge/license-GPL--3.0-green)](LICENSE)
[![PHP](https://img.shields.io/badge/PHP-%3E%3D7.4-blue)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-Supported-orange)](https://www.mysql.com/)

> **سیستم مدیریت محتوای پیشرفته، ماژولار و متن‌باز با معماری مدرن MVC**

---

## ✨ امکانات کلیدی
- مدیریت کاربران (ثبت‌نام، ورود، RBAC، پروفایل)
- صفحات و مطالب (استاتیک، پست، دسته‌بندی چندلایه)
- سیستم چندزبانه و سوییچ زبان
- پلاگین و قالب (سیستم فعال‌سازی، توسعه آسان، انتخاب قالب)
- فروشگاه اینترنتی (محصول، سبد خرید، سفارش، پرداخت زرین‌پال)
- فرم‌ساز داینامیک (ساخت فرم، فیلد سفارشی، مشاهده پاسخ‌ها)
- امنیت پیشرفته (CSRF, XSS, Rate Limiting, Captcha، فایروال)
- تنظیمات مرکزی (سایت و پلاگین)
- داشبورد حرفه‌ای (آمار، نمودار Chart.js، اطلاعیه بروزرسانی)
- سیستم نوتیفیکیشن و پیام داخلی
- انجمن (Forum) و پشتیبانی (تیکتینگ) به صورت پلاگین
- API RESTful با JWT برای موبایل و کلاینت‌ها
- ریسپانسیو و PWA (Bootstrap 5، manifest، service worker)
- مستندسازی کامل و توسعه‌پذیر

---

## 🛠️ تکنولوژی‌ها و کتابخانه‌های استفاده‌شده
- **PHP 7.4+** (OOP, MVC, PDO)
- **MySQL** (InnoDB, Relations)
- **Bootstrap 5** (CDN/Local, RTL)
- **Chart.js** (نمودارهای داشبورد)
- **JWT (JSON Web Token)** (احراز هویت API)
- **CSRF Token** (امنیت فرم)
- **Custom Firewall** (ضد حملات رایج)
- **Captcha** (فارسی/انگلیسی، مدیریت توسط ادمین)
- **PWA** (manifest.json, service-worker.js)
- **AI Content Providers** (OpenAI, DeepSeek, Qwen)
- **AJAX, Fetch API** (ارتباط پویا)
- **PHPUnit** (تست خودکار)
- **سازگاری با CDN و Local Asset Loading**

---

## 📁 ساختار پروژه
```
├── app/           # هسته MVC (مدل، کنترلر، ویو، هسته)
├── public/        # فایل‌های استاتیک، assets، service worker
├── themes/        # قالب‌های کاربری و مدیریتی
├── plugins/       # پلاگین‌های مستقل (forum, support, ...)
├── config/        # تنظیمات و کانفیگ
├── docs/          # مستندات و راهنما
├── tests/         # تست‌های خودکار (PHPUnit)
└── README.md      # این فایل
```

---

## 🚀 نصب سریع
1. کلون پروژه:
   ```bash
   git clone https://github.com/balvardi/dimacms.git
   ```
2. انتقال به روت وب‌سرور (MAMP/XAMPP)
3. ساخت دیتابیس و اجرای SQLهای docs
4. تنظیم `config/config.php`
5. تنظیم دسترسی پوشه‌های `uploads` و `logs`
6. لذت بردن از Dima CMS!

---

## 📚 مستندات و راهنما
- [راهنمای نصب](docs/install_guide.html)
- [راهنمای طراحی پلاگین](docs/plugin_guide.html)
- [راهنمای طراحی قالب](docs/theme_guide.html)
- [مستندات API موبایل](docs/api_reference.md)
- [راهنمای انجمن و پشتیبانی](docs/messaging_guide.html)

---

## 🤝 مشارکت و توسعه
- Pull Request و Issue پذیرفته می‌شود.
- لطفاً قبل از مشارکت، [CONTRIBUTING.md](docs/CONTRIBUTING.md) را مطالعه کنید.
- سورس در [گیت‌هاب Dima CMS](https://github.com/balvardi/dimacms) منتشر شده است.

---

## 👨‍💻 مشارکت هوش مصنوعی
> بخش قابل توجهی از توسعه و مستندسازی این پروژه با همکاری هوش مصنوعی (AI) و ابزار [GitHub Copilot](https://github.com/features/copilot) و [ChatGPT](https://openai.com/chatgpt) انجام شده است. اگر این پروژه برای شما مفید بود، لطفاً در گیت‌هاب ستاره بزنید و به توسعه آن کمک کنید!

---

## 📝 لایسنس
GPL-3.0 License

---

> Dima CMS توسط جامعه متن‌باز و با کمک هوش مصنوعی توسعه داده می‌شود. با ما همراه باشید! 🚀 
