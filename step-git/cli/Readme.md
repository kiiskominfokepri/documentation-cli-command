# Langkah-langkah / tutorial menggunakan git

## Langkah Awal

### Langkah Awal ( Download )
- Untuk langkah awal download dan install aplikasi / software git pada link ( [git-scm.com/download](https://git-scm.com/download) )

### Clone project
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
git push -u origin "nama_branch_baru"
``````

## Memulai project dan langkah - langkah utama
Disini akan mulai step / langkah - langkah / perintah - perintah utama yang sering digunakan dalam mengelola sebuah project

### Menambahkan file ke staging
Staging area adalah sebuah file, biasanya berada pada Git directory. File ini akan menyimpan informasi mengenai data mana saja yang akan masuk kedalam commit berikutnya. File ini biasanya disebut “index”, tapi biasa juga disebut staging area.
Perintah yang digunakan adalah 

``````
git add all 
``````

atau 

``````
git add .
``````

atau jika hanya ingin file tertentu dapat menggunakan perintah 

``````
git add index.html
``````

### Membuat Commit / Pesan 
Digunakan untuk menyimpan data beserta pesan apabila terjadi perubahan dan dilakukan pada repository jarak jauh, namun tidak bisa melakukan perubahan. Perintah yang digunakan :

``````
git commit -m "pesan commit"
``````

### Push hasil perubahan pada project ke repository online
Digunakan untuk mengirimkan hasil revisi / perubahan yang sudah dibuat ke repository online
``````
git push origin nama_branch
``````
Keterangan:

- **origin** adalah nama remote.
- **nama_branch** adalah nama cabang / branch tujuan.

## Apa yang terjadi jika kamu menjadi seorang 'main' dalam sebuah project
Di tim KIIS Kominfo Kepri, seorang *Project Manager* bertugas dalam memimpin sebuah project, terkadang juga mempunyai tugas lebih seperti melakukan *merge* project dari semua branch. 

### Langkah-langkah dalam melakukan merge
Jika kamu bertugas sebagai project manager, kamu dapat menerapkan beberapa langkah perintah di bawah ini.

#### Fetch data untuk mengambil 
Untuk melakukan merge dapat memasukkan perintah di bawah ini 

``````
git fetch
``````

#### Perintah merge / menyatukan source dari berbagai branch 
Untuk melakukan merge dapat memasukkan perintah di bawah ini 

``````
git merge "nama_branch_yang_ingin_disatukan"
``````

#### Push ke remote repository
Langkah selanjutnya adalah push hasil merge ke remote repository
``````
git push -u origin main
``````
