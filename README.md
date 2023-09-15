<p align="center">
  <a href="https://github.com/oXIIIo/marzban-template/" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
      <img width="160" height="160" src="https://raw.githubusercontent.com/Gozargah/Marzban-docs/master/screenshots/logo-dark.png">
    </picture>
  </a>
</p>
<h1 align="center"/>تمپلیت های مختلف برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

# مقدمه
لیستی از تمپلیت های شخصی سازی شده برای مرزبان

# لیست تمپلیت ها
- [تمپلیت برای clash و clash-meta](https://github.com/oXIIIo/marzban-template/tree/master/clash)
- [تمپلیت برای sing-box](https://github.com/oXIIIo/marzban-template/tree/master/singbox)
- [صفحه سابسکریپشن](https://github.com/oXIIIo/marzban-template/tree/master/subscription)
- [صفحه خانه](https://github.com/oXIIIo/marzban-template/tree/master/home)


# مراحل نصب
برای نصب هر تمپلیت به صفحه مربوط به آن مراجعه کنید

# نصب همه
برای نصب همه تمپلیت های موجو دستورات زیر را در ترمینال سرور خود اجرا کنید:
1. دانلود فایل های تمپلیت
```sh
sudo wget -N -P /var/lib/marzban/templates/clash/ https://raw.githubusercontent.com/oXIIIo/marzban-template/master/clash/default.yml
sudo wget -N -P /var/lib/marzban/templates/singbox/ https://raw.githubusercontent.com/oXIIIo/marzban-template/master/singbox/default.json
sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/oXIIIo/marzban-template/master/subscription/index.html
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/oXIIIo/marzban-template/master/home/index.html
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت ها فقط کافیست مرحله 1 را تکرار کنید.

