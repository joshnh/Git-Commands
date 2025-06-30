Git આદેશો
============

## અનુવાદિત આવૃત્તિઓ
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [Azərbaycanca versiya](READMEaz.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)
- [ગુજરાતી અનુવાદ](READMEguj.md)

*મારા વપરાતા સામાન્ય Git આદેશોની યાદી*

**જો તમારે મારા Git aliases જોઈએ હોય, તો મારી `.bash_profile` અહીં જુઓ:**
[https://github.com/joshnh/bash\_profile/blob/master/.bash\_profile](https://github.com/joshnh/bash_profile/blob/master/.bash_profile)

--

### પ્રોજેક્ટ મેળવવો અને બનાવવો

| આદેશ                                                              | વર્ણન                            |
| ----------------------------------------------------------------- | -------------------------------- |
| `git init`                                                        | લોકલ Git રિપોઝિટરી શરૂ કરો       |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | રીમોટ રિપોઝિટરીની લોકલ નકલ બનાવો |


### આધારભૂત Snapshot લેનાં

| આદેશ                               | વર્ણન                                       |
| ---------------------------------- | ------------------------------------------- |
| `git status`                       | હાલત તપાસો                                  |
| `git add [file-name.txt]`          | ફાઇલને સ્ટેજિંગ એરિયામાં ઉમેરો              |
| `git add -A`                       | બધી નવી અને બદલાયેલ ફાઇલો સ્ટેજ કરો         |
| `git commit -m "[commit message]"` | ફેરફારો commit કરો                          |
| `git rm -r [file-name.txt]`        | ફાઇલ અથવા ફોલ્ડર દૂર કરો                    |
| `git remote -v`                    | હાલ કાર્યરત ફોલ્ડર માટે રીમોટ રિપોઝિટરી જુઓ |


### શાખા (Branch) અને મર્જિંગ

| આદેશ                                                 | વર્ણન                                                 |
| ---------------------------------------------------- | ----------------------------------------------------- |
| `git branch`                                         | શાખાઓની યાદી જુઓ (અસ્તેરિસ્ક વર્તમાન શાખા દર્શાવે છે) |
| `git branch -a`                                      | બધી શાખાઓ જુઓ (લોકલ અને રીમોટ)                        |
| `git branch [branch name]`                           | નવી શાખા બનાવો                                        |
| `git branch -d [branch name]`                        | શાખા દૂર કરો                                          |
| `git push origin --delete [branch name]`             | રીમોટ શાખા દૂર કરો                                    |
| `git checkout -b [branch name]`                      | નવી શાખા બનાવો અને તેમાં જાવ                          |
| `git checkout -b [branch name] origin/[branch name]` | રીમોટ શાખા ક્લોન કરો અને સ્વીચ કરો                    |
| `git branch -m [old name] [new name]`                | લોકલ શાખાનું નામ બદલો                                 |
| `git checkout [branch name]`                         | શાખા બદલો                                             |
| `git checkout -`                                     | છેલ્લી ચેકઆઉટ કરેલી શાખા પર પાછા જાઓ                  |
| `git checkout -- [file-name.txt]`                    | ફાઇલમાં કરેલા ફેરફારો રદ કરો                          |
| `git merge [branch name]`                            | એક શાખા બીજીમાં મર્જ કરો                              |
| `git merge [source] [target]`                        | નિર્ધારિત શાખા પર મર્જ કરો                            |
| `git stash`                                          | કામ દરમિયાનના ફેરફારો છુપાવો                          |
| `git stash clear`                                    | બધા stash દૂર કરો                                     |
| `git stash pop`                                      | છેલ્લો stash પાછો લાવો અને લાગૂ કરો                   |


### પ્રોજેક્ટ શેર અને અપડેટ કરવો

| આદેશ                                                                        | વર્ણન                                  |
| --------------------------------------------------------------------------- | -------------------------------------- |
| `git push origin [branch name]`                                             | શાખાને રીમોટ પર મોકલો                  |
| `git push -u origin [branch name]`                                          | શાખા મોકલો અને એ ડિફોલ્ટ તરીકે સેટ કરો |
| `git push`                                                                  | યાદ રહેલી શાખા માટે ફેરફારો મોકલો      |
| `git push origin --delete [branch name]`                                    | રીમોટ શાખા દૂર કરો                     |
| `git pull`                                                                  | લોકલ રિપોઝિટરીને અપડેટ કરો             |
| `git pull origin [branch name]`                                             | રીમોટ રિપોઝિટરીમાંથી અપડેટ લો          |
| `git remote add origin ssh://git@github.com/[username]/[repo-name].git`     | રીમોટ રિપોઝિટરી ઉમેરો                  |
| `git remote set-url origin ssh://git@github.com/[username]/[repo-name].git` | રીમોટ URL બદલો                         |


### તપાસ અને તુલના

| આદેશ                         | વર્ણન                          |
| ---------------------------- | ------------------------------ |
| `git log`                    | commit લોગ જુઓ                 |
| `git log --summary`          | વિસ્તૃત લોગ જુઓ                |
| `git log --oneline`          | સરસ સંક્ષિપ્ત commit લિસ્ટ જુઓ |
| `git diff [source] [target]` | મર્જ કરતા પહેલા ફેરફારો જુઓ    |
