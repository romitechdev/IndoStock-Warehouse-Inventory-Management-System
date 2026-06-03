# IndoStock - Rancang Bangun Sistem Basis Data Manajemen Inventaris Gudang

IndoStock adalah purwarupa (prototype) sistem informasi manajemen inventaris gudang berbasis Relational Database Management System (RDBMS) yang dirancang khusus untuk studi kasus minimarket modern Indomaret. Proyek ini mengintegrasikan lima entitas master data (Karyawan, Kategori, Rak, Supplier, Produk) dengan tiga entitas transaksional utama (Barang Masuk, Barang Keluar, Retur Barang).

Sistem ini dikembangkan menggunakan Microsoft Access sebagai database engine dan Visual Basic for Applications (VBA) sebagai logika kontrol antarmuka dinamis.

## 🚀 Fitur Utama Sistem
- **Role-Based Otorisasi Dinamis (VBA):** Membatasi hak akses menu navigasi secara real-time. Akun dengan role *Pramuniaga* secara otomatis dikunci aksesnya dari menu administratif (Data Karyawan, Supplier, dan Laporan), sedangkan *Store Leader* memiliki otoritas penuh.
- **Otomatisasi Kalkulasi Metrik & Agregasi (SQL):** Perhitungan akumulasi sisa stok fisik secara otomatis melalui fungsi agregasi RDBMS seiring terjadinya transaksi barang masuk dan keluar untuk menghindari risiko *human error*.
- **Sistem Validasi Pencegahan Anomali:** Implementasi logika kontrol matematika untuk memblokir transaksi secara mutlak jika kuantitas barang keluar melebihi sisa stok fisik gudang (*Stok Tidak Mencukupi*).
- **Integritas Referensial & Pencegahan Delete Anomaly:** Pengaturan relasi database yang kokoh tanpa memicu *Cascade Delete* demi menjaga keamanan rekam jejak audit (*audit trail*) transaksional logistik.
- **Context-Sensitive Help System:** Integrasi berkas bantuan digital interaktif (.chm) yang dibuat via HelpNDoc dan dapat dipanggil langsung dari antarmuka sidebar dashboard menggunakan Windows API.

## 📁 Struktur Repositori
- `/Database`: Berisi file purwarupa database fisik `IndoStock.accdb`.
- `/Aplikasi_Manual`: Berisi berkas bantuan digital interaktif `manual.chm` yang terintegrasi langsung dengan tombol sistem bantuan di dalam aplikasi.

## 🎓 Publikasi & Hasil Pengujian
Proyek ini telah dipresentasikan dan diuji secara komprehensif menggunakan metode *Black-Box Testing*. Analisis teoretis dan teknis mendalam mengenai sistem ini telah didokumentasikan dalam artikel ilmiah kelompok kami yang memiliki *Similarity Index* sebesar **5% (Turnitin)**.

- **Artikel Ilmiah Resmi:** Dapat diakses secara terbuka melalui repositori akademik di [ResearchGate]().

## 👥 Tim Pengembang (Class of 2025B)
Proyek ini dibangun sebagai luaran tugas akhir mata kuliah Basis Data, Program Studi Sistem Informasi, Universitas Negeri Surabaya oleh:
1. Muhromin (Project Leader & System Analyst)
2. Yasmin Nur Fadila (System Designer)
3. Inka Nadia Faridiani (Implementator)
4. Muhammad Nadhif Afkar (Dokumentator)
