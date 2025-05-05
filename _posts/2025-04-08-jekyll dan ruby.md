<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Laporan Jekyll dan Ruby</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f9f9f9;
      color: #333;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #2c3e50;
      color: white;
      padding: 30px 40px;
      text-align: center;
    }

    .container {
      max-width: 960px;
      margin: 30px auto;
      padding: 20px 40px;
      background-color: #ffffff;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h1, h2, h3 {
      color: #2c3e50;
    }

    pre {
      background-color: #f0f0f0;
      padding: 15px;
      border-left: 5px solid #3498db;
      overflow-x: auto;
      font-family: monospace;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 10px;
      margin-bottom: 20px;
    }

    th, td {
      border: 1px solid #ccc;
      padding: 10px;
    }

    th {
      background-color: #f2f2f2;
    }

    img {
      max-width: 100%;
      margin: 10px 0;
      border: 1px solid #ccc;
    }

    ul {
      margin-left: 20px;
    }

    ol {
      margin-left: 20px;
    }
  </style>
</head>
<body>

<header>
  <h1>Laporan Teknologi Web</h1>
  <p>Jekyll dan Ruby: Pengembangan Situs Statis Modern</p>
</header>

<div class="container">
  <h2>BAB I – PENDAHULUAN</h2>

  <h3>1.1 Latar Belakang</h3>
  <p>Jekyll adalah generator situs statis berbasis Ruby. Ia memungkinkan pengembangan website tanpa database dan sangat cocok untuk blog, portofolio, dan dokumentasi.</p>

  <h3>1.2 Rumusan Masalah</h3>
  <ul>
    <li>Apa itu Jekyll dan bagaimana cara kerjanya?</li>
    <li>Apa hubungan antara Jekyll dan Ruby?</li>
    <li>Apa kelebihan dan kekurangannya?</li>
  </ul>

  <h3>1.3 Tujuan</h3>
  <ul>
    <li>Menjelaskan pengertian dan fungsi Jekyll dan Ruby.</li>
    <li>Menganalisis kelebihan penggunaan Jekyll.</li>
    <li>Memberikan contoh penerapan.</li>
  </ul>

  <h2>BAB II – TINJAUAN PUSTAKA</h2>

  <h3>2.1 Ruby</h3>
  <p>Ruby adalah bahasa pemrograman dinamis, mudah dibaca dan digunakan dalam berbagai platform web.</p>
  <pre>
puts "Hello, world!"
  </pre>

  <h3>2.2 Jekyll</h3>
  <p>Jekyll mengubah file Markdown menjadi HTML statis.</p>
  <pre>
---
layout: post
title: "Postingan Pertama"
date: 2025-05-01
---

Ini adalah konten blog saya yang dibuat dengan Jekyll.
  </pre>

  <h3>2.3 Struktur Folder Jekyll</h3>
  <pre>
/_layouts
/_posts
/_includes
/_site
_config.yml
  </pre>

  <h2>BAB III – METODOLOGI</h2>
  <h3>3.1 Alat dan Bahan</h3>
  <ul>
    <li>Ruby</li>
    <li>Bundler</li>
    <li>Jekyll</li>
    <li>VS Code</li>
    <li>GitHub Pages (opsional)</li>
  </ul>

  <h3>3.2 Langkah Kerja</h3>
  <pre>
gem install bundler jekyll
jekyll new mysite
cd mysite
bundle exec jekyll serve
  </pre>

  <h2>BAB IV – HASIL DAN PEMBAHASAN</h2>

  <h3>4.1 Struktur Proyek</h3>
  <img src="https://via.placeholder.com/600x300.png?text=Struktur+Folder+Jekyll" alt="Struktur Jekyll" />

  <h3>4.2 Tampilan Situs</h3>
  <img src="https://via.placeholder.com/600x300.png?text=Tampilan+Situs+Jekyll" alt="Tampilan Situs Jekyll" />

  <h3>4.3 Pembahasan</h3>
  <p>Jekyll menghasilkan situs statis yang cepat dan ringan. Dukungan GitHub Pages memudahkan publikasi tanpa biaya tambahan.</p>

  <h2>BAB V – PENUTUP</h2>

  <h3>5.1 Kesimpulan</h3>
  <p>Jekyll adalah alat modern untuk membangun situs statis, didukung Ruby yang fleksibel dan ekspresif.</p>

  <h3>5.2 Saran</h3>
  <p>Gunakan Jekyll untuk blog, dokumentasi, atau portofolio. Pelajari juga plugin dan tema yang tersedia.</p>

  <h2>Daftar Pustaka</h2>
  <ol>
    <li>Jekyllrb.com – Dokumentasi Resmi</li>
    <li>Ruby-lang.org – Bahasa Ruby</li>
    <li>GitHub Pages Docs – Hosting Situs dengan Jekyll</li>
  </ol>
</div>

</body>
</html>
S