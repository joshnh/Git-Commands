Git Commands
============

## અનુવાદિત સંસ્કરણો
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [Azərbaycanca versiya](READMEaz.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)
- [ગુજરાતી અનુવાદ](READMEguj.md)

___

_હું સામાન્ય રીતે ઉપયોગ કરું છું એવા Git કમાન્ડ્સની યાદી_

*જો તમને મારા Git aliases માં રસ હોય, તો અહીં મળતી મારી `.bash_profile` જુઓ: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### પ્રોજેક્ટ્સ મેળવવા અને બનાવવા

| Command | Description |
| ------- | ----------- |
| `git init` | સ્થાનિક Git રિપોઝિટરી શરૂ કરો |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | રિમોટ રિપોઝિટરીની સ્થાનિક નકલ બનાવો |

### મૂળભૂત Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | સ્થિતિ તપાસો |
| `git add [file-name.txt]` | સ્ટેજિંગ વિસ્તારમાં ફાઇલ ઉમેરો |
| `git add -A` | બધી નવી અને બદલાયેલી ફાઇલો સ્ટેજિંગ વિસ્તારમાં ઉમેરો |
| `git commit -m "[commit message]"` | ફેરફારો commit કરો |
| `git rm -r [file-name.txt]` | ફાઇલ (અથવા ફોલ્ડર) દૂર કરો |
| `git remote -v` | હાલમાં કાર્યરત ફાઇલ અથવા ડિરેક્ટરીની રિમોટ રિપોઝિટરી જુઓ |

### Branching અને Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | બ્રાન્ચોની યાદી જુઓ (તારક ચિહ્ન વર્તમાન બ્રાન્ચ દર્શાવે છે) |
| `git branch -a` | બધી બ્રાન્ચોની યાદી જુઓ (સ્થાનિક અને રિમોટ) |
| `git branch [branch name]` | નવી બ્રાન્ચ બનાવો |
| `git branch -d [branch name]` | બ્રાન્ચ કાઢી નાખો |
| `git push origin --delete [branch name]` | રિમોટ બ્રાન્ચ કાઢી નાખો |
| `git checkout -b [branch name]` | નવી બ્રાન્ચ બનાવી તેમાં સ્વિચ કરો |
| `git checkout -b [branch name] origin/[branch name]` | રિમોટ બ્રાન્ચ ક્લોન કરી તેમાં સ્વિચ કરો |
| `git branch -m [old branch name] [new branch name]` | સ્થાનિક બ્રાન્ચનું નામ બદલો |
| `git checkout [branch name]` | બ્રાન્ચ પર સ્વિચ કરો |
| `git checkout -` | છેલ્લે checkout કરેલી બ્રાન્ચ પર સ્વિચ કરો |
| `git checkout -- [file-name.txt]` | ફાઇલમાં થયેલા ફેરફારો રદ કરો |
| `git merge [branch name]` | સક્રિય બ્રાન્ચમાં બીજી બ્રાન્ચ મર્જ કરો |
| `git merge [source branch] [target branch]` | સોર્સ બ્રાન્ચને ટાર્ગેટ બ્રાન્ચમાં મર્જ કરો |
| `git stash` | dirty working directory માં ફેરફારો stash કરો |
| `git stash clear` | સ્ટેશ કરેલી બધી એન્ટ્રીઓ દૂર કરો |
| `git stash pop` | તાજું stash working directory માં લાગુ કરો |

### પ્રોજેક્ટ્સ શેર કરવું અને અપડેટ કરવું

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | તમારી રિમોટ રિપોઝિટરીમાં બ્રાન્ચ push કરો |
| `git push -u origin [branch name]` | રિમોટ રિપોઝિટરીમાં ફેરફારો push કરો (અને બ્રાન્ચ યાદ રાખો) |
| `git push` | રિમોટ રિપોઝિટરીમાં ફેરફારો push કરો (યાદ રાખેલી બ્રાન્ચ) |
| `git push origin --delete [branch name]` | રિમોટ બ્રાન્ચ કાઢી નાખો |
| `git pull` | સ્થાનિક રિપોઝિટરીને નવીનતમ commit સુધી અપડેટ કરો |
| `git pull origin [branch name]` | રિમોટ રિપોઝિટરીમાંથી ફેરફારો pull કરો |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | રિમોટ રિપોઝિટરી ઉમેરો |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | રિપોઝિટરીની origin URL ને SSH પર સેટ કરો |

### નિરીક્ષણ અને તુલના

| Command | Description |
| ------- | ----------- |
| `git log` | ફેરફારો જુઓ |
| `git log --summary` | ફેરફારો જુઓ (વિગતવાર) |
| `git log --oneline` | ફેરફારો જુઓ (સંક્ષેપમાં) |
| `git diff [source branch] [target branch]` | મર્જ પહેલાં ફેરફારોનો પૂર્વાવલોકન કરો |
