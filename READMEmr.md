घेणे किंवा प्रकल्प बनवणे 
| Command                                             | Description                                           |
|-----------------------------------------------------|-------------------------------------------------------|
| `git init`                                          | स्थानिक गीट रेपोसिटोरी आरंभ करा                               |
| `git clone ssh://git@github.com/[username]/[repo]`  | रिमोट ला असलेले बदल तुमचा लोकल ला घ्या                        |


मूलभूत स्नॅपशॉटिंग
| Command                             | Description                                     |
|-------------------------------------|-------------------------------------------------|
| `git status`                        | स्थिती तपासा                                       |
| `git add [file-name.txt]`           | स्टेजिंग क्षेत्रामध्ये फाइल जोडा                             |
| `git add -A`                        | सर्व नवीन आणि बदललेल्या फाइल्स स्टेजिंग क्षेत्रात जोडा           |
| `git commit -m "[commit message]"`  | बदल कंमीट करा                                  |
| `git rm -r [file-name.txt]`         | फाइल (किंवा फोल्डर) काढा                      |


शाखा आणि विलीनीकरण
| Command                                        | Description                                               |
|------------------------------------------------|-----------------------------------------------------------|
| `git branch`                                   |शाखांची यादी करा                                               |
| `git branch -a`                               | सर्व शाखांची यादी करा (स्थानिक आणि रिमोट)                     |
| `git branch [branch name]`                    | नवीन शाखा तयार करा                                       |
| `git branch -d [branch name]`                 | शाखा काढून टाका                                       |
| `git push origin --delete [branch name]`      |  रिमोट ला असलेली शाखा काढून टाका                                    |
| `git checkout -b [branch name]`               | नवीन शाखा तयार करा आणि त्यावर स्विच करा                     |
| `git checkout -b [branch name] origin/[branch name]` |रिमोट ला असलेली शाखा क्लोन करा आणि त्यावर स्विच करा           |
| `git branch -m [old branch name] [new branch name]` | स्थानिक शाखेचे नाव बदला                             |
| `git checkout [branch name]`                  | शाखा बदला                                       |
| `git checkout -`                              | शेवटचे चेक आउट केलेल्या शाखेत जा                   |
| `git checkout -- [file-name.txt]`             | फाइलमधील बदल टाकून द्या                                |
| `git merge [branch name]`                     | सक्रिय शाखेत शाखा विलीन करा                    |
| `git merge [source branch] [target branch]`   | लक्ष्य शाखेत शाखा विलीन करा                      |
| `git stash`                                    | खराब डिरेक्टरी मध्ये स्टेश बदला                |
| `git stash clear`                             | सगळ्या स्टेश प्रवेश काढून टाका                                |


प्रकल्प सामायिक करणे आणि अद्यतनित करणे
| Command                                                   | Description                                                   |
|-----------------------------------------------------------|---------------------------------------------------------------|
| `git push origin [branch name]`                           | तुमच्या रिमोट रेपॉजिटरीमध्ये शाखा पुश करा                    |
| `git push -u origin [branch name]`                        | रिमोट रिपॉझिटरीमध्ये बदल पुश करा (आणि शाखा लक्षात ठेवा)   |
| `git push`                                                |रिमोट रिपॉझिटरीमध्ये बदल पुश करा (लक्षात असलेली शाखा)         |
| `git push origin --delete [branch name]`                  | रिमोट ला असलेली शाखा काढून टाका                                        |
| `git pull`                                                | नवीन कमिटमध्ये स्थानिक भांडार अद्यतनित करा                  |
| `git pull origin [branch name]`                           | रिमोट रिपॉजिटरीमधून बदल खेचा                           |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | रिमोट रेपॉजिटरी जोडा                           |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | रेपॉजिटरीची मूळ शाखा SSH वर सेट करा         |


तपासणी आणि तुलना
| Command                                     | Description                                    |
|---------------------------------------------|------------------------------------------------|
| `git log`                                   | बदल बघा                                    |
| `git log --summary`                         | बदल बघा  (संपूर्ण)                        |
| `git log --oneline`                         | बदल बघा (थोडक्यात)                         |
| `git diff [source branch] [target branch]`  | विलीन करण्यापूर्वी बदलांचे पूर्वावलोकन करा               |

