<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Laporan CSS dan SASS</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f4f4;
      color: #333;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #2c3e50;
      color: white;
      padding: 20px 40px;
      text-align: center;
    }

    .container {
      max-width: 960px;
      margin: auto;
      padding: 20px 40px;
      background-color: #fff;
    }

    h1, h2, h3 {
      color: #2c3e50;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
      margin-bottom: 20px;
    }

    table, th, td {
      border: 1px solid #ccc;
    }

    th, td {
      padding: 10px;
      text-align: left;
    }

    .code {
      background-color: #eee;
      padding: 10px;
      border-left: 5px solid #3498db;
      font-family: monospace;
      white-space: pre-wrap;
      margin-bottom: 15px;
    }

    img {
      max-width: 100%;
      border: 1px solid #ccc;
      margin: 10px 0;
    }
  </style>
</head>
<body>

<header>
  <h1>Laporan Teknologi Web</h1>
  <p>CSS dan SASS: Penggunaan dan Perbandingan dalam Pengembangan Web</p>
</header>

<div class="container">
  <h2>Bab I – Pendahuluan</h2>
  <h3>1.1 Latar Belakang</h3>
  <p>CSS adalah bahasa desain untuk halaman web, sedangkan SASS adalah preprocessor CSS dengan fitur lanjutan.</p>

  <h3>1.2 Rumusan Masalah</h3>
  <ul>
    <li>Apa perbedaan antara CSS dan SASS?</li>
    <li>Apa kelebihan dan kekurangan masing-masing?</li>
    <li>Bagaimana penerapannya dalam proyek web?</li>
  </ul>

  <h3>1.3 Tujuan</h3>
  <ul>
    <li>Menjelaskan fungsi CSS dan SASS</li>
    <li>Menganalisis kelebihan dan kekurangannya</li>
    <li>Memberi contoh implementasi</li>
  </ul>

  <h2>Bab II – Tinjauan Pustaka</h2>
  <h3>2.1 CSS</h3>
  <div class="code">
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}
  </div>

  <h3>2.2 SASS</h3>
  <div class="code">
$primary-color: #3498db;

body {
  background-color: $primary-color;
  font-family: Arial, sans-serif;

  h1 {
    color: white;
  }
}
  </div>

  <h3>2.3 Perbandingan</h3>
  <table>
    <tr>
      <th>Aspek</th>
      <th>CSS</th>
      <th>SASS</th>
    </tr>
    <tr>
      <td>Sintaks</td>
      <td>Sederhana</td>
      <td>Lebih kompleks dan efisien</td>
    </tr>
    <tr>
      <td>Variabel</td>
      <td>Tidak tersedia</td>
      <td>Tersedia</td>
    </tr>
    <tr>
      <td>Nesting</td>
      <td>Tidak tersedia</td>
      <td>Didukung</td>
    </tr>
    <tr>
      <td>Kompilasi</td>
      <td>Langsung di browser</td>
      <td>Perlu dikompilasi</td>
    </tr>
  </table>

  <h2>Bab III – Metodologi</h2>
  <ul>
    <li>Text Editor: VS Code</li>
    <li>Node.js & npm</li>
    <li>SASS Compiler</li>
    <li>Google Chrome</li>
  </ul>

  <h2>Bab IV – Hasil dan Pembahasan</h2>

  <h3>4.1 Tampilan CSS</h3>
  <img src="https://via.placeholder.com/600x300.png?text=Tampilan+CSS" alt="Tampilan CSS">
  <div class="code">
.container {
  width: 80%;
  margin: auto;
  color: blue;
}
  </div>

  <h3>4.2 Tampilan SASS</h3>
  <img src="https://via.placeholder.com/600x300.png?text=Tampilan+SASS" alt="Tampilan SASS">
  <div class="code">
$font-color: blue;

.container {
  width: 80%;
  margin: auto;
  color: $font-color;
}
  </div>

  <h3>4.3 Pembahasan</h3>
  <p>SASS membuat style lebih modular dan efisien. Variabel dan nesting sangat membantu dalam proyek berskala besar.</p>

  <h2>Bab V – Penutup</h2>
  <h3>5.1 Kesimpulan</h3>
  <p>CSS cocok untuk proyek kecil. SASS lebih baik untuk proyek besar karena kemudahan pengelolaan kode.</p>

  <h3>5.2 Saran</h3>
  <p>Gunakan SASS untuk pengembangan skala besar dan pelajari fitur lanjutan seperti mixin dan functions.</p>

  <h2>Daftar Pustaka</h2>
  <ol>
    <li>MDN Web Docs – CSS Documentation</li>
    <li>Sass-lang.com – Official SASS Docs</li>
    <li>W3Schools – CSS and SASS Tutorial</li>
  </ol>
</div>

</body>
</html>
