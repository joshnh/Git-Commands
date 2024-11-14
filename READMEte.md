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

### ప్రాజెక్ట్‌లను షేరింగ్ చేయడం మరియు అప్డేట్ చేయడం 

| కమాండ్ | వివరణ |
| ----- | ----- |
| `git push origin [branch name]` | మీ రిమోట్ రిపోజిటరీకి ఒక బ్రాంచ్ని పుష్ చేయండి |
| `git push -u origin [branch name]` | రిమోట్ రిపోజిటరీకి మార్పులను పుష్ చేయండి (మరియు ఆ బ్రాంచ్ని గుర్తుంచుకోండి) |
| `git push` | రిమోట్ రిపోజిటరీకి మార్పులను పుష్ చేయండి (అదే గుర్తుపెట్టుకున్న బ్రాంచ్లో) |
| `git push origin --delete [branch name]` | ఒక రిమోట్ బ్రాంచ్ని తొలగించండి |
| `git pull` | లోకల్ రిపోజిటరీని సరికొత్త కమిట్‌కి అప్‌డేట్ చేయండి |
| `git pull origin [branch name]` | రిమోట్ రిపోజిటరీ నుండి మార్పులను పుల్ చేయండి |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | రిమోట్ రిపోజిటరీని జోడించండి |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | రిపోజిటరీ యొక్క అరిజిన్ బ్రాంచ్ని SSHకి సెట్ చేయండి |

### గమనించి & సరిపోల్చండి

| కమాండ్ | వివరణ |
| ----- | ----- |
| `git log` | మార్పులను వీక్షించండి |
| `git log --summary` | మార్పులను వీక్షించండి (వివరంగా) |
| `git log --oneline` | మార్పులను వీక్షించండి (క్లుప్తంగా) |
| `git diff [source branch] [target branch]` | మర్జింగ్ చేయడానికి ముందు మార్పులను సమీక్షించండి |