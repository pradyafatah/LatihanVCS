# Cara Membuat Repository
<p>Dalam petunjuk ini, saya akan membahas bagaimana cara membuat repository baru di windows.</p>

## 1 persiapan
siapkan software bernama "git" bisa di download di website resmi https://git-scm.com/downloads

### installasi
jalankan setup git yang didownload dan akan muncul jendela seperti ini :
![jendela install](![git - Imgur](https://github.com/user-attachments/assets/cd8788bc-d93c-4aa8-bbdc-b45a4f77931e))
klik next saja sampai selesai dan install

## 2. Membuat akun Github
<p>Selanjutnya anda harus mempunyai akun github terlebih dahulu, jika anda belum pernah mendaftar, silahkan anda kunjungi website github.com lalu buat akun github</p>

### buat repository.
klik tombol "+" pada sudut kanan atas halaman web lalu klik "new repository"
![menambah repository](https://i.imgur.com/MqIEA8T.png)
maka akan mucul halaman di bawah ini :
![halaman penambahan repository](![home - Imgur](https://github.com/user-attachments/assets/f1e764ae-925c-4982-9b85-29a78282aebe)
)
isi nama repository sesuai keinginan anda lalu klik "create repository"

## 3 cara menggunakan git
buka software "git bash" yang sudah di install tadi, lalu ketikkan command line di bawah ini :
```
$ git config --global user.name "username yg anda buat di github"
$ git config --global user.email "email yg anda pakai untuk github"
```
contohnya seperti ini:
![contoh 1](![undefined - Imgur](https://github.com/user-attachments/assets/253c8ba6-1bf6-40b6-9585-728c5b10b280))
lalu ketik command:
```
$ git config --list
```
maka akan muncul seperti ini:
![contoh 2](![git - Imgur (1)](https://github.com/user-attachments/assets/387411e9-e20a-4f71-ac8c-6fb6b25cf133))


jika username dan email terisi sesuai yg anda ketik berarti berhasil
lalu buat folder untuk tempat menyimpan repository local di komputer anda dengan cara buat new folder di tempat yg anda suka contohnya:
![contoh 3](![gitt - Imgur](https://github.com/user-attachments/assets/f0958cc4-f3ce-46d0-9c25-1bd673c54ee8))

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
![contoh 4](![git - Imgur (3)](https://github.com/user-attachments/assets/5e0ac3bb-5ad1-45cb-b70e-3bff8e8b2b67))

lalu ketik:
```
$ git remote add origin "link url repository di github"
```
contoh bisa dilihat di gambar sebelumnya
untuk mendapatkan link repository yg anda buat anda tinggal ke akun github anda
klik repository yg anda buat
![contoh 5](![posting - Imgur](https://github.com/user-attachments/assets/b644f4b0-4ca7-4434-8541-78957319fbd7))


lalu klik klik copy or download
![contoh 6](![copy or download - Imgur](https://github.com/user-attachments/assets/def8c62e-fa57-42ce-ba7c-3ec6087a0db3))


lalu ketik :
```
$ git push -u origin master
```
lalu anda akan diminta username dan password untuk login ke github anda dan selamat repository anda berhasil di isi (upload) dengan file readme.md silahkan cek repository anda di github dan anda akan melihat perubahan yg tadinya kosong menjadi berisi file readme.md
