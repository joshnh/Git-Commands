Git Commands
============

## دستورات گیت
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [Azərbaycanca versiya](READMEaz.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)
- [فارسی](READMEfr.md)

___

_فهرستی از دستورات گیت که من به‌طور معمول استفاده می‌کنم_

*اگر به نام‌های مستعار گیت من علاقه‌مند هستید، به `.bash_profile` من نگاهی بیندازید که در اینجا پیدا می‌شود: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### دریافت و ایجاد پروژه‌ها

| دستور | توضیح |
| ------- | ----------- |
| `git init` | یک مخزن گیت محلی را راه‌اندازی کنید |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | یک کپی محلی از یک مخزن راه دور ایجاد کنید |

### اسنپ‌شات‌گیری پایه

| دستور | توضیح |
| ------- | ----------- |
| `git status` | وضعیت را بررسی کنید |
| `git add [file-name.txt]` | یک فایل را به منطقه‌ی استیج اضافه کنید |
| `git add -A` | تمام فایل‌های جدید و تغییر کرده را به منطقه‌ی استیج اضافه کنید |
| `git commit -m "[commit message]"` | تغییرات را کامیت کنید |
| `git rm -r [file-name.txt]` | یک فایل (یا پوشه) را حذف کنید |
| `git remote -v` | مشاهده‌ی مخزن راه دور فایل یا دایرکتوری در حال کار |

### شاخه‌بندی و ادغام

| دستور | توضیح |
| ------- | ----------- |
| `git branch` | لیست شاخه‌ها (ستاره نشان‌دهنده‌ی شاخه‌ی جاری است) |
| `git branch -a` | لیست تمام شاخه‌ها (محلی و راه دور) |
| `git branch [branch name]` | ایجاد یک شاخه‌ی جدید |
| `git branch -d [branch name]` | حذف یک شاخه |
| `git push origin --delete [branch name]` | حذف یک شاخه‌ی راه دور |
| `git checkout -b [branch name]` | ایجاد و سوئیچ به یک شاخه‌ی جدید |
| `git checkout -b [branch name] origin/[branch name]` | کلون کردن یک شاخه‌ی راه دور و سوئیچ به آن |
| `git branch -m [old branch name] [new branch name]` | تغییر نام یک شاخه‌ی محلی |
| `git checkout [branch name]` | سوئیچ به یک شاخه |
| `git checkout -` | سوئیچ به شاخه‌ای که آخرین بار انتخاب شده است |
| `git checkout -- [file-name.txt]` | تغییرات یک فایل را لغو کنید |
| `git merge [branch name]` | ادغام یک شاخه با شاخه‌ی فعال |
| `git merge [source branch] [target branch]` | ادغام یک شاخه با شاخه‌ی هدف |
| `git stash` | ذخیره‌ی تغییرات در یک دایرکتوری کاری کثیف |
| `git stash clear` | حذف تمام موارد ذخیره‌شده |
| `git stash pop` | اعمال آخرین تغییرات ذخیره‌شده در دایرکتوری کاری |

### به اشتراک‌گذاری و به‌روزرسانی پروژه‌ها

| دستور | توضیح |
| ------- | ----------- |
| `git push origin [branch name]` | ارسال یک شاخه به مخزن راه دور |
| `git push -u origin [branch name]` | ارسال تغییرات به مخزن راه دور (و به خاطر سپردن شاخه) |
| `git push` | ارسال تغییرات به مخزن راه دور (شاخه به خاطر سپرده شده) |
| `git push origin --delete [branch name]` | حذف یک شاخه‌ی راه دور |
| `git pull` | به‌روزرسانی مخزن محلی به جدیدترین کامیت |
| `git pull origin [branch name]` | دریافت تغییرات از مخزن راه دور |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | افزودن یک مخزن راه دور |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | تنظیم شاخه‌ی origin مخزن به SSH |

### بازرسی و مقایسه

| دستور | توضیح |
| ------- | ----------- |
| `git log` | مشاهده‌ی تغییرات |
| `git log --summary` | مشاهده‌ی تغییرات (جزئیات) |
| `git log --oneline` | مشاهده‌ی تغییرات (خلاصه) |
| `git diff [source branch] [target branch]` | پیش‌نمایش تغییرات قبل از ادغام |
