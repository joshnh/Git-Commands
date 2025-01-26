دستورات گیت
============

## نسخه های ترجمه شده
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [Azərbaycanca versiya](READMEaz.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)
- [فارسی](READMEir.md)
___

_فهرستی از دستورات گیت که معمولاً استفاده می کنم_

*اگر به نام مستعار گیت من علاقه دارید، به `bash_profile.` من که در اینجا یافت می شود نگاه کنید: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### دریافت و ایجاد پروژه ها

| دستور | توضیحات |
| ------- | ----------- |
| `git init` | ایجاد یک ریپوزیتوری یا مخزن در لوکال |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | کپی کردن یک ریموت ریپوزیتوری در لوکال |

### مبانی

| دستور | توضیحات |
| ------- | ----------- |
| `git status` | بررسی کردن وضعیت |
| `git add [file-name.txt]` | اضافه کردن یک فایل به استیجینگ |
| `git add -A` | اضاغه کردن همه ی فایل های جدیدِ تغییر یافته به استیجینگ |
| `git commit -m "[commit message]"` | ثبت تغییرات با پیام مناسب |
| `git rm -r [file-name.txt]` | حذف کردن یک فایل یا فولدر |
| `git remote -v` | مشاهده ی ریموت ریپوزیتوری از فایل یا دایرکتوری فعلیِ در حال کار |

### شاخه ها یا برنچ ها و ادغام کردن آنها

| دستور | توضیحات |
| ------- | ----------- |
| `git branch` | لیست شاخه ها یا برنچ ها را نمایش می دهد (ستاره نشان دهنده ی شاخه ی فعلی است) |
| `git branch -a` | لیست تمام برنچ ها یا شاخه ها (اعم از داخلی و ریموت) |
| `git branch [branch name]` | ساخت یک برنچ یا شاخه ی جدید |
| `git branch -d [branch name]` | حذف یک شاخه |
| `git push origin --delete [branch name]` | حذف یک ریموت برنچ یا شاخه ی ریموت |
| `git checkout -b [branch name]` | ساخت یک برنچ جدید و سوئیچ کردن به آن در لحظه |
| `git checkout -b [branch name] origin/[branch name]` | نسخه برداری از یک ریموت برنچ و سوئیچ کردن به آن در لحظه |
| `git branch -m [old branch name] [new branch name]` | تغییر نام یک برنچ یا شاخه ی محلی یا لوکال |
| `git checkout [branch name]` | سوئیچ کردن به یک برنچ یا شاخه |
| `git checkout -` | رفتن به شاخه یا برنچی که آخرین بار بررسی شد یا در آن بودیم |
| `git checkout -- [file-name.txt]` | حذف تغییرات درون یک فایل |
| `git merge [branch name]` | ادغام کردن یا مرج کردن یک شاخه یا برنچ در شاخه یا برنچ فعال |
| `git merge [source branch] [target branch]` | ادغام یا مرج کردن شاخه یا برنچ فرعی در شاخه برنچ هدف |
| `git stash` | ذخیره تغییرات در یک چرک نویس |
| `git stash clear` | حذف کردن تمام چرک نویس های ذخیره شده  |
| `git stash pop` | اضافه کردن آخرین چرک نویس را به ورکینگ دایرکتوری  |

### اشتراک‌گذاری و به‌روزرسانی پروژه‌ها

| دستور | توضیحات |
| ------- | ----------- |
| `git push origin [branch name]` | پوش کردن یه برنچ یا شاخه به مخزن ریموت شما |
| `git push -u origin [branch name]` | ارسال تغییرات به مخزن ریموت (و شاخه یا برنچ را به خاطر بسپار) |
| `git push` | ارسال تغییرات به مخزن ریموت (شاخه‌ای که به خاطر سپرده شده) |
| `git push origin --delete [branch name]` | حذف یک برنچ یا شاخه ی ریموت |
| `git pull` | به‌روزرسانی مخزن محلی به جدیدترین commit |
| `git pull origin [branch name]` | آوردن یا کشیدن تغییرات از مخزن یا ریپوزیتوری ریموت |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | اضافه کردن یک مخزن یا ریپوزیتوری ریموت |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | تنظیم یا قرار دادن شاخه ی اوریجین یک مخزن یا ریپوزیتوری به SHH |

### بازبینی و مقایسه

| دستور | توضیحات |
| ------- | ----------- |
| `git log` | مشاهده ی تغییرات |
| `git log --summary` | مشاهده ی تغییرات (به طور جزئی) |
| `git log --oneline` | مشاهده ی تغییرات (به طور مختصر) |
| `git diff [source branch] [target branch]` | پیش‌ نمایش تغییرات قبل از ادغام یا مرج کردن |
