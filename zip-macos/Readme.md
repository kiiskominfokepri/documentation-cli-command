# Membuat file .zip di MacOS

### Membuat file .zip di MacOS tanpa membawa .DS_Store dan folder __MACOSX
Perintah : 
```
zip -r nama_file.zip folder_tujuan -x "*.DS_Store" -x "__MACOSX" -x ".git"
```
