Git కమాండ్స్
============

## అనువదించబడిన సంస్కరణ
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)
- [English Version](README.md)

___

_సాధారణంగా ఉపయోగించే Git కమాండ్స్ జాబితా_

*మీకు git మారుపేర్లపై ఆసక్తి ఉంటే, ఇక్కడ `.bash_profile`ని చూడండి: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### ప్రాజెక్ట్‌ను పొందడం మరియు సృష్టించడం


| కమాండ్ | వివరణ |
| ----- | ----- |
| `git init` | లోకల్ git రిపోజిటరీని ప్రారంభించండి |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | రిమోట్ రిపోజిటరీ యొక్క లోకల్ కాపీని సృష్టించండి |

### బేసిక్ స్నాప్‌షాటింగ్

| కమాండ్ | వివరణ |
| ----- | ----- |
| `git status` | ఫైల్ స్తితిని చెక్ చేయండి |
| `git add [file-name.txt]` | స్టేజింగ్ ప్రాంతానికి ఫైల్‌ను జోడించండి |
| `git add -A` | స్టేజింగ్ ఏరియాకు అన్ని కొత్త మరియు మార్చబడిన ఫైల్‌లను జోడించండి |
| `git commit -m "[commit message]"` | మార్పులు కమిట్ చేయండి |
| `git rm -r [file-name.txt]` | ఫైల్ (లేదా ఫోల్డర్)ని తీసివేయండి |
| `git remote -v` | ప్రస్తుతం పని చేస్తున్న ఫైల్ లేదా డైరెక్టరీ యొక్క రిమోట్ రిపోజిటరీని వీక్షించండి |

### బ్రాంచింగ్ మరియు మర్జింగ్

| కమాండ్ | వివరణ |
| ----- | ----- |
| `git branch` | బ్రాంచ్ల జాబితా  (ఆస్టరిస్క్ [*] గుర్తు ప్రస్తుత బ్రాంచ్ని సూచిస్తుంది) |
| `git branch -a` | అన్ని బ్రాంచ్ల జాబితా చేయండి (లోకల్ మరియు రిమోట్) |
| `git branch [branch name]` | కొత్త బ్రాంచ్ని సృష్టించండి |
| `git branch -d [branch name]` | ఒక బ్రాంచ్ని తొలగించండి |
| `git push origin --delete [branch name]` | రిమోట్ బ్రాంచ్ని తొలగించండి |
| `git checkout -b [branch name]` | కొత్త బ్రాంచ్ సృష్టించండి మరియు దానికి మారండి |
| `git checkout -b [branch name] origin/[branch name]` | రిమోట్ బ్రాంచ్ క్లోన్ చేసి దానికి మారండి |
| `git branch -m [old branch name] [new branch name]` | రిమోట్ బ్రాంచ్ పేరు మార్చండి |
| `git checkout [branch name]` | ఒక బ్రాంచ్కి మారండి |
| `git checkout -` |చివరిగా చెక్కౌట్ చేసిన బ్రాంచ్కి మారండి |
| `git checkout -- [file-name.txt]` | ఒకే ఫైల్‌లోని అన్ని మార్పులను తీసివేయండి |
| `git merge [branch name]` | ఒక బ్రాంచ్ ని యాక్టివ్ బ్రాంచ్ లో మర్జ్ చేయండి |
| `git merge [source branch] [target branch]` | ఒక బ్రాంచ్ని టార్గెట్ బ్రాంచ్ లో మర్జ్ చేయండి |
| `git stash` | పనిచేసే ఫోల్డర్‌లో మార్పులను స్టాష్ చేయండి |
| `git stash clear` | అన్ని స్టాష్ ఎంట్రీలను తొలగించండి |

### प्राजेक्ट्स को शेर और अप्डेट करना

| కమాండ్ | వివరణ |
| ----- | ----- |
| `git push origin [branch name]` | अपने रिमोट रिपॉजिटरी में ब्रांच को पुश करें |
| `git push -u origin [branch name]` | रिमोट रिपॉजिटरी में ब्रांच को पुश करें (और उसी ब्रांच को याद रखे) |
| `git push` | रिमोट रिपॉजिटरी में ब्रांच को पुश करें (उसी याद की गई ब्रांच में) |
| `git push origin --delete [branch name]` | एक रिमोट ब्रांच को डिलीट करे |
| `git pull` | अपनी लोकल रिपॉजिटरी को लेटेस्ट कमिट में अपडेट करें |
| `git pull origin [branch name]` | रिमोट रिपॉजिटरी में से चैन्जश पुल करे |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | एक रिमोट रिपॉजिटरी जोड़ें |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | रिपॉजिटरी की ओरिजिन ब्रांच को SSH पर सेट करें |

### निरीक्षण और तुलना

| కమాండ్ | వివరణ |
| ----- | ----- |
| `git log` | चैन्जश देखें |
| `git log --summary` | चैन्जश देखें (डीटेल में) |
| `git log --oneline` | चैन्जश देखें (संक्षेप में) |
| `git diff [source branch] [target branch]` | मर्जिंग से पहले चैन्जश की समीक्षा करें |
करें