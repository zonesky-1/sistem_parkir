# 🅿️ Smart Parking System & Database Portal

Sistem perparkiran pintar yang dirancang untuk mengelola sirkulasi kendaraan, transaksi kasir, dan basis data operasional secara efisien dan aman.

---

## 📋 Fitur Sistem

- **Basis Data Relasional Lengkap**: Dilengkapi dengan skema database teruji (`parkir2.sql`) mencakup tabel kendaraan, transaksi, tarif, log petugas, dan data member.
- **Pencarian Cepat Nomor Polisi**: Pengindeksan cepat untuk pencarian tiket yang hilang atau verifikasi kendaraan member.
- **Simulasi & Pengujian (QA Suite)**: Dilengkapi modul skrip verifikasi otomatis (`qa_cek_tiket.php`, `qa_member_flow.ps1`, `qa_time_travel.php`).
- **Laporan & Rekapitulasi Kasir**: Cetak rekap pendapatan per shift petugas dan audit berkala.

---

## 🛠️ Stack Teknologi

- **Framework Backend**: Laravel 11 (PHP 8.2+)
- **Framework Frontend**: Nuxt 3 / Vue 3 dengan TypeScript
- **Basis Data**: MySQL / MariaDB (import dari `parkir2.sql`)

---

## 💻 Cara Memulai

1. **Import Database**:
   Import file `parkir2.sql` ke database MySQL lokal Anda:
   ```bash
   mysql -u root -p database_parkir < parkir2.sql
   ```
2. **Konfigurasi Backend**:
   ```bash
   cd backend && composer install && php artisan serve
   ```
3. **Jalankan Frontend**:
   ```bash
   cd frontend && npm install && npm run dev
   ```
