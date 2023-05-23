# Migrasi dari GitLab ke GitHub

1. Hapus Remote dengan GitLab
```
git remote remove origin
```

2. Ambil link remote dari GitHub dan tambahkan remote
```
git remote add origin https://github.com/kiiskominfokepri/nama-repo.git
```

3. Sync repo lokal dengan GitHub
```
git push --all origin
```