<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Link dan Lists</title>
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
        <h1>HTML Link dan Lists</h1>
        <p>Penjelasan tentang link dan lists pada HTML.</p>
    </header>

    <img src="/assets/image/Screenshot 2025-05-04 221227.jpg" alt="HTML link dan lists">

    <h2>HTML Link (Tautan)</h2>
    <p>HTML link atau tautan adalah elemen di HTML yang digunakan untuk menghubungkan satu halaman dengan halaman lainnya. Misalnya, dari halaman utama ke halaman profil, atau dari websitemu ke Google. Biasanya, link ini terlihat seperti teks biru yang bisa diklik.</p>
    <p>Contohnya seperti ini: “Klik di sini untuk membuka Google.”</p>
    <p>Link dibuat menggunakan tag (anchor <code>&lt;a&gt;</code>), dan di dalamnya kita menulis alamat tujuan di atribut <code>href</code>.</p>

    <h3>Penjelasan Atribut Link:</h3>
    <ul>
        <li><code>href</code>: Alamat tujuan tautan.</li>
        <li><code>target="_blank"</code>: Buka link di tab baru.</li>
    </ul>
    <p>Contoh penggunaan link:</p>
    <pre><code>&lt;a href="https://www.google.com" target="_blank"&gt;Klik di sini untuk membuka Google&lt;/a&gt;</code></pre>

    <h2>List (Daftar) dalam HTML</h2>
    <p>List digunakan untuk menyusun informasi dalam bentuk poin-poin atau urutan.</p>

    <h3>Unordered List (&lt;ul&gt;) – daftar tak berurutan (pakai bullet)</h3>
    <p>Digunakan untuk item-item yang tidak memerlukan urutan tertentu. Setiap item daftar ditandai dengan simbol seperti bullet point.</p>
    <p>Contoh :</p>
    <pre><code>&lt;ul&gt;
    &lt;li&gt;HTML&lt;/li&gt;
    &lt;li&gt;CSS&lt;/li&gt;
    &lt;li&gt;JavaScript&lt;/li&gt;
&lt;/ul&gt;</code></pre>
    Hasilnya akan terlihat seperti ini:
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>

    <h3>Ordered List (&lt;ol&gt;) – daftar berurutan (pakai angka)</h3>
    <p>Digunakan untuk item-item yang memiliki urutan penting, seperti langkah-langkah atau peringkat. Setiap item daftar ditandai dengan angka atau huruf secara otomatis.</p>
    <p>Contoh:</p>
    <pre><code>&lt;ol&gt;
    &lt;li&gt;Masuk akun&lt;/li&gt;
    &lt;li&gt;Buka profil&lt;/li&gt;
    &lt;li&gt;Edit data&lt;/li&gt;
&lt;/ol&gt;</code></pre>
    Hasilnya akan terlihat seperti ini:
    <ol>
        <li>Masuk akun</li>
        <li>Buka profil</li>
        <li>Edit data</li>
    </ol>

    <h3>Definition List (&lt;dl&gt;) – daftar istilah dan definisinya</h3>
    <p>Digunakan untuk menyusun daftar istilah (<code>&lt;dt&gt;</code>) dan definisi atau penjelasannya (<code>&lt;dd&gt;</code>).</p>
    <p>Contoh:</p>
    <pre><code>&lt;dl&gt;
    &lt;dt&gt;HTML&lt;/dt&gt;
    &lt;dd&gt;HyperText Markup Language&lt;/dd&gt;
    &lt;dt&gt;CSS&lt;/dt&gt;
    &lt;dd&gt;Cascading Style Sheets&lt;/dd&gt;
&lt;/dl&gt;</code></pre>
    Hasilnya akan terlihat seperti ini:
    <dl>
        <dt>HTML</dt>
        <dd>HyperText Markup Language</dd>
        <dt>CSS</dt>
        <dd>Cascading Style Sheets</dd>
    </dl>

    <footer>
        <p>&copy; 2025 Dwi Ida Rahmadani Situmorang. All rights reserved.</p>
    </footer>

</div>

</body>
</html>