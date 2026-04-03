<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>

  <h1>Finance Tracker Mobile (Google Apps Script)</h1>
  <p>
    Aplikasi ini digunakan untuk mencatat pemasukan dan pengeluaran harian.
    Data tersimpan di Google Spreadsheet dan dapat diakses melalui web.
  </p>

  <div class="section">
    <h2>1. Download Source Code</h2>
    <ol>
      <li>Buka repository GitHub</li>
      <li>Klik tombol <strong>Code</strong></li>
      <li>Pilih <strong>Download ZIP</strong></li>
      <li>Ekstrak file</li>
    </ol>
  </div>

  <div class="section">
    <h2>2. Persiapan Spreadsheet</h2>
    <p>Buat Google Spreadsheet dan buat sheet dengan nama berikut (harus sama persis):</p>
    <code>Data Keuangan</code>

    <p><strong>Struktur Kolom (harus sesuai urutan):</strong></p>
    <table>
      <tr>
        <th>ID</th>
        <th>Tanggal</th>
        <th>Jenis</th>
        <th>Kategori</th>
        <th>Deskripsi</th>
        <th>Nominal</th>
        <th>Metode Bayar</th>
        <th>Catatan</th>
      </tr>
      <tr>
        <td>Auto</td>
        <td>DD/MM/YYYY</td>
        <td>Pemasukan / Pengeluaran</td>
        <td>Bebas</td>
        <td>Bebas</td>
        <td>Angka saja</td>
        <td>Opsional</td>
        <td>Opsional</td>
      </tr>
    </table>

    <p>Catatan:</p>
    <ul>
      <li>Nama kolom harus sama persis (huruf besar kecil diperhatikan)</li>
      <li>Urutan kolom tidak boleh diubah</li>
      <li>Nominal hanya angka tanpa titik atau koma</li>
    </ul>
  </div>

  <div class="section">
    <h2>3. Setup Google Apps Script</h2>
    <ol>
      <li>Buka Spreadsheet</li>
      <li>Klik <strong>Extensions → Apps Script</strong></li>
      <li>Salin isi file <code>Code.gs</code> dari repository</li>
      <li>Buat file <code>Index.html</code></li>
      <li>Salin isi file <code>Index.html</code> dari repository</li>
    </ol>
  </div>

  <div class="section">
    <h2>4. Deploy Web App</h2>
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
      <li>Salin URL aplikasi</li>
    </ol>
  </div>

  <div class="section">
    <h2>5. Cara Penggunaan</h2>
    <ol>
      <li>Buka URL Web App</li>
      <li>Klik Tambah Transaksi</li>
      <li>Isi data transaksi</li>
      <li>Klik Simpan</li>
    </ol>
    <p>Data akan otomatis masuk ke Spreadsheet.</p>
  </div>

  <div class="section">
    <h2>6. Fitur</h2>
    <ul>
      <li>Tambah, edit, dan hapus transaksi</li>
      <li>Sinkronisasi otomatis ke Google Spreadsheet</li>
      <li>Laporan dan grafik keuangan</li>
      <li>Filter dan pencarian data</li>
      <li>Export CSV</li>
    </ul>
  </div>

</body>
</html>
