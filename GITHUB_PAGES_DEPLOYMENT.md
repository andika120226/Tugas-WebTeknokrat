# 🚀 Panduan Deployment ke GitHub Pages

## Status Deployment

✅ Repository sudah terhubung ke GitHub  
✅ Semua file sudah di-push ke branch `main`  
✅ File `index.html` sudah ada di root directory  
✅ Siap untuk di-deploy ke GitHub Pages

---

## 📋 Langkah-langkah Aktivasi GitHub Pages

### 1. Buka Repository di GitHub

Kunjungi: https://github.com/andika120226/Tugas-WebTeknokrat

### 2. Masuk ke Settings

- Klik tab **"Settings"** di bagian atas repository
- Scroll ke bawah di sidebar kiri

### 3. Klik Menu "Pages"

- Di sidebar kiri, cari dan klik **"Pages"**
- Anda akan masuk ke halaman GitHub Pages settings

### 4. Konfigurasi Source

Di bagian **"Build and deployment"**:

- **Source**: Deploy from a branch
- **Branch**: Pilih `main`
- **Folder**: Pilih `/ (root)`
- Klik tombol **"Save"**

### 5. Tunggu Proses Deployment

- GitHub akan mulai men-deploy website Anda
- Proses biasanya memakan waktu 2-5 menit
- Anda akan melihat URL website di bagian atas halaman

### 6. Akses Website Anda

Setelah selesai, website dapat diakses di:

```
https://andika120226.github.io/Tugas-WebTeknokrat/
```

---

## 🌐 Daftar Halaman yang Dapat Diakses

Setelah deployment berhasil, semua halaman berikut dapat diakses:

### Halaman Utama

- **Home**: `https://andika120226.github.io/Tugas-WebTeknokrat/`
- **Home Page**: `https://andika120226.github.io/Tugas-WebTeknokrat/Home.html`
- **Profil**: `https://andika120226.github.io/Tugas-WebTeknokrat/Profil.html`
- **History**: `https://andika120226.github.io/Tugas-WebTeknokrat/History.html`
- **Facility**: `https://andika120226.github.io/Tugas-WebTeknokrat/Facility.html`
- **SDGs**: `https://andika120226.github.io/Tugas-WebTeknokrat/SDGs.html`
- **Organizational Structure**: `https://andika120226.github.io/Tugas-WebTeknokrat/OrganizationalStructure.html`

### Admission & Registration

- **Admission**: `https://andika120226.github.io/Tugas-WebTeknokrat/Admission.html`
- **Admission Complete**: `https://andika120226.github.io/Tugas-WebTeknokrat/Admission_Complete.html`
- **Admission New**: `https://andika120226.github.io/Tugas-WebTeknokrat/Admission_new.html`
- **Online Application Form**: `https://andika120226.github.io/Tugas-WebTeknokrat/OnlineApplicationForm.html`
- **Scholarship**: `https://andika120226.github.io/Tugas-WebTeknokrat/Scholarship.html`

### Academic Programs

- **Academic**: `https://andika120226.github.io/Tugas-WebTeknokrat/Academic.html`
- **CPL**: `https://andika120226.github.io/Tugas-WebTeknokrat/CPL.html`
- **PPM**: `https://andika120226.github.io/Tugas-WebTeknokrat/PPM.html`
- **Download Files**: `https://andika120226.github.io/Tugas-WebTeknokrat/DownloadFiles.html`

### Student Affairs

- **Student Affairs**: `https://andika120226.github.io/Tugas-WebTeknokrat/StudentAffairs.html`
- **Student Affairs New**: `https://andika120226.github.io/Tugas-WebTeknokrat/StudentAffairs_New.html`

### Documentation

- **Reference Guide**: `https://andika120226.github.io/Tugas-WebTeknokrat/REFERENCE_GUIDE.html`

---

## 🔄 Update Website (Push Changes)

Setiap kali Anda melakukan perubahan pada file, ikuti langkah berikut:

### 1. Tambahkan File yang Berubah

```powershell
git add .
```

### 2. Commit Perubahan

```powershell
git commit -m "Deskripsi perubahan Anda"
```

### 3. Push ke GitHub

```powershell
git push origin main
```

### 4. Tunggu Auto-Deploy

- GitHub Pages akan otomatis mendeteksi perubahan
- Website akan ter-update dalam 1-3 menit
- Tidak perlu konfigurasi ulang

---

## ✅ Verifikasi Deployment

### Cek Status Deployment

1. Buka repository di GitHub
2. Klik tab **"Actions"**
3. Lihat workflow **"pages build and deployment"**
4. Status hijau ✅ = berhasil
5. Status merah ❌ = ada error

### Test Halaman

Buka beberapa halaman untuk memastikan semuanya berfungsi:

- ✅ Index page loading dengan benar
- ✅ Navigasi antar halaman berfungsi
- ✅ CSS dan styling ter-load dengan baik
- ✅ Gambar tampil dengan sempurna
- ✅ JavaScript berfungsi (untuk halaman interaktif)

---

## 🎯 Tips & Troubleshooting

### Jika Halaman 404 Not Found

- Pastikan nama file **case-sensitive** (contoh: `Home.html` bukan `home.html`)
- Verifikasi file berada di root directory atau path yang benar
- Clear cache browser (Ctrl+Shift+Delete)

### Jika CSS/JS Tidak Loading

- Periksa path relatif di HTML
- Pastikan file CSS/JS ada di repository
- Gunakan path relatif, bukan absolute

### Jika Gambar Tidak Tampil

- Verifikasi path gambar: `Kumpulan foto/nama-file.jpg`
- Pastikan nama file gambar sama persis (termasuk case)
- Cek ekstensi file (.jpg, .png, .jpeg, dll)

### Jika Update Tidak Muncul

- Tunggu 1-3 menit setelah push
- Hard refresh browser (Ctrl+F5)
- Clear cache browser
- Cek tab Actions untuk status deployment

---

## 📱 Custom Domain (Opsional)

Jika ingin menggunakan domain sendiri:

### 1. Beli Domain

Beli domain dari provider seperti:

- Niagahoster
- Domainesia
- GoDaddy
- Namecheap

### 2. Konfigurasi DNS

Tambahkan DNS record:

```
Type: CNAME
Name: www
Value: andika120226.github.io
```

### 3. Setting di GitHub

1. Buka Settings → Pages
2. Di bagian "Custom domain"
3. Masukkan domain Anda
4. Klik "Save"
5. Tunggu DNS propagation (24-48 jam)

---

## 📊 Monitoring & Analytics

### Google Analytics (Opsional)

Untuk tracking visitor, tambahkan Google Analytics:

1. Buat akun di https://analytics.google.com
2. Dapatkan tracking code
3. Tambahkan ke semua file HTML sebelum `</head>`:

```html
<!-- Google Analytics -->
<script
  async
  src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"
></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag() {
    dataLayer.push(arguments);
  }
  gtag("js", new Date());
  gtag("config", "GA_MEASUREMENT_ID");
</script>
```

---

## 🎉 Selamat!

Website Anda sekarang **LIVE** dan dapat diakses oleh siapa saja di internet!

**URL Website**: https://andika120226.github.io/Tugas-WebTeknokrat/

### Bagikan Link Anda:

- Social Media
- Email signature
- Business cards
- LinkedIn profile
- Portfolio

---

## 📞 Support

Jika ada pertanyaan atau masalah:

1. Cek dokumentasi GitHub Pages: https://pages.github.com/
2. Baca file troubleshooting di repository
3. Lihat tab Issues di repository GitHub

---

**Last Updated**: January 2, 2026  
**Status**: ✅ Ready for Production  
**Repository**: https://github.com/andika120226/Tugas-WebTeknokrat
