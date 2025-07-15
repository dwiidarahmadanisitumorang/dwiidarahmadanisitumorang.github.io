<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Database MySQL dan PHP</title>
    <style>
        body {
            font-family: Georgia, serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f7f7f7;
            color: #333;
        }
        .container {
            max-width: 800px;
            margin: 40px auto;
            padding: 30px 40px;
            background-color: #fff;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            border-radius: 5px;
        }
        header {
            text-align: center;
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 1px solid #eee;
        }
        header h1 {
            font-size: 2.5em;
            color: #333;
            margin-bottom: 5px;
        }
        header p {
            color: #666;
            font-size: 1.1em;
            margin-top: 0;
        }
        h2 {
            font-size: 1.8em;
            color: #24292e;
            border-bottom: 2px solid #eee;
            padding-bottom: 10px;
            margin-top: 40px;
            margin-bottom: 20px;
        }
        h3 {
            font-size: 1.4em;
            color: #555;
            margin-top: 30px;
            margin-bottom: 15px;
        }
        a {
            color: #007bff;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        pre {
            background: #f0f0f0;
            padding: 15px;
            border-left: 4px solid #007bff;
            overflow-x: auto;
            font-family: 'Courier New', Courier, monospace;
            font-size: 0.9em;
            white-space: pre-wrap;
            word-wrap: break-word;
            margin-bottom: 20px;
            border-radius: 3px;
        }
        img {
            max-width: 100%;
            height: auto;
            display: block;
            margin: 20px auto;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
        }
        ul, ol {
            margin-bottom: 20px;
            padding-left: 25px;
        }
        li {
            margin-bottom: 8px;
        }
        footer {
            text-align: center;
            margin-top: 50px;
            padding-top: 20px;
            border-top: 1px solid #eee;
            color: #888;
            font-size: 0.9em;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>Database MySQL dan PHP</h1>
        <p>Penjelasan tentang database mysql dan PHP.</p>
    </header>

    <h2>MySQL</h2>
    <p><strong>MySQL</strong> adalah sistem manajemen basis data relasional (RDBMS) yang menggunakan bahasa SQL (Structured Query Language). MySQL digunakan untuk menyimpan, mengelola, dan mengambil data secara efisien. MySQL sangat populer dalam pengembangan aplikasi web karena gratis (open source), ringan, dan cepat.</p>

    <h2>PHP</h2>
    <p><strong>PHP</strong> (Hypertext Preprocessor) adalah bahasa pemrograman sisi server yang dirancang khusus untuk pengembangan web. PHP dapat digunakan untuk menghubungkan aplikasi web dengan database, seperti MySQL.</p>

    <h2>Hubungan antara PHP dan MySQL</h2>
    <p>PHP digunakan untuk mengakses dan memanipulasi data dalam MySQL. Contohnya:</p>
    <ul>
        <li>Menyimpan data dari formulir HTML ke database</li>
        <li>Menampilkan data dari database ke halaman web</li>
        <li>Memperbarui atau menghapus data dalam database</li>
    </ul>

    <h2>Proses Umum PHP Mengakses MySQL</h2>
    <ol>
        <li>Koneksi ke Database</li>
        <li>Menjalankan Query SQL</li>
        <li>Mengambil atau memproses hasil</li>
        <li>Menutup koneksi</li>
    </ol>

    <h2>Contoh Kerja PHP dan MySQL</h2>

    <h3>1. Membuat Koneksi ke database</h3>
    <pre><code>&lt;?php
$host = "localhost";
$user = "root";
$password = "";
$database = "bengkel";

$conn = mysqli_connect($host, $user, $password, $database);

if (!$conn) {
    die("Koneksi gagal: " . mysqli_connect_error());
}

echo "Koneksi berhasil!";
?&gt;</code></pre>

    <h3>2. Menjalankan Query Select</h3>
    <pre><code>&lt;?php
$query = "SELECT * FROM pelanggan";
$result = mysqli_query($conn, $query);

// Menampilkan data
while ($row = mysqli_fetch_assoc($result)) {
    echo "Nama: " . $row['nama'] . "&lt;br&gt;";
}
?&gt;</code></pre>

    <h3>3. Query Insert (Menambah Data)</h3>
    <pre><code>&lt;?php
$nama = "Andi";
$alamat = "Jakarta";
$sql = "INSERT INTO pelanggan (nama, alamat) VALUES ('$nama', '$alamat')";

if (mysqli_query($conn, $sql)) {
    echo "Data berhasil ditambahkan!";
} else {
    echo "Error: " . mysqli_error($conn);
}
?&gt;</code></pre>

    <h3>4. Menutup Koneksi</h3>
    <pre><code>&lt;?php
mysqli_close($conn);
?&gt;</code></pre>

    <h2>Tips Penggunaan</h2>
    <ul>
        <li>Gunakan <strong>prepared statements</strong> (mysqli atau PDO) untuk mencegah <strong>SQL Injection</strong>.</li>
        <li>Pastikan database dan tabel sudah dibuat sebelum digunakan dalam PHP.</li>
        <li>Selalu cek hasil koneksi dan hasil query untuk menangani error dengan baik.</li>
    </ul>

    <h2>Tools Pendukung</h2>
    <ul>
        <li><strong>XAMPP/Laragon:</strong> Paket instalasi PHP, MySQL, dan Apache untuk lokal development.</li>
        <li><strong>phpMyAdmin:</strong> Antarmuka web untuk mengelola MySQL.</li>
        <li><strong>VS Code:</strong> Editor kode yang umum digunakan untuk PHP + MySQL development.</li>
    </ul>

    <footer>
        <p>&copy; 2025 Dwi Ida Rahmadani Situmorang. All rights reserved.</p>
    </footer>

</div>

</body>
</html>