# Sigap Sampah 🗑️
### Aplikasi Pelaporan & Jadwal Pengangkutan Sampah Lingkungan RT/RW

Proyek Tugas Mata Kuliah **Rekayasa Perangkat Lunak (RPL)** — dikelola menggunakan **GitHub** (Repository, Issues, Projects/Board, Pull Request).

---

## 1. Latar Belakang / Studi Kasus

Di banyak lingkungan RT/RW, warga sering tidak tahu jadwal pasti pengangkutan sampah dan tidak punya saluran jelas untuk melaporkan tumpukan sampah liar atau sampah yang terlewat jadwal. Akibatnya sampah menumpuk, menimbulkan bau, dan berpotensi menjadi sumber penyakit.

**Sigap Sampah** hadir sebagai solusi digital sederhana: warga dapat melaporkan titik sampah secara langsung, sementara pengurus RT/RW dapat mengatur jadwal pengangkutan dan menindaklanjuti laporan dari satu dasbor.

Detail lengkap ada di [`docs/studi-kasus.md`](docs/studi-kasus.md).

## 2. Fitur Utama

| Fitur | Deskripsi |
|---|---|
| 📋 Lapor Sampah | Warga mengisi formulir (nama, RT, lokasi, jenis sampah, deskripsi) |
| 📅 Jadwal Pengangkutan | Menampilkan jadwal per RT (hari, jam, rute) |
| 🛠️ Kelola Laporan (Admin) | Pengurus RT/RW mengubah status laporan: Menunggu → Diproses → Selesai |
| 🗓️ Kelola Jadwal (Admin) | Pengurus menambah/menghapus jadwal pengangkutan per RT |
| 📊 Ringkasan Beranda | Statistik jumlah laporan, laporan selesai, dan RT terjadwal |

## 3. Cara Menjalankan

Proyek ini adalah aplikasi web statis (HTML/CSS/JavaScript), tidak memerlukan instalasi backend.

```bash
git clone https://github.com/nama-kelompok/sigap-sampah.git
cd sigap-sampah
# buka index.html langsung di browser, atau jalankan local server:
python -m http.server 8000
```

Lalu buka `http://localhost:8000` di browser.

> Catatan: Versi ini menyimpan data laporan & jadwal di memori browser selama sesi berjalan (untuk keperluan demo/prototipe). Untuk versi produksi, data perlu disimpan ke database (lihat bagian **Pengembangan Selanjutnya**).

## 4. Struktur Proyek

```
sigap-sampah/
├── index.html              # Aplikasi utama (Beranda, Lapor, Jadwal, Admin)
├── README.md
└── docs/
    ├── studi-kasus.md       # Analisis masalah & solusi
    ├── requirements.md      # Kebutuhan fungsional & non-fungsional
    └── design/               # Diagram use case, ERD, flowchart (tambahkan di sini)
```

## 5. Manajemen Proyek

Proyek ini dikembangkan menggunakan alur kerja GitHub:

- **Issues** — setiap fitur/bug dicatat sebagai issue dan diberi label (`feature`, `bug`, `docs`)
- **Projects (Board)** — kolom `To Do → In Progress → Review → Done`
- **Branching** — `main` (stabil), `develop` (integrasi), `feature/nama-fitur` (per fitur)
- **Pull Request** — setiap fitur direview anggota tim sebelum digabung ke `develop`
- **Milestones** — dibagi per tahap: Analisis → Desain → Development → Testing

## 6. Anggota Tim

| Nama | Peran | GitHub |
|---|---|---|
| _(isi nama)_ | Project Manager | @username |
| _(isi nama)_ | Frontend Developer | @username |
| _(isi nama)_ | Backend Developer | @username |
| _(isi nama)_ | QA / Tester | @username |
| _(isi nama)_ | Dokumentasi & Desain | @username |

## 7. Pengembangan Selanjutnya

- Integrasi database (mis. Firebase / MySQL) agar data tersimpan permanen
- Sistem login untuk pengurus RT/RW (autentikasi admin)
- Notifikasi WhatsApp/Telegram H-1 sebelum jadwal pengangkutan
- Upload foto bukti laporan
- Peta lokasi laporan (Google Maps API)

---
*Dibuat untuk memenuhi Tugas Mata Kuliah RPL — Studi Kasus Pengelolaan Sampah Lingkungan RT/RW.*
