اكواد جيث
============

## الإصدارات المترجمة
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)

___

_قائمة بأوامر جيث شائعة الاستخدام_

*ذا كنت مهتمًا بالأسماء المستعارة الخاصة بـ Git، فقم بإلقاء نظرة على `.bash_profile`, من هنا: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### الحصول على المشاريع وإنشائها 

| أمر | وصف                                        |
| ------- |--------------------------------------------|
| `git init` | قم بتهيئة الملف جيث المحلي                 |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | إنشاء نسخة محلية من ملف رئيسي |

### الأساسيات 

| أمر | وصف |
| ------- | ----------- |
| `git status` | تحقق من حالة |
| `git add [file-name.txt]` | إضافة ملف إلى منطقة التدريج |
| `git add -A` | قم بإضافة كافة الملفات الجديدة والمتغيرة إلى منطقة التدريج |
| `git commit -m "[commit message]"` | نشر التغييرات |
| `git rm -r [file-name.txt]` | إزالة ملف أو مجلد |

### التفرع والدمج

| أمر | وصف |
| ------- | ----------- |
| `git branch` | قائمة الفروع تشير العلامة النجمية إلى الفرع الحالي |
| `git branch -a` | قائمة بجميع الفروع (المحلية والبعيدة) |
| `git branch [branch name]` | إنشاء فرع جديد |
| `git branch -d [branch name]` | حذف فرع |
| `git push origin --delete [branch name]` | حذف فرع بعيد |
| `git checkout -b [branch name]` | إنشاء فرع جديد والتبديل إليه |
| `git checkout -b [branch name] origin/[branch name]` |  استنساخ فرع بعيد والتبديل إليه |
| `git branch -m [old branch name] [new branch name]` |  إعادة تسمية فرع محلي |
| `git checkout [branch name]` |  التبديل إلى فرع |
| `git checkout -` | التبديل إلى الفرع الذي تم الخروج منه آخر مرة  |
| `git checkout -- [file-name.txt]` | تجاهل التغييرات التي طرأت على ملف  |
| `git merge [branch name]` | دمج فرع في الفرع النشط |
| `git merge [source branch] [target branch]` | دمج فرع في فرع مستهدف |
| `git stash` |  تخزين التغييرات في دليل عمل متسخ  |
| `git stash clear` | إزالة جميع المشاركات المخزنة  |

### مشاركة وتحديث المشاريع 

| أمر | وصف |
| ------- | ----------- |
| `git push origin [branch name]` | نشر فرع إلى مستودعك البعيد |
| `git push -u origin [branch name]` | نشر التغييرات إلى المستودع البعيد (وتذكر الفرع) |
| `git push` | نشر التغييرات إلى المستودع البعيد (الفرع المتذكر) |
| `git push origin --delete [branch name]` | حذف فرع بعيد |
| `git pull` |  تحديث المستودع المحلي إلى أحدث التغييرات |
| `git pull origin [branch name]` | سحب التغييرات من المستودع البعيد |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | إضافة مستودع بعيد |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | تعيين فرع الأصل في المستودع على SSH  |

### التفتيش والمقارنة 

| أمر | وصف |
| ------- | ----------- |
| `git log` | عرض التغييرات |
| `git log --summary` | عرض التغييرات (مفصّلة) |
| `git log --oneline` | عرض التغييرات (باختصار) |
| `git diff [source branch] [target branch]` | معاينة التغييرات قبل الدمج |
