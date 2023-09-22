গিট কমান্ডস
============

## অনুবাদিত সংস্করণ
- [English version (original)](README.md)
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)

___

_প্রায়শই ব্যবহৃত গিট কমান্ডের তালিকা_

*আপনি যদি গিট এলিয়াসে আগ্রহী হন তবে এখানে '.bash_profile' এ দেখুন: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

*অনুবাদে মূল ইংরেজি শব্দগুলো সংরক্ষণ করা হয়েছে, যেখানে "রিপোজিটরি" শব্দটিকে "রেপো", "লোকাল" কে "লোকাল" এবং "রিমোট" কে "রিমোট" হিসেবে অনুবাদ করা হয়েছে। আশা করি এগুলো বিবেচনা করলে ডকুমেন্ট থেকে উপকৃত হতে পারবেন .*

--

### প্রজেক্ট নামানো ও তৈরি করা

| কমান্ড | বর্ণনা |
| ------- | ----------- |
| `git init` | একটি লোকাল গিট রেপো শুরু করুন |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | একটি রিমোট রেপোর লোকাল অনুলিপি তৈরি করুন |

### বেসিক স্ন্যাপশট

| কমান্ড | বর্ণনা |
| ------- | ----------- |
| `git status` | স্ট্যটাস চেক করুন |
| `git add [file-name.txt]` | স্টেজিং এরিয়ায় একটি ফাইল এড করুন  |
| `git add -A` | স্টেজিং এলাকায় সমস্ত নতুন এবং পরিবর্তিত ফাইল এড করুন |
| `git commit -m "[commit message]"` | পরিবর্তনগুলোর কমিট (ব্যাখ্যা) করুন  |
| `git rm -r [file-name.txt]` | ফাইল (বা ডিরেক্টরি) ডিলেট করুন |

### ব্রাঞ্চিং এবং মার্জিং

| কমান্ড | বর্ণনা |
| ------- | ----------- |
| `git branch` | ব্রাঞ্চের তালিকা (তারকা চিহ্ন বর্তমান ব্রাঞ্চ নির্দেশ করে) |
| `git branch -a` | সকল ব্রাঞ্চের তালিকা (লোকাল এবং রিমোট উভয়ই একত্রে) |
| `git branch [branch name]` | নতুন ব্রাঞ্চ তৈরি করুন |
| `git branch -d [branch name]` | ব্রাঞ্চ ডিলিট করুন  |
| `git push origin --delete [branch name]` | রিমোট ব্রাঞ্চ ডিলিট করুন |
| `git checkout -b [branch name]` | একটি নতুন ব্রাঞ্চ তৈরি করুন এবং এতে স্যুইচ করুন |
| `git checkout -b [branch name] origin/[branch name]` | রিমোট ব্রাঞ্চ ক্লোন করুন এবং এটিতে স্যুইচ করুন |
| `git branch -m [old branch name] [new branch name]` | লোকাল ব্রাঞ্চের নাম পরিবর্তন করুন |
| `git checkout [branch name]` | স্পেসিফিক ব্রাঞ্চে স্যুইচ করুন |
| `git checkout -` | সর্বশেষ চেক করা ব্রাঞ্চে স্যুইচ করুন |
| `git checkout -- [file-name.txt]` | স্পেসিফিক ফাইলের পরিবর্তন মুছে ফেলুন |
| `git merge [branch name]` | একটিভ ব্রাঞ্চের সাথে আরেকটি ব্রাঞ্চ মার্জ করুন |
| `git merge [source branch] [target branch]` | টার্গেট ব্রাঞ্চের সাথে স্পেসিফিক ব্রাঞ্চ একত্রিত করুন |
| `git stash` | অসমাপ্ত কাজের ডিরেক্টরিতে পরিবর্তনগুলি সংরক্ষণ করুন |
| `git stash clear` | স্ট্যাশ এন্টিগুলো সরিয়ে ফেলুন |

### শেয়ারিং এবং আপডেটিং প্রোজেক্টগুলো

| কমান্ড | বর্ণনা |
| ------- | ----------- |
| `git push origin [branch name]` | রিমোট রেপোতে ব্রাঞ্চ পুশ করুন  |
| `git push -u origin [branch name]` | রিমোট রেপোতে পরিবর্তনগুলি পুশ করুন (এবং ব্রাঞ্চটি মনে রাখুন) |
| `git push` | রিমোট রিপোজিটরিতে পরিবর্তনগুলি পুশ করুন (যে শাখাটি ইতিমধ্যে মনে রাখা হয়েছে) |
| `git push origin --delete [branch name]` | রিমোট ব্রাঞ্চ ডিলিট করুন |
| `git pull` | সর্বশেষ কমিট দ্বারা স্থানীয় রেপো আপডেট করুন |
| `git pull origin [branch name]` | রিমোট রেপো থেকে পরিবর্তনগুলি পুল করুন |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | রিমোট রেপো এড করুন |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | রেপোর অরিজিন ব্রাঞ্চে SSH এ সেট করুন |

### পর্যালোচনা এবং তুলনা

| কমান্ড | বর্ণনা |
| ------- | ----------- |
| `git log` | পরিবর্তনগুলি দেখুন|
| `git log --summary` | পরিবর্তন দেখুন (বিস্তারিত) |
| `git log --oneline` | পরিবর্তনগুলি দেখুন (সংক্ষেপে)|
| `git diff [source branch] [target branch]` | মার্জ করার আগে চেঞ্জগুলির প্রিভিউ দেখুন |
