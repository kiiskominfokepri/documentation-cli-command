# Rules Commit
## Rules / Peraturan Commit Git by tim KIIS Kominfo Kepri

### add 
Menambahkan Function di File bersangkutan
```
add : `send_message_email` in module_a
```

### create 
Membuat File Baru
```
create : `Send_email.php` in module_a
```

### delete 
menghapus File
```
delete : `Send_notif.php` in module_a
```

### remove 
Menghapus atribut dan fungsi
```
remove : `send_notification` in module_a
```

### update
Mengubah atribut, fungsi 
```
update : `send_notification` in module_a
```

### fix 
Memperbaiki bug
```
fix(bug) : `send_notification` in module_a
```

### feat
Menambahkan fitur
```
feat(delete_message) : `notification` in module_a
```

## Catatan
Jika ada yang salah dan ingin ditambahkan silahkan clone dan push.

### Tambahan
- **(build)** 
Perubahan yang memengaruhi sistem build atau dependensi eksternal (contoh cakupan (scope): gulp, broccoli, npm)
- **(ci)**
Perubahan pada file konfigurasi dan skrip CI kami (contoh cakupan: Circle, BrowserStack, SauceLabs) // Skip
docs: perubahan Dokumentasi
- **(feat)**
Fitur baru
- **(fix)**
Perbaikan bug
- **(perf)**
Perubahan kode yang meningkatkan kinerja
- **(refactor)**
Perubahan kode yang tidak memperbaiki bug atau menambahkan fitur
- **(style)**
Perubahan yang tidak memengaruhi makna kode (white-space, pemformatan, tidak ada titik koma, etc)
- **(test)**
Menambahkan tes yang hilang atau mengoreksi tes yang ada
