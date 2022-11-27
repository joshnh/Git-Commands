Git Commands
============

## Translated Versions
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)

___

_आमतौर पर उपयोग किए जाने वाले गिट कमांड की सूची_

*यदि आप गिट उपनामों में रुचि रखते हैं, तो यहां `.bash_profile` पर एक नज़र डालें: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | लोकल गिट रिपॉजिटरी को इनिशियलाइज़ करें |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | अपनी रिपॉजिटरी की एक लोकल कॉपी बनाएँ |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | स्टेटस जांचीये |
| `git add [file-name.txt]` | फ़ाइल को स्टेजिंग एरिया जोड़ें |
| `git add -A` | सभी नई और परिवर्तित फ़ाइलें को स्टेजिंग एरिया जोड़ें |
| `git commit -m "[commit message]"` | चैन्जश को मेसज के साथ कमिट करे |
| `git rm -r [file-name.txt]` | एक फ़ाइल (या फ़ोल्डर) निकालें |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | ब्रांचश की सूची बनाएं (ऐस्टरिस्क(*) साइन वर्तमान शाखा को दर्शाता है) |
| `git branch -a` | सभी ब्रांचश की सूची बनाएं (लोकल और रिमोट) |
| `git branch [branch name]` | एक नई ब्रांच बनाएँ |
| `git branch -d [branch name]` | एक ब्रांच डिलीट करे |
| `git push origin --delete [branch name]` | एक रिमोट ब्रांच हटाएं |
| `git checkout -b [branch name]` | एक नई ब्रांच बनाएं और उसमें स्विच करें |
| `git checkout -b [branch name] origin/[branch name]` | एक रिमोट ब्रांच को क्लोन करें और उसमें स्विच करें |
| `git branch -m [old branch name] [new branch name]` | एक रिमोट ब्रांच का नाम बदलें |
| `git checkout [branch name]` | एक ब्रांच पर स्विच करें |
| `git checkout -` | पिछली बार चेक आउट की गई ब्रांच में स्विच करें |
| `git checkout -- [file-name.txt]` | फ़ाइल में सभी परिवर्तन निकालें |
| `git merge [branch name]` | एक ब्रांच को ऐक्टिव ब्रांच में मर्ज करें |
| `git merge [source branch] [target branch]` | एक ब्रांच को टार्गेट ब्रांच में मर्ज करें |
| `git stash` | वर्किंग फोल्डर में चैन्जश को स्टैश करें |
| `git stash clear` | सभी स्टैश चैन्जश हटाएं |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | अपने रिमोट रिपॉजिटरी में ब्रांच को पुश करें |
| `git push -u origin [branch name]` | रिमोट रिपॉजिटरी में ब्रांच को पुश करें (और शाखा को याद करो) |
| `git push` | रिमोट रिपॉजिटरी में ब्रांच को पुश करें (याद की गई ब्रांच में) |
| `git push origin --delete [branch name]` | एक रिमोट ब्रांच को डिलीट करे |
| `git pull` | अपनी लोकल रिपॉजिटरी को लेटेस्ट कमिट में अपडेट करें |
| `git pull origin [branch name]` | रिमोट रिपॉजिटरी में से चैन्जश पुल करे |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | एक रिमोट रिपॉजिटरी जोड़ें |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | रिपॉजिटरी की ओरिजिन ब्रांच को SSH पर सेट करें |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | चैन्जश देखें |
| `git log --summary` | चैन्जश देखें (डीटेल में) |
| `git log --oneline` | चैन्जश देखें (संक्षेप में) |
| `git diff [source branch] [target branch]` | मर्जिंग से पहले चैन्जश का समीक्षा करें |
