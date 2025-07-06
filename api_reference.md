# Dima CMS API Reference

این مستند راهنمای کامل استفاده از API RESTful برای اتصال نرم‌افزار موبایل یا کلاینت‌های دیگر به Dima CMS است.

---

## احراز هویت (Authentication)

### ثبت‌نام
`POST /api/register`

**Body (JSON):**
```
{
  "username": "user1",
  "email": "user1@example.com",
  "password": "123456"
}
```
**Response:**
```
{"status":"ok"}
```

### ورود و دریافت توکن JWT
`POST /api/login`

**Body (JSON):**
```
{
  "username": "user1",
  "password": "123456"
}
```
**Response:**
```
{"token": "...JWT..."}
```

### دریافت پروفایل کاربر
`GET /api/user`

**Headers:**
`Authorization: Bearer {JWT}`

**Response:**
```
{
  "user": {
    "id": 1,
    "username": "user1",
    "email": "user1@example.com",
    ...
  }
}
```

---

## انجمن (Forum)

### لیست انجمن‌ها
`GET /api/forums`

**Response:**
```
{"forums": [ {"id":1, "title":"عمومی", ...}, ... ]}
```

### لیست موضوعات هر انجمن
`GET /api/forums/{id}/threads`

**Response:**
```
{"threads": [ {"id":1, "title":"سوالات متداول", ...}, ... ]}
```

### لیست پست‌های هر موضوع
`GET /api/threads/{id}/posts`

**Response:**
```
{"posts": [ {"id":1, "body":"...", ...}, ... ]}
```

---

## پشتیبانی (Support)

### لیست تیکت‌های کاربر
`GET /api/tickets`

**Headers:**
`Authorization: Bearer {JWT}`

**Response:**
```
{"tickets": [ {"id":1, "subject":"مشکل ورود", ...}, ... ]}
```

### مشاهده تیکت و پاسخ‌ها
`GET /api/tickets/{id}`

**Headers:**
`Authorization: Bearer {JWT}`

**Response:**
```
{
  "ticket": {"id":1, "subject":"مشکل ورود", ...},
  "replies": [ {"id":1, "body":"...", ...}, ... ]
}
```

### ارسال پاسخ به تیکت
`POST /api/tickets/{id}/reply`

**Headers:**
`Authorization: Bearer {JWT}`

**Body (JSON):**
```
{
  "body": "پاسخ به تیکت ..."
}
```
**Response:**
```
{"status":"ok"}
```

---

## نکات امنیتی و توسعه
- همه درخواست‌های نیازمند احراز هویت باید هدر `Authorization: Bearer {JWT}` داشته باشند.
- توکن JWT را امن نگه دارید و در هر درخواست ارسال کنید.
- خروجی API همیشه JSON استاندارد است و در صورت خطا، فیلد `error` دارد.
- برای توسعه endpointهای جدید، همین ساختار را دنبال کنید.

---

## توسعه آینده
- افزودن endpointهای پیام‌رسانی، فروشگاه، نوتیفیکیشن و ...
- مستندسازی Swagger/OpenAPI (در صورت نیاز)
- مثال‌های بیشتر و سناریوهای کاربردی

---

**تهیه و توسعه: تیم Dima CMS** 