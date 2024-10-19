# Cara Membuat Repository
<p>Dalam petunjuk ini, saya akan membahas bagaimana cara membuat repository baru di windows.</p>

## 1 persiapan
siapkan software bernama "git" bisa di download di website resmi https://git-scm.com/downloads

### installasi
jalankan setup git yang didownload dan akan muncul jendela seperti ini :
![jendela install](https://i.imgur.com/4XgxmVL.png)
klik next saja sampai selesai dan install

## 2. Membuat akun Github
<p>Selanjutnya anda harus mempunyai akun github terlebih dahulu, jika anda belum pernah mendaftar, silahkan anda kunjungi website github.com lalu buat akun github</p>

### buat repository.
klik tombol "+" pada sudut kanan atas halaman web lalu klik "new repository"
![menambah repository](https://i.imgur.com/MqIEA8T.png)
maka akan mucul halaman di bawah ini :
![halaman penambahan repository](https://i.imgur.com/1LjVRDn.png)
isi nama repository sesuai keinginan anda lalu klik "create repository"

## 3 cara menggunakan git
buka software "git bash" yang sudah di install tadi, lalu ketikkan command line di bawah ini :
```
$ git config --global user.name "username yg anda buat di github"
$ git config --global user.email "email yg anda pakai untuk github"
```
contohnya seperti ini:
![contoh 1](https://i.imgur.com/IFNts3y.png)
lalu ketik command:
```
$ git config --list
```
maka akan muncul seperti ini:
![contoh 2](https://i.imgur.com/xnbhA8C.png)
jika username dan email terisi sesuai yg anda ketik berarti berhasil
lalu buat folder untuk tempat menyimpan repository local di komputer anda dengan cara buat new folder di tempat yg anda suka contohnya:
![contoh 3](https://i.imgur.com/aQqxl60.png)
saya membuat folder "latihanvcs" di drive D
lalu klik kanan dan pilih "git bash here"
lalu ketik command:
```
$ git init
```
Lalu masukan perintah berikut untuk membuat file "readme.md"
```
$ echo "# Latihan1" >> readme.md
```
lalu ketik :
```
$ git add readme.md
```
setelah itu commit dengan cara :
```
$ git commit -m "komentar"
```
contohnya seperti ini:
![contoh 4](https://i.imgur.com/vDyzNN2.png)
lalu ketik:
```
$ git remote add origin "link url repository di github"
```
contoh bisa dilihat di gambar sebelumnya
untuk mendapatkan link repository yg anda buat anda tinggal ke akun github anda
klik repository yg anda buat
![contoh 5](https://i.imgur.com/mHEcVq5.png)
lalu klik klik clone or download
![contoh 6](https://i.imgur.com/52fWijn.png)
lalu ketik :
```
$ git push -u origin master
```
lalu anda akan diminta username dan password untuk login ke github anda dan selamat repository anda berhasil di isi (upload) dengan file readme.md silahkan cek repository anda di github dan anda akan melihat perubahan yg tadinya kosong menjadi berisi file readme.md
