# Lab1Web - Praktikum 1: HTML Dasar

**Nama:** Khairi Ramadhan Yudhatama  
**NIM:** 312510099  
**Kelas:** Pemrograman Web (I251A)  
**Dosen:** Agung Nugroho, S.Kom., M.Kom.  
**Mata Kuliah:** Pemrograman Web  
**Universitas:** Universitas Pelita Bangsa

---

## Deskripsi Praktikum

Praktikum ini bertujuan untuk mengenal dan mempraktikkan tag-tag dasar HTML, mulai dari struktur dokumen, paragraf, heading, formatting teks, gambar, hyperlink, list, komentar, hingga menggabungkan semua elemen menjadi satu halaman Profil Mahasiswa.

Struktur folder yang digunakan:

```
praktikum-1-html-dasar/
├── index.html
├── halaman2.html
└── images/
    └── profil.jpg
```

---

## Langkah-langkah Praktikum

### 1. Membuat Paragraf

Menambahkan beberapa paragraf sederhana menggunakan tag `<p>`.

**Kode yang ditambahkan:**

```html
<!-- Ini adalah paragraf pertama -->
<p>
  Kami sedang belajar HTML dasar pada mata kuliah Pemrograman Web. Praktikum ini
  digunakan untuk mengenal tag-tag dasar HTML.
</p>

<!-- Ini adalah paragraf kedua -->
<p>
  HTML digunakan untuk menyusun struktur dan konten halaman web. Browser akan
  menampilkan hasil interpretasi dari dokumen HTML.
</p>
```

**Hasil:**  
Setelah disimpan dan di-refresh di browser, teks muncul sebagai dua paragraf terpisah dengan jarak antar paragraf yang jelas.

---

### 2. Menambahkan Judul

Menambahkan heading `h1` sebelum paragraf pertama dan `h2` sebelum paragraf kedua.

**Kode yang ditambahkan:**

```html
<!-- judul utama -->
<h1>Belajar Dasar HTML</h1>

<!-- subjudul -->
<h2>Paragraf pada HTML</h2>
```

**Hasil:**  
Judul utama (`h1`) tampil lebih besar dan menonjol, sedangkan subjudul (`h2`) lebih kecil. Hierarki heading membantu struktur dokumen.

---

### 3. Memformat Teks

Melakukan pemformatan teks pada paragraf menggunakan tag formatting.

**Kode yang digunakan:**

```html
<p>
  Kami sedang belajar <b>HTML dasar</b> pada mata kuliah <i>Pemrograman Web</i>.
</p>

<p>
  HTML merupakan <strong>bahasa markup</strong> untuk menyusun struktur halaman
  web.
</p>

<p>
  Air ditulis sebagai H<sub>2</sub>O dan luas dapat ditulis sebagai
  x<sup>2</sup>.
</p>
```

**Eksperimen tambahan:**  
Mencoba tag lain seperti `<em>`, `<mark>`, `<small>`, `<del>`, dan `<ins>` untuk melihat perbedaan efek visualnya.

**Hasil:**

- `<b>` dan `<strong>` membuat teks tebal
- `<i>` dan `<em>` membuat teks miring
- `<sub>` untuk subscript, `<sup>` untuk superscript
- Tag lain memberikan efek highlight, ukuran kecil, coret, dan garis bawah.

---

### 4. Menyisipkan Gambar

Menyiapkan gambar di folder `images/` lalu menampilkannya menggunakan tag `<img>`.

**Struktur folder:**

```
praktikum-1-html-dasar/
├── index.html
└── images/
    └── profil.jpg
```

**Kode yang ditambahkan:**

```html
<h3>Menambahkan Gambar</h3>

<img
  src="images/profil.jpg"
  width="200"
  alt="Foto profil mahasiswa"
  title="Foto Profil Mahasiswa"
/>
```

**Hasil:**  
Gambar profil muncul di halaman dengan lebar 200px. Atribut `alt` menampilkan teks alternatif jika gambar gagal dimuat, dan `title` muncul saat kursor diarahkan ke gambar.

---

### 5. Mengatur Ukuran Gambar

Mengatur ukuran gambar menggunakan atribut `width` dan `height`.

**Contoh kode:**

```html
<img src="images/profil.jpg" width="200" alt="Foto profil mahasiswa" />
```

**Hasil:**  
Dengan mengubah nilai `width` (dan/atau `height`), ukuran gambar berubah sesuai nilai yang diberikan. Disarankan menjaga proporsi agar gambar tidak terdistorsi.

---

### 6. Menambahkan Hyperlink

Membuat file kedua bernama `halaman2.html` dan menambahkan navigasi antar halaman serta link eksternal.

**Kode navigasi (diletakkan di `index.html` dan `halaman2.html`):**

```html
<!-- navigasi halaman -->
<nav>
  <a href="index.html">Dasar HTML</a>
  <a href="halaman2.html">Halaman 2</a>
  <a href="https://www.google.com">Website Eksternal</a>
</nav>

<hr />
```

**Hasil:**

- Link internal (`index.html` dan `halaman2.html`) membuka halaman lokal.
- Link eksternal membuka website Google di tab/browser yang sama.
- Tag `<hr>` menampilkan garis horizontal sebagai pemisah.

---

### 7. Menambahkan List

Menambahkan daftar keahlian (unordered list) dan urutan belajar (ordered list).

**Kode yang ditambahkan:**

```html
<h2>Keahlian</h2>
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

<h2>Urutan Belajar</h2>
<ol>
  <li>Mempelajari struktur HTML</li>
  <li>Mempelajari tag dan atribut</li>
  <li>Membuat halaman HTML</li>
  <li>Menguji halaman pada browser</li>
</ol>
```

**Hasil:**

- `<ul>` menampilkan daftar berpoin (bullet).
- `<ol>` menampilkan daftar berurutan (angka).

---

### 8. Menambahkan Komentar

Menambahkan komentar HTML untuk memberi penanda pada bagian kode.

**Contoh kode:**

```html
<!-- Bagian Profil Mahasiswa -->
<h2>Profil Mahasiswa</h2>

<!-- Bagian Keahlian -->
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>
```

**Hasil:**  
Komentar (`<!-- ... -->`) tidak ditampilkan di browser. Fungsinya hanya untuk dokumentasi kode agar lebih mudah dibaca dan dikelola.

---

### 9. Menggabungkan Semua Elemen

Membuat halaman **Profil Mahasiswa** yang menggabungkan semua elemen yang telah dipelajari.

**Kode lengkap (`index.html`):**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Profil Mahasiswa</title>
  </head>
  <body>
    <nav>
      <a href="index.html">Beranda</a>
      <a href="halaman2.html">Halaman 2</a>
    </nav>

    <hr />

    <h1>Profil Mahasiswa</h1>

    <img src="images/profil.jpg" width="200" alt="Foto profil mahasiswa" />

    <h2>Data Diri</h2>

    <p>Nama: Khairi Ramadhan Yudhatama</p>

    <p>Program Studi: Teknik Informatika</p>

    <p>
      Saya sedang mempelajari dasar-dasar pengembangan aplikasi web menggunakan
      HTML.
    </p>

    <h2>Keahlian</h2>

    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
    </ul>

    <h2>Target Belajar</h2>

    <ol>
      <li>Menguasai HTML</li>
      <li>Menguasai CSS</li>
      <li>Menguasai JavaScript</li>
    </ol>
  </body>
</html>
```

**Hasil:**  
Halaman profil lengkap dengan navigasi, gambar, data diri, daftar keahlian, dan target belajar. Semua elemen HTML dasar sudah digabungkan dalam satu dokumen yang terstruktur.

---
