<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Finance Tracker - Panduan</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      max-width: 900px;
      margin: 40px auto;
      padding: 0 16px;
      color: #333;
    }
    h1, h2 {
      color: #1a7a3c;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 12px 0;
    }
    table, th, td {
      border: 1px solid #ddd;
    }
    th, td {
      padding: 10px;
      text-align: left;
    }
    th {
      background-color: #f5f5f5;
    }
    code {
      background: #f4f4f4;
      padding: 4px 6px;
      border-radius: 4px;
    }
    .section {
      margin-bottom: 32px;
    }
  </style>
</head>
<body>

  <h1>Finance Tracker Mobile (Google Apps Script)</h1>
  <p>
    Aplikasi ini digunakan untuk mencatat pemasukan dan pengeluaran harian.
    Data tersimpan langsung di Google Spreadsheet dan dapat diakses melalui web.
  </p>

  <div class="section">
    <h2>1. Persiapan Spreadsheet</h2>
    <p>Buat Google Spreadsheet baru, lalu siapkan:</p>

    <p><strong>Nama Sheet (wajib):</strong></p>
    <code>Data Keuangan</code>

    <p><strong>Struktur Kolom (harus sesuai urutan):</strong></p>
    <table>
      <tr>
        <th>Kolom</th>
        <th>Nama</th>
        <th>Keterangan</th>
      </tr>
      <tr><td>A</td><td>ID</td><td>Otomatis (tidak perlu diisi)</td></tr>
      <tr><td>B</td><td>Tanggal</td><td>Format: DD/MM/YYYY</td></tr>
      <tr><td>C</td><td>Jenis</td><td>Pemasukan / Pengeluaran</td></tr>
      <tr><td>D</td><td>Kategori</td><td>Contoh: Gaji, Makanan</td></tr>
      <tr><td>E</td><td>Deskripsi</td><td>Keterangan transaksi</td></tr>
      <tr><td>F</td><td>Nominal</td><td>Angka saja (tanpa titik/koma)</td></tr>
    </table>

    <p><strong>Kolom Tambahan (opsional):</strong></p>
    <table>
      <tr>
        <th>Kolom</th>
        <th>Nama</th>
      </tr>
      <tr><td>G</td><td>Metode Bayar</td></tr>
      <tr><td>H</td><td>Catatan</td></tr>
    </table>
  </div>

  <div class="section">
    <h2>2. Sheet Kategori (Opsional)</h2>
    <p>Jika ingin kategori custom, buat sheet baru dengan nama:</p>
    <code>Referensi Kategori</code>

    <p><strong>Struktur:</strong></p>
    <ul>
      <li>Kolom A: Jenis (Pemasukan / Pengeluaran)</li>
      <li>Kolom B: Nama Kategori</li>
    </ul>

    <p>Jika tidak dibuat, aplikasi akan menggunakan kategori default.</p>
  </div>

  <div class="section">
    <h2>3. Setup Google Apps Script</h2>
    <p>Langkah:</p>
    <ol>
      <li>Buka Spreadsheet</li>
      <li>Klik <strong>Extensions → Apps Script</strong></li>
      <li>Buat file <code>Code.gs</code></li>
      <li>Buat file <code>Index.html</code></li>
      <li>Masukkan kode aplikasi yang sudah disiapkan</li>
    </ol>
  </div>

  <div class="section">
    <h2>4. Deploy Web App</h2>
    <p>Langkah:</p>
    <ol>
      <li>Klik <strong>Deploy</strong></li>
      <li>Pilih <strong>Deploy as Web App</strong></li>
      <li>Pengaturan:
        <ul>
          <li>Execute as: Me</li>
          <li>Who has access: Anyone</li>
        </ul>
      </li>
      <li>Klik Deploy</li>
      <li>Salin URL Web App</li>
    </ol>
  </div>

  <div class="section">
    <h2>5. Cara Penggunaan</h2>
    <ol>
      <li>Klik tombol Tambah Transaksi</li>
      <li>Isi data:
        <ul>
          <li>Tanggal</li>
          <li>Jenis</li>
          <li>Kategori</li>
          <li>Deskripsi</li>
          <li>Nominal</li>
        </ul>
      </li>
      <li>Klik Simpan</li>
      <li>Data otomatis masuk ke Spreadsheet</li>
    </ol>
  </div>

  <div class="section">
    <h2>6. Fitur</h2>
    <ul>
      <li>Tambah, edit, dan hapus transaksi</li>
      <li>Sinkronisasi otomatis ke Google Spreadsheet</li>
      <li>Laporan dan grafik keuangan</li>
      <li>Filter dan pencarian data</li>
      <li>Export ke CSV</li>
    </ul>
  </div>

</body>
</html>
