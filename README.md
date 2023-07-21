<p align="center">
  <a href="https://github.com/oXIIIo/clash-meta-template" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Dreamacro/clash/master/docs/logo.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Dreamacro/clash/master/docs/logo.png">
    </picture>
  </a>
</p>
<h1 align="center"/>Clash Meta Config Example for <a href="https://github.com/Gozargah/Marzban">Marzban</a></h1>

## فهرست مطالب
- [ویژگی‌ ها](#ویژگی-ها)
- [مراحل نصب](#مراحل-نصب)
- [لینک دانلود کلش متا](#لینک-دانلود-کلش-متا)

# مقدمه
کلش متا یک پروکسی مبتنی بر قوانین است که به شما این امکان را می‌دهد که تنظیمات مربوط به برنامه از قبیل DNS و مسیریابی و ... را از سمت سرور انجام دهید. به عنوان مثال، می‌توانید از سمت سرور، کلش را به گونه‌ای تنظیم کنید که اتصال به سایت‌های ایرانی به صورت مستقیم انجام شود.

# ویژگی ها
- وصل شدن به سریع ترین کانفیگ
- وصل شدن به اولین کانفیگ سالم
- لودبالانس
- وصل شدن مستقیم به وب‌سایت‌های ایرانی هنگامی که فیلترشکن روشن است
- بلاک کردن تبلیغات
و ...

# مراحل نصب
1. دانلود فایل template
```sh
sudo wget -N -P /var/lib/marzban/templates/clash/  https://raw.githubusercontent.com/oXIIIo/clash-meta-template/master/template.yml
```

2. اضافه کردن مشخصات به فایل .env:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'CLASH_SUBSCRIPTION_TEMPLATE="clash/template.yml"' | sudo tee -a /opt/marzban/.env
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت فقط کافیست مرحله 1 را تکرار کنید.

# لینک دانلود کلش متا
- Android:
   - [Clash. Meta for Android](https://github.com/MetaCubeX/ClashMetaForAndroid/releases/tag/Prerelease-alpha)
- iOS:
  - [MFI](https://t.me/meta_for_ios)
- Windows：
  - [clash-verge](https://github.com/zzzgydi/clash-verge)
  - [ClashMetaForWindows_Mini](https://github.com/kogekiplay/ClashMetaForWindows_Mini)
  - [clashN](https://github.com/2dust/clashN)
  - [v2rayN](https://github.com/2dust/v2rayN)
  - [Clash.Mini](https://github.com/MetaCubeX/Clash.Mini)
- Mac OS：
  - [clash-verge](https://github.com/zzzgydi/clash-verge)
  - [ClashX.Meta](https://github.com/MetaCubeX/ClashX.Meta)
- Linux：
  - [clash-verge](https://github.com/zzzgydi/clash-verge)
