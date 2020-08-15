GitHub Terminal Kısayolları
============

Sık kullanılan GitHub kısayollarının listesi, hem de Türkçe!

<br/>

## Translated Versions
- [English](https://github.com/joshnh/Git-Commands/blob/master/README.md)
- [Português](https://github.com/vali-kh/Git-Commands/blob/master/READMEpt.md)

<!-- ___ -->
<br/>



### Proje Yönetimi

| Komut | Açıklama |
| ------- | ----------- |
| `git init` | Yeni bir yerel Git deposu oluştur |
| `git clone https://github.com/[username]/[repo_name].git` | Sunucudaki deponun yerel bir klonunu oluştur |

<br/>

### Sürüm / Değişiklik Yönetimi

| Komut | Açıklama |
| ------- | ----------- |
| `git status` | Yerel deponun durumunu kontrol et |
| `git add [filename.txt]` | Belirli bir dosyayı (ya da klasörü) evreleme alanına ekle |
| `git add .` | Tüm yeni ve değiştirilmiş dosyaları evreleme alanına ekle (silinenler eklenmez) |
| `git add -u` | Tüm silinen ve değiştirilmiş dosyaları evreleme alanına ekle (yeniler eklenmez) |
| `git add -A` | Tüm dosyaları evreleme alanına ekle (üstteki iki komutun toplu hali) |
| `git reset` | Evreleme alanını komple temizle |
| `git restore --staged [filename.txt]` | Belirli bir dosyayı (ya da klasörü) evreleme alanından çıkar |
| `git commit -m "[commit_message]"` | Evreleme alnındaki dosyaların değişiklikleri bir mesaj ile kayıt defterine işle |

<br/>

### Branş Yönetimi

| Komut | Açıklama |
| ------- | ----------- |
| `git branch` | Tüm yerel branşları listele |
| `git branch -a` | Tüm yerel ve sunucudaki branşları listele |
| `git branch [branch_name]` | Yeni bir branş oluştur |
| `git branch -d [branch_name]` | Yerel bir branşı sil |
| `git push origin --delete [branch_name]` | Sunucudaki branşı sil |
| `git checkout -b [branch_name]` | Yeni bir branş oluştur ve ona geçiş yap |
| `git checkout -b [branch_name] origin/[branch_name]` | Sunucudaki bir branşı klonla ve ona geçiş yap |
| `git branch -m [old_branch_name] [new_branch_name]` | Bir branşı yeniden adlandır |
| `git checkout [branch_name]` | Başka bir branşa geçiş yap |
| `git checkout -- .` | Branştaki tüm değişiklikleri temizle (ve kayıt defterindeki son halini geri yükle) |
| `git checkout -- [filename.txt]` | Branştaki bir dosyadaki değişiklikleri temizle (ve kayıt defterindeki son halini geri yükle) |
| `git merge [branch_name]` | Başka bir branşı, şu an bulunulan branş ile birleştir |
| `git merge [source-branch] [target-branch]` | İki farklı branşı birleştir |

<br/>

### Kirli Saklama Yöntemleri

| Komut | Açıklama |
| ------- | ----------- |
| `git stash` | Değişikleri branş dışında sakla (ve branştaki değişiklikleri temizle) |
| `git stash list` | Saklanan tüm değişiklikleri göster |
| `git stash apply` | En son saklanan değişikliği bulunulan branşa aktar |
| `git stash apply stash@{stash_index}` | Seçilen bir saklanan değişikliği bulunulan branşa aktar |
| `git stash pop stash@{stash_index}` | Seçilen bir saklanan değişikliği bulunulan branşa aktar, ve ardından listeden temizle |
| `git stash clear` | Saklanan tüm değişiklikleri temizle |

<br/>

### Depo Paylaşım & Güncellemesi

| Komut | Açıklama |
| ------- | ----------- |
| `git push origin [branch_name]` | Branşı sunucudaki depoya itele |
| `git push -u origin [branch_name]` | Branşı sunucudaki depoya itele (ve branşı hatırla) |
| `git push` | Branşı sunucudaki depoya itele (hatırlanan branş için) |
| `git pull` | Sunucudaki en son değişiklikleri yerel depoya çek |
| `git pull origin [branch_name]` | Sunucudaki değişiklikleri branşa çek |
| `git remote add origin https://github.com/[username]/[repo_name].git` | Sunucuda yeni bir depo oluştur |
| `git remote set-url origin ssh://git@github.com/[username]/[repository_name].git` | Deponun sunucudaki branşını SSH olarak ayarla |

<br/>

### Kayıt Defteri & Kıyaslama

| Komut | Açıklama |
| ------- | ----------- |
| `git log` | Kayıttaki tüm değişikleri göster |
| `git log --oneline` | Kayıttaki tüm değişikleri göster (tek satırlık özet halinde) |
| `git diff [source_branch] [target_branch]` | İki branş arasındakı farkı göster |

