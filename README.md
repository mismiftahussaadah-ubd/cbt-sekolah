# 💻 Aplikasi CBT Online & Administrasi Ujian (V2.0)
Sistem Aplikasi Computer Based Test (CBT) gratis berbasis Cloud. Menggunakan **GitHub Pages** sebagai antarmuka pengguna (Frontend) dan **Google Sheets + Google Apps Script** sebagai pusat data base (Backend).

---

## 🔗 Link Akses Resmi Aplikasi

*   **📱 Ruang Ujian Siswa:** 
    [https://github.io](https://github.io)
*   **📊 Panel Kontrol Admin (Guru):** 
    [https://github.io](https://github.io)

---

## 🛠️ Fitur Utama Aplikasi

1. **Multi-Jenis Soal (AKM Ready):** Mendukung Pilihan Ganda (PG), Pilihan Ganda Kompleks (PGK), Pilihan Ganda Kategori (Benar/Salah per baris), Menjodohkan, dan Soal Uraian/Essay.
2. **Auto-Setup Database:** Spreadsheet akan otomatis membuat tabel *Siswa*, *Soal*, dan *Jawaban* saat aplikasi dijalankan pertama kali.
3. **Sistem Pengaman Nilai:** Koreksi jawaban dilakukan di sisi server Google, siswa tidak bisa melihat kunci jawaban melalui inspeksi kode HTML.
4. **Timer Batasan Waktu:** Ujian dilengkapi hitung mundur otomatis dan sistem akan langsung mengirim jawaban jika waktu habis.
5. **Cetak Dokumen Administrasi:** Fitur cetak langsung Kartu Ujian, Daftar Hadir, dan Berita Acara yang rapi siap cetak di kertas A4.
6. **Live Monitoring:** Memantau status pengerjaan siswa secara langsung dari halaman admin.

---

## 📋 Panduan Pengoperasian Kontrol Panel

### 1. Memasukkan Data Siswa & Bank Soal
* Buka Google Spreadsheet yang telah Anda hubungkan.
* **Input Siswa:** Isi data pada tab sheet `Siswa` (kolom username, password, nama, kelas, nomor_peserta).
* **Input Soal:** Isi data pada tab sheet `Soal`. Pastikan pengisian kolom `jenis_soal` dan `kunci_jawaban` mengikuti aturan format kode (`PG`, `PGK`, `PGK_KAT`, `JODOH`, `BS`, `URAIAN`).

### 2. Sinkronisasi Data Ke Web Dashboard
* Setelah memperbarui data di Google Sheets, buka **Panel Kontrol Admin**.
* Klik tombol **"🔄 Sinkronisasi Data Terbaru"** pada halaman utama Dashboard.
* Sistem akan memuat seluruh data siswa, bank soal, dan hasil nilai terbaru ke dalam tabel web.

### 3. Mencetak Dokumen Resmi Ujian
* Masuk ke menu **🖨️ Cetak Administrasi** di bilah menu samping halaman Admin.
* Klik salah satu tombol dokumen yang dibutuhkan (Kartu Ujian / Daftar Hadir / Berita Acara).
* Sistem akan menampilkan pratinjau cetak (*print preview*). Pastikan printer Anda disetel ke ukuran kertas A4, lalu klik **Print**.

---

## ⚠️ Catatan Pemeliharaan (Maintenance)
* Jika Anda melakukan perubahan kode pada **Google Apps Script**, pastikan untuk selalu melakukan **Deploy Ulang** (*Manage Deployments* > *Edit* > *Version: New Version* > *Deploy*) agar perubahan API tersebut langsung aktif dan dapat diakses oleh GitHub.
* Tautan aplikasi ini bersifat sensitif terhadap huruf besar/kecil (*case-sensitive*), pastikan membagikan link ke siswa dengan huruf kecil semua (`siswa.html`).
