Git Əmrləri
============

## Tərcümə versiyaları
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [Azərbaycanca versiya](READMEaz.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)

___

_Tez-tez istifadə edilən Git əmrləri siyahısı_

*Git adlandırmaları ilə maraqlanırsınızsa, `.bash_profile` profilimə burada baxın: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Proyekti əldə etmək və yaratmaq

| Əmr | İzah |
| ------- | ----------- |
| `git init` | Lokal Git reposunu başlat |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Uzaq (remote) reponun lokal kopiyasını yarat |

### Əsas anlıq görüntü

| Əmr | İzah |
| ------- | ----------- |
| `git status` | Statusu yoxla |
| `git add [file-name.txt]` | Hazırlama sahəsinə fayl əlavə et |
| `git add -A` | Hazırlama sahəsinə bütün yeni və dəyişiklik edilmiş faylları əlavə et |
| `git commit -m "[commit message]"` | Dəyişiklikləri icra (commit) et |
| `git rm -r [file-name.txt]` | Fayl (və ya qovluğu) sil |

### Qollara (branch) ayrılma & Birləşmə

| Əmr | İzah |
| ------- | ----------- |
| `git branch` | Branch-lərin siyahısını göstər (ulduz (*) işarəsi cari branch-ı göstərir) |
| `git branch -a` | Bütün branch-ləri (lokal və uzaq) göstər |
| `git branch [branch name]` | Yeni branch yarat |
| `git branch -d [branch name]` | Branch-ı sil |
| `git push origin --delete [branch name]` | Uzaq branch-ı sil |
| `git checkout -b [branch name]` | Yeni branch yarat və ona keçid et |
| `git checkout -b [branch name] origin/[branch name]` | Uzaq branch-ı kopyala (clone) və ona keçid et |
| `git branch -m [old branch name] [new branch name]` | Lokal branch-ın adını dəyiş |
| `git checkout [branch name]` | Branch-a keçid et |
| `git checkout -` | Sonuncu keçid edilmiş branch-a qayıt |
| `git checkout -- [file-name.txt]` | Bir fayldakı dəyişiklikləri sil |
| `git merge [branch name]` | Branch-ı cari branch-a birləşdir |
| `git merge [source branch] [target branch]` | Branch-ı hədəf branch-a birləşdir |
| `git stash` | Yarımçıq qalmış işləmə qovluğundakı dəyişiklikləri saxla |
| `git stash clear` | Bütün saxlanılmış dəyişiklikləri təmizlə |
| `git stash pop` | Sonuncu saxlanılmış dəyişiklikləri cari işləmə qovluğuna əlavə et |

### Proyektləri paylaşmaq və yeniləmək

| Əmr | İzah |
| ------- | ----------- |
| `git push origin [branch name]` | Uzaq repoya branch göndər |
| `git push -u origin [branch name]` | Dəyişiklikləri uzaq repoya (branch-ı yada sal) göndər |
| `git push` | Dəyişiklikləri uzaq repoya (yada salınmış branch-a) göndər |
| `git push origin --delete [branch name]` | Uzaq branch-ı sil |
| `git pull` | Lokal reponu ən yeni commit ilə yenilə |
| `git pull origin [branch name]` | Uzaq repodan dəyişiklikləri çək |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Uzaq repo əlavə et |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Reponun başlanğıc branch-ını SSH olaraq təyin et |

### Yoxlama & Müqayisə

| Əmr | İzah |
| ------- | ----------- |
| `git log` | Dəyişikliklərə bax |
| `git log --summary` | Dəyişikliklərə bax (detallı) |
| `git log --oneline` | Dəyişikliklərə bax (qısa) |
| `git diff [source branch] [target branch]` | Birləşdirmədən əvvəl dəyişiklikləri önizlə |
