[ENG](./READEM.md)

<img src='./img/a.png'>
### ابزار پیشرفته مدیریت فایل، پردازش لاگ‌ها و استخراج اطلاعات حساس

این ابزار یک راهکار جامع برای پردازش و مدیریت فایل‌های متنی، لاگ‌ها و آرشیوهای فشرده است. هدف اصلی این پروژه تسهیل جستجو، استخراج، حذف، و سازمان‌دهی داده‌های بزرگ و پراکنده در سیستم‌های ذخیره‌سازی است. ابزار به گونه‌ای طراحی شده که بتواند به آسانی اطلاعات مهم را شناسایی کند و به کاربران در مدیریت داده‌های حساس کمک کند.

---

## **ویژگی‌های کلیدی**

### **1. مدیریت فایل‌های متنی (.txt)**
#### جستجوی هوشمند
این ابزار امکان جستجوی عبارات خاص در فایل‌های متنی را فراهم می‌کند. کاربران می‌توانند عبارت‌های کلیدی (مانند "username" یا "password") را مشخص کنند و نتایج به صورت فهرستی از فایل‌های متنی مرتبط ذخیره می‌شود.

#### حذف خودکار فایل‌ها
اگر فایل‌های متنی قدیمی یا غیرضروری در سیستم شما وجود دارد، این ابزار می‌تواند به‌صورت خودکار فایل‌هایی را که شامل کلمات کلیدی مشخص هستند حذف کند. 

#### استخراج اطلاعات حساس
ابزار می‌تواند با تجزیه فایل‌های متنی، اطلاعات مهم مانند نام کاربری، رمز عبور، یا URLهای مرتبط را استخراج کرده و در قالب فایل‌های خروجی ساختارمند ذخیره کند. این قابلیت برای ایجاد پایگاه داده‌هایی مانند `username:password` یا `url:username:password` بسیار مفید است.

---

### **2. مدیریت آرشیوهای فشرده (.zip و .rar)**
#### استخراج پوشه‌ها و فایل‌های خاص
ابزار می‌تواند فایل‌ها و پوشه‌های موردنظر را از آرشیوهای فشرده با استفاده از فیلترهای خاص (مانند نام کشور یا منطقه) استخراج کند. 

#### پشتیبانی از فرمت‌های متنوع
ابزار از آرشیوهای `.zip` و `.rar` پشتیبانی می‌کند و می‌تواند به‌صورت خودکار پوشه‌های دلخواه را از این آرشیوها خارج کند.

#### مرتب‌سازی خروجی
پوشه‌ها و فایل‌های استخراج‌شده به‌طور خودکار در مسیر مشخص‌شده توسط کاربر ذخیره می‌شوند و ساختاری سازمان‌دهی‌شده دارند.

---

### **3. مدیریت پوشه‌ها**
#### حذف پوشه‌ها بر اساس نام
کاربران می‌توانند پوشه‌هایی را که نام آن‌ها شامل کلمات کلیدی مشخص است حذف کنند. این قابلیت برای پاکسازی فایل‌های غیرضروری یا حساس استفاده می‌شود.

#### شمارش لاگ‌ها بر اساس منطقه
ابزار می‌تواند تعداد لاگ‌های موجود در هر پوشه را بر اساس کد منطقه (مانند `US` یا `FR`) شمارش کرده و نتایج را به صورت آماری نمایش دهد.

---

### **4. ایجاد پایگاه داده**
#### تولید پایگاه داده لاگین
ابزار می‌تواند اطلاعات استخراج‌شده از فایل‌های متنی را به‌صورت ساختارمند در فایل‌های خروجی ذخیره کند. پایگاه داده می‌تواند شامل فرمت‌های:
- `username:password`
- `url:username:password`

باشد.

#### حذف داده‌های تکراری
ابزار داده‌های تکراری را از پایگاه داده حذف کرده و تنها داده‌های یکتا را ذخیره می‌کند. این فرآیند باعث افزایش دقت و کاهش حجم داده‌ها می‌شود.

#### ذخیره‌سازی داده‌ها
اطلاعات یکتا به دو صورت در فایل‌های خروجی ذخیره می‌شود:
- فایل اصلی شامل تمام داده‌ها.
- فایل جداگانه برای داده‌های یکتا.

---

### **5. رابط کاربری خط فرمان**
#### منوی کاربرپسند
یک منوی ساده ولی قدرتمند با استفاده از متن و گرافیک ASCII برای راهنمایی کاربر ارائه شده است. کاربران می‌توانند با وارد کردن گزینه‌های عددی، عملکرد موردنظر خود را انتخاب کنند.

#### گزارش نتایج
ابزار پس از انجام هر عملیات، گزارش کامل از نتایج شامل تعداد فایل‌های پردازش‌شده، داده‌های استخراج‌شده، و مدت زمان عملیات را نمایش می‌دهد.

---

## **نصب و پیش‌نیازها**

### پیش‌نیازها
برای اجرای این ابزار، ابتدا باید Python و کتابخانه‌های زیر را نصب کنید. از دستورات زیر استفاده کنید:

```bash
pip install colorama tqdm rarfile
```

### نحوه کلون کردن پروژه
ابتدا مخزن گیت‌هاب پروژه را کلون کنید:
```bash
git clone https://github.com/your-repo-name.git
cd your-repo-name
```

### اجرای ابزار
برای اجرای ابزار، دستور زیر را اجرا کنید:
```bash
python tool.py
```

---

## **راهنمای استفاده**

### منوی اصلی
پس از اجرای ابزار، منوی زیر نمایش داده می‌شود:

```
 ____    ______   ___    ___       ____     __    __  ____    __  __  ____    ____       
/\  _`\ /\__  _\ /\_ \  /\_ \     /\  _`\  /\ \  /\ \/\  _`\ /\ \/\ \/\  _`\ /\  _`\     
\ \ \L\ \/_/\ \/ \//\ \ \//\ \    \ \ \/\_\\ `\`\\/'/\ \ \L\ \ \ \_\ \ \ \L\_\ \ \L\ \   
 \ \  _ <' \ \ \   \ \ \  \ \ \    \ \ \/_/_`\ `\ /'  \ \ ,__/\ \  _  \ \  _\L\ \ ,  /   
  \ \ \L\ \ \_\ \__ \_\ \_ \_\ \_   \ \ \L\ \ `\ \ \   \ \ \/  \ \ \ \ \ \ \L\ \ \ \\ \  
   \ \____/ /\_____\/\____\/\____\   \ \____/   \ \_\   \ \_\   \ \_\ \_\ \____/\ \_\ \_\
    \/___/  \/_____/\/____/\/____/    \/___/     \/_/    \/_/    \/_/\/_/\/___/  \/_/\/ /

----------------------------------------------
1. استخراج لاگ‌ها از آرشیوهای فشرده (.rar, .zip).
2. جستجو برای عبارات مشخص در فایل‌های متنی.
3. کاهش حجم لاگ‌ها (حذف فایل‌ها و پوشه‌ها).
4. شمارش پوشه‌ها بر اساس منطقه.
5. ایجاد پایگاه داده لاگین (login:pass).
6. ایجاد پایگاه داده کامل (url:login:pass).
7. خروج.
----------------------------------------------
```

با وارد کردن عدد مربوطه، می‌توانید عملیات موردنظر خود را اجرا کنید.

---

## **ساختار فایل‌ها**

- `tool.py`: فایل اصلی حاوی کد برنامه.
- `result.txt`: فایل خروجی شامل نتایج پردازش داده‌ها.
- `unique_entries.txt`: فایل خروجی شامل اطلاعات یکتا.
- `Extract/`: پوشه‌ای برای ذخیره فایل‌های استخراج‌شده از آرشیوها.

---

## **موارد استفاده**

- مدیریت و پردازش لاگ‌های سیستمی.
- استخراج اطلاعات حساس از فایل‌های متنی.
- پاکسازی فایل‌ها و پوشه‌های غیرضروری.
- ایجاد پایگاه داده برای آنالیز اطلاعات.

---

## **مشارکت**
اگر پیشنهادی دارید یا می‌خواهید به بهبود این ابزار کمک کنید، می‌توانید از طریق گیت‌هاب مشارکت کنید. بازخوردهای شما ارزشمند است! 😊

> نویسنده: [Your Name](https://github.com/your-profile)  
> لایسنس: MIT
