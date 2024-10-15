<p align="center">
  <a href="https://github.com/Gozargah/Marzban" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://s8.uupload.ir/files/screenshot_2024-10-15-19-23-22-210_com.android.chrome-edit_yxgr.jpg">
      <img width="340" height="640" src="https://s8.uupload.ir/files/screenshot_2024-10-15-19-23-22-210_com.android.chrome-edit_yxgr.jpg">
    </picture>
  </a>
</p>
<h1 align="center"/>قالب صفحه اشتراک 2 برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

## فهرست مطالب
- [ویژگی‌ ها](#ویژگی-ها)
- [مراحل نصب](#مراحل-نصب)
- [امکان درخواست شارژ اظطراری](#اظطراری)

# مقدمه
یک قالب html ساده برای نمایش بهتر اطلاعات کاربر

# ویژگی ها
- افزودن سریع لینک سابسکریپشن به برنامه ها
- لینک دانلود اپلیکیشن های مورد نیاز

# مراحل نصب
1. دانلود فایل template
```sh
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/Saj-1992/Marz-Theme2/refs/heads/main/index.html
```

2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
```

3. ری استارت مرزبان
```sh
marzban restart
```

# اشطراری
در خطوط 759 و 760 ( توکن بات و آیدی عددی اکانت را جایزگین کنید )

## بروزرسانی
برای بروزرسانی تمپلیت فقط کافیست مرحله 1 را تکرار کنید.



