# Git
پروژه‌های زیادی وجود دارد که همه‌ی کارهای خواسته شده در آن‌ها توسط اعضای تیم انجام شده که متاسفانه بیشتر آن‌ها پرایوت هستند ولی برای مثال تعدادی از پروژه‌ها با این ویژگی‌ها را ادامه می‌نویسیم. در این پروژه هم سعی شده موارد خواسته شده رعایت شود.

به طور معمول برای مرج کردن دو شاخه از rebase استفاده می‌کنیم، ولی با توجه به این که در هیستوری برطرف شدن کانفلیکت مشخص نخواهد شد در این ریپازیتوری از مرج استفاده می‌کنیم.

- https://github.com/software-engineering-lab-fall-2023/tdd
- https://github.com/web-programming-fall-2022/digivision-backend


# پرسش ها
## سوال ۱
### ۱.۱
پوشه .git  جز اصلی ریپازیتوری گیت است که همه  اطلاعات مورد نیاز برای ورژن کنترل را در  خود دارد.

### ۱.۲
 این پوشه شامل object ها و رفرنس ها و head و index و configfile و غیری میباشد.
 
### ۱.۳
این پوشه با دستور git init ساخته میشود.

## سوال ۲
 اتمیک بودن به این معنی است که آن کامیت یا پول ریکوئست هم نامرئی باشد و هم غیر قابل حذف. در عمل به تغییری تغییر اتمیک گفته میشود که به اندازه ای کوچک باشد که به راحتی بازبینی شده و مورد فهم قرار گیرد اما به حدی بزرگ باشد که یک ایده یا بهبود مشکل را کاملا پیاده سازی کرده باشد و از باقی کامیت ها مستقل باشد.

## سوال ۳
### ۳.۱
دستور fetch درخت ریموت را دریافت می‌کند.
### ۳.۲
دستور pull علاوه بر fetch کردن، آن را با لوکال مرج یا ریبیس نیز می‌کند و در نتیجه درخت برنچ لوکال تغییرات ریموت را خواهد داشت.
### ۳.۳
دستور merge دو کامیت از دو شاخه مختلف را به هم وصل می‌کند (دو والد دارد) و در آن هر گونه conflict موجود در این دو والد برطرف می‌شد. بنابراین محتوای این کامیت برطرف کردن conflict ها برای یکی کردن دو شاخه است.
### ۳.۴
دستور rebase کامیت‌های یک شاخه که از شاخه‌ی دیگر جدا شده‌اند را جدا کرده و در ادامه‌ی آخرین کامیت شاخه‌ی دیگر قرار می‌دهد و در حین قرار دادن هر جا conflict وجود داشته باشد آن را برطرف می‌کنیم و در نتیجه درخت ما به صورت خطی جلو می‌رود.
### ۳.۵
دستور cherry-pick یک کامیت مشخص را کپی کرده و شاخه‌ی فعلی ما قرار می‌دهد. بنابراین از این دستور می‌توان برای آوردن فقط یک کامیت خاص از یک شاخه دیگر استفاده کرد بدون این که نیاز باشد کل آن شاخه مرج شود.
