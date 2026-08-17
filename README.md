# Planner Jadwal — S1 Teknik Mesin ITS ⚙️📅

Aplikasi web interaktif *single-page* untuk membantu mahasiswa S1 Teknik Mesin ITS dalam merencanakan, menyusun, dan memvisualisasikan jadwal kuliah mingguan dengan mudah dan efisien.

👉 **[Live Demo / Akses Aplikasi](https://thaliban04.github.io/planner-jadwal/)**

---

## ✨ Fitur Utama

- **Peta Slot Interaktif**: Visualisasi jadwal layaknya kalender mingguan. Anda dapat langsung melihat bentrok waktu antar kelas.
- **Katalog Terpadu (Semester 1–8)**: Memuat seluruh daftar mata kuliah S1 Teknik Mesin ITS dengan pemisahan jelas antara Mata Kuliah Wajib dan Mata Kuliah Pilihan.
- **Validasi SKS & Pilihan Cerdas**:
  - Pelacakan jumlah total SKS yang diambil.
  - Memastikan distribusi SKS Mata Kuliah Pilihan tercapai sesuai kurikulum (contoh: proporsi 1 banding 3 antar semester).
- **Responsive Design**: Tampilan yang mulus dan elegan baik di Desktop (Grid View) maupun di Smartphone (List View).
- **Export & Cetak**: 
  - Salin jadwal dalam format teks yang rapi ke Clipboard (siap di-paste ke WhatsApp/Line).
  - Mode cetak khusus (*Print*) untuk menyimpan jadwal dalam format PDF atau kertas.
- **Data Tersimpan Lokal**: Jadwal tersimpan otomatis di dalam *browser* (menggunakan `localStorage`), tidak ada data yang dikirim ke server.

---

## 🛠 Teknologi yang Digunakan

Aplikasi ini dikembangkan murni menggunakan teknologi web fundamental (*Vanilla*), sehingga sangat cepat, ringan, dan gratis di-*hosting*:
- **HTML5** untuk struktur semantik.
- **CSS3 (Vanilla)** untuk sistem *styling* berbasis variabel (Custom Properties), desain responsif, dan animasi transisi yang mulus.
- **JavaScript (ES6)** untuk manajemen *state*, DOM interaktif, dan fungsionalitas logika kurikulum.

---

## 🚀 Panduan Penggunaan Lokal (Development)

Bagi Anda yang ingin memodifikasi atau mengembangkan aplikasi ini secara lokal:

1. **Clone Repository**
   ```bash
   git clone https://github.com/thaliban04/planner-jadwal.git
   cd planner-jadwal
   ```
2. **Jalankan Aplikasi**
   Karena tidak menggunakan *backend* atau *build-tools*, Anda cukup membuka file `index.html` langsung ke *browser* Anda:
   ```bash
   # Pengguna Mac:
   open index.html
   ```
3. **Modifikasi Data Matkul**
   Semua jadwal bawaan dan logika rendering disimpan di dalam blok `<script>` pada file `index.html`. Cari variabel `BUILTIN_SCHEDULES` dan `CATALOG` untuk menambahkan atau mengubah data kelas per semester.

---

## 🔄 Pembaruan & Deployment

Aplikasi ini di-*hosting* secara gratis menggunakan **GitHub Pages**. Setiap kali ada pembaruan kode, Anda cukup melakukan *commit* dan *push* ke *branch* utama (`main`), maka GitHub Pages akan otomatis memperbarui situs web dalam waktu 1-2 menit.

```bash
git add .
git commit -m "Update jadwal semester baru"
git push
```

---

Dibuat untuk mempermudah penyusunan KRS mahasiswa Teknik Mesin ITS.
