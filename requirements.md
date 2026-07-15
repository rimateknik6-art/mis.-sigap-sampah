# Kebutuhan Sistem (Requirements)

## 1. Kebutuhan Fungsional

| ID | Kebutuhan | Aktor |
|---|---|---|
| F-01 | Sistem dapat menampilkan formulir pelaporan sampah (nama, RT, lokasi, jenis sampah, deskripsi) | Warga |
| F-02 | Sistem menyimpan setiap laporan dengan status awal "Menunggu" | Sistem |
| F-03 | Sistem menampilkan daftar jadwal pengangkutan sampah per RT (hari, jam, rute) | Warga |
| F-04 | Sistem menampilkan ringkasan statistik (total laporan, laporan selesai, laporan menunggu) | Warga/Admin |
| F-05 | Admin dapat melihat seluruh laporan warga secara lengkap | Admin (Pengurus RT/RW) |
| F-06 | Admin dapat mengubah status laporan (Menunggu / Diproses / Selesai) | Admin |
| F-07 | Admin dapat menambahkan jadwal pengangkutan baru per RT | Admin |
| F-08 | Admin dapat menghapus jadwal yang sudah tidak berlaku | Admin |

## 2. Kebutuhan Non-Fungsional

| ID | Kebutuhan | Keterangan |
|---|---|---|
| NF-01 | Usability | Antarmuka sederhana, mudah dipahami warga dari berbagai usia |
| NF-02 | Responsif | Tampilan dapat diakses baik dari desktop maupun mobile |
| NF-03 | Performa | Perubahan data (submit laporan, update status) langsung terlihat tanpa reload halaman |
| NF-04 | Portabilitas | Berjalan sebagai aplikasi web statis tanpa instalasi khusus di sisi warga |
| NF-05 | Keamanan (pengembangan lanjutan) | Halaman admin idealnya dilindungi autentikasi agar hanya pengurus yang dapat mengubah data |

## 3. Aktor Sistem

- **Warga**: mengakses halaman Beranda, Lapor Sampah, dan Jadwal
- **Admin (Pengurus RT/RW)**: mengakses seluruh halaman warga ditambah halaman Kelola (Admin) untuk mengelola laporan dan jadwal

## 4. Ruang Lingkup (Scope)

**Termasuk dalam scope tugas ini:**
- Prototipe aplikasi web (frontend) dengan alur pelaporan dan pengelolaan jadwal
- Dokumentasi studi kasus dan requirement
- Pengelolaan proyek melalui GitHub (Issues, Projects, branching, PR)

**Di luar scope (pengembangan lanjutan):**
- Backend/database permanen
- Autentikasi login admin
- Notifikasi otomatis (WhatsApp/Telegram)
- Upload foto bukti laporan
