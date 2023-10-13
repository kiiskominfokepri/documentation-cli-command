# Langkah-langkah / tutorial menggunakan git

### Langkah Awal ( Download )
- Untuk langkah awal download dan install aplikasi / software git pada link ( [git-scm.com/download](https://git-scm.com/download) )

### Langkah clone dan proses langkah utama
- Untuk mengambil project, silahkan cari repository di tempat dimana kamu menyimpan / mengambil project. Untuk contoh yang digunakan.

``````
https://github.com/kiiskominfokepri/documentation-cli-command.git
`````` 
atau jika menggunakan SSH
``````
git@github.com:kiiskominfokepri/documentation-cli-command.git
``````

Kode diatas dapat ditemukan pada tombol **<> Code**

- Jika sudah ter-clone, langkah selanjutnya kamu dapat meng-**fetch** Data agar data kamu dapat tersinkronasi file project local kamu dengan project online. Dengan Perintah

``````
git fetch
``````
- Maka project dan branch pada local sudah tersinkronasi dengan remote project

### Membuat Branch Baru
Kamu dapat membuat branch baru jika pada project yang kamu ambil belum memiliki branch yang diperuntukkan untuk kamu. 
- Sebelum memulai membuat branch kamu dapat memeriksa daftar branch yang ada di local project kamu dengan memasukkan perintah :

``````
git branch --list
``````
branch yang aktif saat ini disorot dengan tanda bintang '*' Dalam contoh diatas adalah branch master.

- Di Git, branch lokal dan remote branch adalah objek yang terpisah. Jika Anda ingin mendaftar branch lokal dan remote, tambahkan opsi -a:

``````
git branch -a
``````

- Untuk membuat sebuah branch baru kamu dapat memasukkan perintah 

``````
git checkout -b "nama_branch_baru"
``````

- Dan untuk sinkronasi / push kamu dapat menggunakan perintah

``````
git checkout -b "nama_branch_baru"
``````
