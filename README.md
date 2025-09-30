# Data Diri

Nama : Safitri Eka Ramadhani

NIM : 312410431

Kelas : TI.24.A.3

# Praktikum CSS Dasar

Tujuan Praktikum
- Mengenal penggunaan Inline CSS, Internal CSS, dan Eksternal CSS.
- Memahami cara kerja ID Selector (#id) dan Class Selector (.class) dalam CSS.
- Membuat halaman web sederhana dengan kombinasi HTML dan CSS.
- Melatih keterampilan memisahkan struktur (HTML) dan gaya tampilan (CSS).

# Langkah-Langkah Praktikum

# 1. Struktur HTML

## Input Struktur HTML
<Img src="code 1.png">

## Output
<Img src="hasil 1.png">

Penjelasan:
- `<header>` → menampilkan judul utama.
- `<nav>` → menu navigasi ke halaman lain.
- `<div#intro>` → bagian utama dengan ID untuk di-style khusus.
- `<p style="...">` → contoh Inline CSS.
- `<a class="button btn-primary">` → contoh penggunaan Class Selector.

# 2. Menambahkan Inline CSS 

## Input Struktur HTML
<Img src="code 3.png">

## Output
<Img src="hasil 3.png">

Penjelasan:
- tag `<p>` digunakan untuk membuat paragraf.
- Semua teks di dalamnya dianggap sebagai satu blok paragraf.
`style="text-align: center; color: #ccd8e4;"`
- Ini adalah Inline CSS, yaitu CSS langsung ditulis pada atribut style di elemen.
- `text-align: center;` → membuat teks rata tengah.
- `color: #ccd8e4;` → memberi warna teks dengan kode hex (#ccd8e4 → abu-abu kebiruan).

# 3. Internal CSS & Eksternal CSS

## Input CSS & Eksternal CSS
<Img src="code 2.png">
<img src="code 4.png>

## Output
<Img src="hasil 2.png">
<img src="hasil 4.png>

Penjelasan:
- Internal CSS → ditulis dalam tag `<style>` (contohnya untuk `body`, `header`, dan `h1`
- Eksternal CSS → dipisahkan di file `style_eksternal.css` yang dipanggil dengan `link`.

# 4. CSS untuk Navigasi

## Input Nav
<img src="code css 1.png">

## Output
<img src="code css 1.png">

Penjelasan:
- `nav` → memberi warna latar hijau & teks putih.
- `nav a` → link tanpa garis bawah dengan padding.
- `nav .active` & `nav a:hover` → efek highlight ketika link aktif atau di-hover.

# 5. ID Selector & Class Selector

## Input 
<img src="code css 2.png">

## Output
<img src="hasil akhir.png">

Penjelasan:
- `#intro` → khusus untuk elemen dengan ID `intro`.
- `#intro h1` → heading di dalam intro menjadi rata kiri dan berwarna putih.
- `.button` → gaya dasar tombol (padding, background abu-abu, teks putih, margin, inline-block).
- `.btn-primary` → variasi tombol utama dengan background merah.

# Kesimpulan

Dalam praktikum ini dipelajari:
- Inline CSS → gaya langsung dalam atribut style.
- Internal CSS → gaya dalam `<style>` di `HTML`.
- Eksternal CSS → gaya di file .css` terpisah.
- ID Selector → digunakan untuk elemen unik (`#intro`).
- Class Selector → digunakan untuk elemen yang bisa berulang (`.button`, `.btn-primary`).

# Pertanyaan dan Tugas

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini. 
Jawab:

## Input CSS
<img src="code css tugas 1.png">

## Input HTML
<img src="code tugas 1.png">

## Output
<img src="hasil tugas 1.png">

Penjelasan Eksperimen:
A. Body
- Tambahan `margin: 0; padding: 0;` → agar halaman lebih rapi tanpa spasi default.
- `line-height: 1.6;` → membuat teks lebih enak dibaca.

B. h1 (judul)
- `text-transform: uppercase;` → otomatis mengubah teks jadi huruf kapital.
- `letter-spacing: 2px;` → memberi jarak antar huruf.
- `text-shadow` → efek bayangan agar judul lebih menonjol.
- `border-bottom` → garis dekorasi di bawah judul.

C. p (paragraf)
- `font-size: 18px;` → ukuran teks lebih nyaman dibaca.
- `text-align: justify;` → paragraf rata kiri-kanan agar rapi.

D. .container
- `display: flex;` justify-content: center; align-items: center;` → konten selalu rata tengah.
- `background-image: linear-gradient()` → menambahkan efek gradasi warna.

E. button
- `border-radius: 8px;` → sudut tombol lebih halus.
- `cursor: pointer;` → kursor berubah saat diarahkan.
- `transition` → animasi halus saat hover.
- `transform: scale(1.1);` → efek tombol sedikit membesar ketika di-hover.

2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya! 
Jawab:

## Input CSS
<img src="code tugas css 2.png">

## Input HTML
<img src="code tugas html 2.png">

## Output
<img src="hasil tugas 2.png">

Perbedaan `h1` { ... } dengan `#intro h1` { ... }
- `h1` { ... }
→ berlaku untuk semua elemen `<h1>` di halaman web.
- #intro h1` { ... }
→ berlaku khusus untuk elemen `<h1>` yang ada di dalam elemen dengan ID intro.

3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! 
Jawab:

Urutan Prioritas CSS (Cascade & Specificity)
Jika ada Internal CSS, Eksternal CSS, dan Inline CSS pada elemen yang sama → browser akan memilih yang paling spesifik.

Urutannya (dari lemah ke kuat):
A. Eksternal CSS
B. Internal CSS `<style>` 
C. Inline CSS `(style="...")`

# Input CSS
<img src="code tugas css 2.png">

## Input HTML
<img src="code tugas html 3.png">

## Output
<img src="hasil tugas 3.png">

→ Hasil di browser: teks berwarna merah (karena Inline CSS yang paling kuat).

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! `( <p id="paragraf-1" class="text-paragraf"> )`
Jawab:

Jika Elemen Memiliki ID dan Class:
- ID Selector `(#id)` memiliki prioritas lebih tinggi daripada Class Selector `(.class)`.
- Jika keduanya didefinisikan pada elemen yang sama, maka gaya dari ID akan ditampilkan.

# Input CSS
<img src="code tugas css 4.png">

## Input HTML
<img src="code tugas html 4.png">

## Output
<img src="hasil tugas 4.png">

→ Hasil: teks berwarna merah (karena ID lebih spesifik daripada Class).
