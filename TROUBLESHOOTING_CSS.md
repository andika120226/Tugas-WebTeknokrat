# PANDUAN TROUBLESHOOTING CSS - Home.html

## Masalah yang Telah Diperbaiki:

1. ✅ Path CSS sudah benar: `../eksternal.css`, `../style-hero.css`, `../home-styles.css`
2. ✅ File CSS sudah diverifikasi ada di lokasi yang benar
3. ✅ Ditambahkan cache-busting dengan parameter `?v=1.0`
4. ✅ Ditambahkan critical inline CSS untuk tampilan dasar
5. ✅ Ditambahkan script debug untuk memonitor loading CSS

## Cara Melihat Halaman dengan CSS yang Benar:

### LANGKAH 1: HARD REFRESH Browser

Buka file `Home.html` di browser, lalu tekan:

- **Windows/Linux**: `Ctrl + Shift + R` atau `Ctrl + F5`
- **Mac**: `Cmd + Shift + R`

### LANGKAH 2: Bersihkan Cache Browser

Jika masih tidak muncul:

1. Tekan `F12` untuk membuka Developer Tools
2. Klik kanan pada tombol Refresh browser
3. Pilih "Empty Cache and Hard Reload"

### LANGKAH 3: Cek Console untuk Debug

1. Buka Developer Tools (F12)
2. Buka tab "Console"
3. Anda akan melihat log:
   - "Page loaded"
   - "Stylesheets: X" (jumlah stylesheet)
   - Path dari setiap stylesheet

### LANGKAH 4: Cek Network Tab

1. Buka Developer Tools (F12)
2. Buka tab "Network"
3. Refresh halaman (Ctrl + Shift + R)
4. Cari file CSS:
   - `eksternal.css` - harus status 200
   - `style-hero.css` - harus status 200
   - `home-styles.css` - harus status 200
5. Jika status 404, berarti path salah

## Verifikasi CSS Berfungsi:

Jika CSS dimuat dengan benar, Anda akan melihat:

- ✅ Menu navigasi horizontal dengan background gradient biru
- ✅ Hero banner dengan background gradient biru gelap
- ✅ Font Poppins pada semua teks
- ✅ Stat cards dengan icon dan styling
- ✅ Layout responsive dan modern

## File Test Tersedia:

File `test.html` sudah dibuat di folder yang sama untuk testing sederhana.
Buka file ini untuk memverifikasi CSS dasar bekerja.

## Troubleshooting Tambahan:

### Jika CSS masih tidak muncul:

1. Pastikan file dibuka dari file explorer, bukan dari dalam VS Code
2. Coba browser lain (Chrome, Firefox, Edge)
3. Pastikan path relatif benar dengan cek di console

### Jika hanya sebagian CSS yang muncul:

1. Cek apakah ada error di console
2. Cek apakah font Google berhasil dimuat (perlu koneksi internet)
3. Cek apakah file logo.png ada di folder ../ext/

---

## Status Perbaikan: ✅ SELESAI

Semua file CSS sudah diperbaiki dan diverifikasi.
Silakan refresh browser Anda dengan Ctrl + Shift + R.
