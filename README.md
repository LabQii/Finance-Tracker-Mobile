Finance Tracker Mobile (Google Apps Script)

Aplikasi ini digunakan untuk mencatat pemasukan dan pengeluaran harian. Data tersimpan langsung di Google Spreadsheet dan dapat diakses melalui web.

1. Persiapan Spreadsheet

Buat Google Spreadsheet baru, lalu siapkan:

Nama Sheet (wajib)

Data Keuangan

Struktur Kolom (harus sesuai urutan)
Kolom	Nama	Keterangan
A	ID	Otomatis (tidak perlu diisi)
B	Tanggal	Format: DD/MM/YYYY
C	Jenis	Pemasukan / Pengeluaran
D	Kategori	Contoh: Gaji, Makanan
E	Deskripsi	Keterangan transaksi
F	Nominal	Angka saja (tanpa titik/koma)
Kolom Tambahan (opsional)
Kolom	Nama
G	Metode Bayar
H	Catatan
2. (Opsional) Sheet Kategori

Jika ingin kategori custom, buat sheet baru:

Nama sheet:
Referensi Kategori

Struktur:

Kolom A: Jenis (Pemasukan/Pengeluaran)
Kolom B: Nama Kategori

Jika tidak dibuat, aplikasi akan menggunakan kategori default.

3. Setup Google Apps Script
Langkah
Buka Spreadsheet
Klik Extensions → Apps Script
Buat file Code.gs
Buat file Index.html
lalu masukkan code diatas

4. Deploy Web App

Langkah:

Klik Deploy
Pilih Deploy as Web App
Pengaturan:
Execute as: Me
Who has access: Anyone
Klik Deploy
Salin URL Web App

5. Cara Penggunaan
Klik tombol Tambah Transaksi
Isi data:
Tanggal
Jenis
Kategori
Deskripsi
Nominal
Klik Simpan
Data otomatis masuk ke Spreadsheet

6. Fitur
Tambah, edit, dan hapus transaksi
Sinkronisasi otomatis ke Google Spreadsheet
Laporan dan grafik keuangan
Filter dan pencarian data
Export ke CSV
