# 🚀 Panduan Git & GitHub untuk Project Tugas Web Teknokrat

## ✅ Status Saat Ini

Repository Git sudah diinisialisasi dan terhubung ke:

```
https://github.com/andika120226/Tugas-WebTeknokrat.git
```

## 📝 Perintah Git yang Sudah Dijalankan

```bash
# 1. Inisialisasi repository
git init

# 2. Menambahkan semua file ke staging
git add .

# 3. Commit pertama
git commit -m "first commit"

# 4. Mengubah branch menjadi main
git branch -M main

# 5. Menambahkan remote repository
git remote add origin https://github.com/andika120226/Tugas-WebTeknokrat.git

# 6. Push ke GitHub
git push -u origin main
```

## 🔄 Workflow Git untuk Update Selanjutnya

### Setiap kali ada perubahan:

```bash
# 1. Cek status file yang berubah
git status

# 2. Tambahkan file yang diubah
git add .
# atau spesifik file:
git add html/Home.html
git add home-styles.css

# 3. Commit dengan pesan yang jelas
git commit -m "Pesan commit yang deskriptif"

# Contoh pesan commit yang baik:
git commit -m "Add contact section to home page"
git commit -m "Fix responsive layout on mobile"
git commit -m "Update hero banner styling"

# 4. Push ke GitHub
git push origin main
```

## 📋 Perintah Git yang Berguna

### Melihat Status

```bash
# Lihat file yang dimodifikasi
git status

# Lihat history commit
git log

# Lihat history commit singkat
git log --oneline

# Lihat perubahan yang belum di-commit
git diff
```

### Mengelola Remote

```bash
# Lihat remote yang terhubung
git remote -v

# Ubah URL remote
git remote set-url origin <URL-BARU>

# Hapus remote
git remote remove origin
```

### Branch Management

```bash
# Lihat semua branch
git branch

# Buat branch baru
git branch <nama-branch>

# Pindah ke branch lain
git checkout <nama-branch>

# Buat dan pindah ke branch baru
git checkout -b <nama-branch>

# Merge branch
git merge <nama-branch>
```

### Undo Changes

```bash
# Undo perubahan pada file (sebelum add)
git checkout -- <namafile>

# Unstage file (setelah add, sebelum commit)
git reset HEAD <namafile>

# Undo commit terakhir (keep changes)
git reset --soft HEAD~1

# Undo commit terakhir (discard changes)
git reset --hard HEAD~1
```

## 🌿 Workflow dengan Branch

Untuk development yang lebih terstruktur:

```bash
# 1. Buat branch untuk fitur baru
git checkout -b feature/new-page

# 2. Kerjakan perubahan
# ... edit files ...

# 3. Commit di branch
git add .
git commit -m "Add new page"

# 4. Push branch ke GitHub
git push origin feature/new-page

# 5. Kembali ke main
git checkout main

# 6. Merge branch
git merge feature/new-page

# 7. Push main
git push origin main

# 8. Hapus branch (optional)
git branch -d feature/new-page
```

## 🔍 Melihat Project di GitHub

Setelah push berhasil, akses:

```
https://github.com/andika120226/Tugas-WebTeknokrat
```

## 📦 Clone Repository (untuk komputer lain)

```bash
# Clone ke komputer lain
git clone https://github.com/andika120226/Tugas-WebTeknokrat.git

# Masuk ke folder
cd Tugas-WebTeknokrat

# Mulai bekerja
```

## 🚨 Troubleshooting

### Problem: Remote already exists

```bash
git remote remove origin
git remote add origin <URL>
```

### Problem: Push rejected

```bash
# Pull dulu sebelum push
git pull origin main --rebase
git push origin main
```

### Problem: Merge conflict

```bash
# Edit file yang conflict
# Hapus marker <<<<, ====, >>>>
git add <file-yang-conflict>
git commit -m "Resolve conflict"
git push origin main
```

### Problem: File terlalu besar

```bash
# Tambahkan ke .gitignore
echo "file-besar.zip" >> .gitignore
git rm --cached file-besar.zip
git commit -m "Remove large file"
git push origin main
```

## 📝 Best Practices

### Commit Messages

✅ **Good:**

- "Add footer section to home page"
- "Fix responsive navbar on mobile"
- "Update hero banner background"

❌ **Bad:**

- "update"
- "fix"
- "asdfgh"

### Commit Frequency

- Commit setiap kali menyelesaikan satu fitur/perbaikan
- Jangan commit terlalu jarang (kehilangan history)
- Jangan commit terlalu sering (history berantakan)

### .gitignore

Sudah dibuat file `.gitignore` untuk mengabaikan:

- IDE folders (.vscode, .idea)
- OS files (Thumbs.db, .DS_Store)
- Temporary files (_.tmp, _.log)
- Node modules (jika ada)

## 🎯 Next Steps

1. ✅ **Verifikasi Upload**

   - Buka https://github.com/andika120226/Tugas-WebTeknokrat
   - Pastikan semua file terupload

2. ✅ **Update README**

   - Edit README.md di GitHub
   - Tambahkan screenshot
   - Tambahkan demo link (jika di-deploy)

3. ✅ **Enable GitHub Pages** (Optional)

   - Settings → Pages
   - Source: Deploy from branch → main
   - Folder: / (root) atau /html
   - Save
   - Website akan available di: https://andika120226.github.io/Tugas-WebTeknokrat/

4. ✅ **Add License** (Optional)
   - Add file → Create new file
   - Name: LICENSE
   - Choose license template (MIT recommended)

## 🌐 Deploy ke GitHub Pages

Untuk membuat website live:

1. **Via GitHub Website:**

   - Masuk ke repository
   - Settings → Pages
   - Source: main branch
   - Folder: /html (karena HTML ada di folder html)
   - Save

2. **Update index.html di root:**

```bash
# Copy Home.html ke root sebagai index.html
cp html/Home.html index.html
# Ubah semua path relatif di index.html
# ../eksternal.css → eksternal.css
# ../ext/logo.png → ext/logo.png
```

## 📞 Support

Jika ada masalah:

1. Cek dokumentasi Git: https://git-scm.com/doc
2. GitHub Docs: https://docs.github.com/
3. Stack Overflow: https://stackoverflow.com/questions/tagged/git

---

**Happy Coding! 🚀**

_Last Updated: 2 Januari 2026_
