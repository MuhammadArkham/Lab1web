# Praktikum 1: HTML Dasar

Nama: [Isi dengan nama Anda]  
NIM: [Isi dengan NIM Anda]  
Kelas: [Isi dengan kelas Anda]  
Mata Kuliah: Pemrograman Web

## Tujuan Praktikum
1. Mahasiswa mampu memahami struktur dasar HTML
2. Mahasiswa mampu memahami Tag-tag dasar HTML  
3. Mahasiswa mampu membuat dokumen HTML

## Langkah-langkah Praktikum

### 1. Persiapan
- Membuka VSCode sebagai text editor
- Menyiapkan browser untuk testing (Mozilla Firefox/Chrome)

### 2. Membuat Struktur Dasar HTML

Membuat file `lab1_tag_dasar.html` dengan struktur dasar HTML:

```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tag HTML Dasar</title>
</head>
<body>
    <!-- Konten HTML -->
</body>
</html>
```

**Screenshot:** *[Lampirkan screenshot struktur dasar HTML di VSCode]*

### 3. Membuat Paragraf

Menambahkan dua paragraf dengan menggunakan tag `<p>`:

```html
<!-- Ini adalah paragraf pertama -->
<p align="center">Kami sedang belajar HTML dasar...</p>

<!-- Ini adalah paragraf kedua -->
<p align="right">Ini merupakan sebuah paragraf...</p>
```

**Screenshot:** *[Lampirkan screenshot hasil paragraf di browser]*

**Hasil:**
- Paragraf pertama rata tengah
- Paragraf kedua rata kanan
- Teks terbungkus dalam elemen paragraf

### 4. Menambahkan Judul (Heading)

Menambahkan heading dengan tag `<h1>`, `<h2>`, dan `<h3>`:

```html
<h1>Belajar Dasar HTML</h1>
<h2>Paragraf pada HTML</h2>
<h3>Menambahkan Gambar</h3>
```

**Screenshot:** *[Lampirkan screenshot hasil heading di browser]*

**Hasil:**
- H1 berukuran paling besar
- H2 berukuran sedang
- H3 berukuran lebih kecil
- Hierarchy yang jelas terlihat

### 5. Memformat Teks

Menggunakan berbagai tag pemformatan teks:

```html
<b>Bold text</b>
<i>Italic text</i>
<strong>Important text</strong>
<em>Emphasized text</em>
<mark>Marked text</mark>
<small>Smaller text</small>
<del>Deleted text</del>
<ins>Inserted text</ins>
<sub>Subscript</sub>
<sup>Superscript</sup>
```

**Screenshot:** *[Lampirkan screenshot hasil pemformatan teks]*

**Hasil:**
- Berbagai gaya teks berhasil diterapkan
- Setiap tag memiliki tampilan yang berbeda

### 6. Menyisipkan Gambar

Menambahkan gambar dengan tag `<img>`:

```html
<img src="Logo_UPB.png" width="200" alt="Logo Universitas Pelita Bangsa" title="Logo Universitas Pelita Bangsa">
```

**Screenshot:** *[Lampirkan screenshot hasil gambar di browser]*

**Hasil:**
- Gambar berhasil ditampilkan
- Ukuran gambar disesuaikan dengan atribut width
- Alt dan title berfungsi sebagai deskripsi

### 7. Menambahkan Hyperlink

Membuat navigasi dengan hyperlink:

```html
<nav>
    <a href="lab1_tag_dasar.html">Dasar HTML</a>
    <a href="lab1_halaman2.html">Halaman 2</a>
    <a href="http://www.google.com">Halaman Web Eksternal Google</a>
</nav>
```

**Screenshot:** *[Lampirkan screenshot hasil hyperlink]*

**Hasil:**
- Link internal dan eksternal berfungsi
- Navigasi antar halaman berhasil

### 8. Membuat Halaman Kedua

Membuat file `lab1_halaman2.html` dengan konten berbeda dan link balik ke halaman utama.

**Screenshot:** *[Lampirkan screenshot halaman kedua]*

## Validasi HTML

Melakukan validasi HTML menggunakan https://validator.w3.org

**Screenshot:** *[Lampirkan screenshot hasil validasi]*

## Jawaban Pertanyaan

### 1. Perubahan kode dan error handling
Ketika terjadi kesalahan penulisan tag HTML:
- Browser akan tetap berusaha menampilkan konten
- Tag yang tidak tertutup mungkin akan mempengaruhi elemen lainnya
- HTML bersifat "forgiving" - tidak akan menampilkan error seperti bahasa pemrograman lain
- Validator W3C dapat membantu mendeteksi kesalahan

### 2. Perbedaan tag `<p>` dan `<br>`
- **Tag `<p>`**: 
  - Membuat paragraf baru dengan jarak (margin) atas dan bawah
  - Block-level element
  - Memiliki tag pembuka dan penutup
  - Digunakan untuk membungkus kumpulan kalimat
  
- **Tag `<br>`**:
  - Hanya membuat line break (pindah baris)
  - Inline element
  - Self-closing tag (tidak memiliki tag penutup)
  - Digunakan untuk pindah baris tanpa membuat paragraf baru

### 3. Perbedaan atribut `title` dan `alt` pada tag `<img>`
- **Atribut `alt`**:
  - Alternatif teks yang ditampilkan jika gambar gagal dimuat
  - Penting untuk accessibility (screen reader)
  - Wajib ada untuk validasi HTML
  
- **Atribut `title`**:
  - Tooltip yang muncul saat mouse hover di atas gambar
  - Memberikan informasi tambahan
  - Bersifat opsional

### 4. Pengaturan ukuran gambar dengan width dan height
**Sebaiknya tidak mengisi keduanya secara bersamaan** kecuali Anda yakin dengan rasio yang tepat.

**Alasan:**
- Jika mengisi keduanya dengan nilai yang tidak proporsional, gambar akan terdistorsi
- **Rekomendasi**: Gunakan hanya `width` ATAU `height`, browser akan otomatis menyesuaikan yang lain secara proporsional
- Jika harus menggunakan keduanya, pastikan rasio sesuai dengan gambar asli

### 5. Atribut `target` pada link

```html
<a href="url" target="_blank">_blank</a>   <!-- Buka di tab/window baru -->
<a href="url" target="_self">_self</a>     <!-- Buka di tab yang sama (default) -->
<a href="url" target="_parent">_parent</a> <!-- Buka di parent frame -->
<a href="url" target="_top">_top</a>       <!-- Buka di window paling atas -->
```

**Hasil pengujian:**
- `_blank`: Membuka link di tab atau window baru
- `_self`: Membuka link di tab yang sama (perilaku default)
- `_parent`: Berguna dalam frame, membuka di parent frame
- `_top`: Berguna dalam frame, membuka di window paling atas

## Kesimpulan

Praktikum ini berhasil mengajarkan:
1. Struktur dasar dokumen HTML
2. Penggunaan berbagai tag HTML dasar
3. Pemformatan teks dan pengaturan layout sederhana
4. Penyisipan gambar dan hyperlink
5. Validasi dokumen HTML

HTML sebagai markup language sangat fleksibel dan mudah dipelajari, menjadi fondasi penting untuk pengembangan web.

## File yang Dibuat
1. `lab1_tag_dasar.html` - Halaman utama dengan berbagai contoh tag HTML
2. `lab1_halaman2.html` - Halaman kedua untuk demonstrasi hyperlink
3. `README.md` - Dokumentasi praktikum ini

---
**Catatan**: Pastikan untuk melakukan screenshot pada setiap langkah dan menyimpannya dalam folder `screenshots/` di repository ini.
