<p align="center">
  <a href="https://github.com/oXIIIo/marzban-template/tree/master/home" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/oXIIIo/marzban-template/master/home/preview.gif">
      <img width="363" height="328" src="https://raw.githubusercontent.com/oXIIIo/marzban-template/master/home/preview.gif">
    </picture>
  </a>
</p>
<h1 align="center"/>قالب صفحه خانه برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

## فهرست مطالب
- [مقدمه](#مقدمه)
- [مراحل نصب](#مراحل-نصب)

# مقدمه
یک قالب html ساده برای صفحه خانه مرزبان

# مراحل نصب
1. دانلود فایل template
```sh
sudo wget -N -P /var/lib/marzban/templates/home/ https://raw.githubusercontent.com/oXIIIo/marzban-template/master/home/index.html
```

2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'HOME_PAGE_TEMPLATE="home/index.html"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
HOME_PAGE_TEMPLATE="home/index.html"
```

3. ری استارت مرزبان
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت فقط کافیست مرحله 1 را تکرار کنید.

# حمایت از من

<a href="https://nowpayments.io/donation?api_key=MG750CX-D7AMMH9-QWARQ7V-9ZKH9XQ&source=lk_donation&medium=referral" target="_blank">
  <img src="https://nowpayments.io/images/embeds/donation-button-black.svg" alt="Crypto donation button by NOWPayments">
</a>