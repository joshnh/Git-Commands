Perintah-Perintah Git
============

## Versi Terjemahan
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [Bahasa Indonesia](READMEid.md)

___

_Daftar perintah Git yang biasa aku gunakan_

*Jika kamu tertarik dengan Git aliasku, silahkan lihat `.bash_profile` ku, disini: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Memulai dan Membuat Proyek

| Perintah | Deskripsi |
| ------- | ----------- |
| `git init` | Inisialisasi repositori Git lokal |
| `git clone ssh://git@github.com/[username]/[nama-repository].git` | Buat salinan lokal dari repository luar |

### Dasar Melakukan Snapshot

| Perintah | Deskripsi |
| ------- | ----------- |
| `git status` | Cek status |
| `git add [nama-file.txt]` | Tambahkan sebuah file ke area staging |
| `git add -A` | Tambahkan semua file baru dan file yang berubah ke area staging |
| `git commit -m "[pesan commit]"` | Lakukan commit perubahan |
| `git rm -r [nama-file.txt]` | Menghapus sebuah file atau folder |

### Percabangan dan Penggabungan

| Perintah | Deskripsi |
| ------- | ----------- |
| `git branch` | Daftar branch (bintang menandai branch saat ini) |
| `git branch -a` | Daftar semua branch (lokal dan luar) |
| `git branch [nama branch]` | Membuat sebuah branch baru |
| `git branch -d [nama branch]` | Menghapus sebuah branch |
| `git push origin --delete [nama branch]` | Menghapus sebuah branch luar |
| `git checkout -b [nama branch]` | Membuat sebuah branch baru lalu berpindah ke branch tersebut |
| `git checkout -b [nama branch] origin/[nama branch]` | Klon sebuah branch luar lalu berpindah ke branch tersebut |
| `git branch -m [nama branch sebelum] [nama branch baru]` | Mengubah nama sebuah branch lokal |
| `git checkout [nama branch]` | Berpindah ke sebuah branch |
| `git checkout -` | Berpindah ke branch terakhir kali dikunjungi |
| `git checkout -- [nama-file.txt]` | Membuang perubahan ke sebuah file |
| `git merge [nama branch]` | Menggabungkan sebuah branch ke branch yang aktif |
| `git merge [branch sumber] [branch tujuan]` | Menggabungkan sebuah branch ke branch yang dituju |
| `git stash` | Simpan perubahan (stash) dari direktori kerja saat ini |
| `git stash clear` | Hapus semua perubahan (stash) yang tersimpan |

### Berbagi dan Pembaruan Proyek

| Perintah | Deskripsi |
| ------- | ----------- |
| `git push origin [nama branch]` | Mengunggah sebuah branch ke repositori luar |
| `git push -u origin [nama branch]` | Mengunggah perubahan ke repositori luar (dan mengingat branch tersebut) |
| `git push` | Mengunggah perubahan ke repositori luar (dari branch yang sudah diingat) |
| `git push origin --delete [nama branch]` | Menghapus sebuah branch dari repositori luar |
| `git pull` | Memperbarui repositori lokal dengan commit terbaru |
| `git pull origin [nama branch]` | Menarik perubahan dari branch luar |
| `git remote add origin ssh://git@github.com/[username]/[nama-repositori].git` | Menambahkan sebuah branch luar |
| `git remote set-url origin ssh://git@github.com/[username]/[nama-repositori].git` | Mengubah url repositori luar menggunakan SSH |

### Inspeksi dan Pembadingan

| Perintah | Deskripsi |
| ------- | ----------- |
| `git log` | Lihat log |
| `git log --summary` | Lihat log (secara lengkap) |
| `git log --oneline` | Lihat log (secara ringkasan) |
| `git diff [branch sumber] [branch tujuan]` | Pratinjau perubahan sebelum melakukan merging |
