# Weblab3

Nama : Eka Maulana Prasetia
Nim  : 312510012
prodi: Teknik Infomatika

 # Membuat dokumen HTML
![Gambar1](Screenshot/Membuat_dokumen_HTML.png)

 # Mendeklarasikan CSS Internal
 ![Gambar2](Screenshot/Mendeklarisasikan_CSS_internal.png)

 # Menambahkan Inline CSS
 ![Gamba3](Screenshot/Menambahkan_inline_CSS.png)

 # Membuat CSS Eksternal
 ![Gambar4](Screenshot/Menambah_css_Eksternal.png)

 # Menambahkan CSS Selector
 ![Gambar5](Screenshot/Menambhahkan_CSS_selector.png)

 # Pertanyaan dan Tugas Praktikum CSS

## 1. Eksperimen Mengubah dan Menambah Properti CSS

Eksperimen dilakukan dengan mengubah dan menambahkan properti CSS untuk mengetahui pengaruhnya terhadap tampilan halaman web.

Contoh kode CSS:

```css
body {
    background-color: #f0f0f0;
    font-family: Arial, sans-serif;
}

h1 {
    color: blue;
    text-align: center;
    font-size: 32px;
}

p {
    color: black;
    font-size: 18px;
    line-height: 1.8;
    background-color: white;
    padding: 15px;
    border: 2px solid blue;
    border-radius: 10px;
}
```

**Penjelasan:**

- `background-color` digunakan untuk mengatur warna latar belakang.
- `font-family` digunakan untuk menentukan jenis huruf.
- `color` digunakan untuk mengatur warna teks.
- `text-align` digunakan untuk mengatur posisi teks.
- `font-size` digunakan untuk mengatur ukuran huruf.
- `line-height` digunakan untuk mengatur jarak antarbaris.
- `padding` digunakan untuk memberikan jarak antara isi elemen dan tepinya.
- `border` digunakan untuk memberikan garis tepi.
- `border-radius` digunakan untuk membuat sudut elemen menjadi melengkung.

**Kesimpulan:** Dengan mengubah dan menambahkan properti CSS, tampilan halaman web dapat dibuat lebih menarik, rapi, dan mudah dibaca.

## 2. Perbedaan Selector `h1` dan `#intro h1`

Selector `h1` digunakan untuk memberikan gaya kepada semua elemen `<h1>` pada halaman HTML.

Contoh:

```css
h1 {
    color: blue;
}
```

Sementara itu, selector `#intro h1` digunakan untuk memberikan gaya kepada elemen `<h1>` yang berada di dalam elemen dengan ID `intro`.

Contoh:

```css
#intro h1 {
    color: red;
}
```

HTML:

```html
<h1>Judul Pertama</h1>

<div id="intro">
    <h1>Judul Kedua</h1>
</div>
```

**Penjelasan:**

- Judul pertama akan berwarna biru.
- Judul kedua akan berwarna merah karena berada di dalam elemen dengan ID `intro`.

**Kesimpulan:** Selector `h1` berlaku untuk semua elemen `<h1>`, sedangkan `#intro h1` hanya berlaku untuk elemen `<h1>` yang berada di dalam elemen dengan ID `intro`.

## 3. Prioritas CSS Internal, Eksternal, dan Inline

CSS dapat ditulis menggunakan tiga cara, yaitu internal CSS, eksternal CSS, dan inline CSS.

Contoh internal CSS:

```html
<style>
    p {
        color: blue;
    }
</style>
```

Contoh eksternal CSS pada file `style.css`:

```css
p {
    color: green;
}
```

Contoh inline CSS:

```html
<p style="color: red;">Saya sedang belajar CSS.</p>
```

**Penjelasan:**

Pada contoh tersebut, teks paragraf akan berwarna merah karena inline CSS memiliki prioritas lebih tinggi daripada deklarasi internal dan eksternal biasa.

Namun, hasil akhir juga dapat dipengaruhi oleh spesifisitas selector, urutan deklarasi, dan penggunaan `!important`.

**Kesimpulan:** Inline CSS umumnya lebih diprioritaskan daripada internal dan eksternal CSS untuk deklarasi biasa yang mengatur properti yang sama pada elemen yang sama. Internal dan eksternal CSS tidak selalu memiliki urutan prioritas tetap karena hasilnya bergantung pada aturan cascade CSS.

## 4. Prioritas Selector ID dan Class

Apabila sebuah elemen HTML memiliki ID dan Class, selector ID memiliki tingkat spesifisitas lebih tinggi daripada selector Class jika keduanya mengatur properti yang sama.

Contoh HTML:

```html
<p id="paragraf-1" class="text-paragraf">
    Saya sedang belajar CSS.
</p>
```

Contoh CSS:

```css
#paragraf-1 {
    color: red;
}

.text-paragraf {
    color: blue;
}
```

**Penjelasan:**

Pada contoh tersebut, teks paragraf akan berwarna merah karena selector `#paragraf-1` menggunakan ID yang memiliki tingkat spesifisitas lebih tinggi daripada selector `.text-paragraf` yang menggunakan Class.

Perbedaan selector:

- `p` digunakan untuk memilih elemen paragraf.
- `.text-paragraf` digunakan untuk memilih elemen berdasarkan Class.
- `#paragraf-1` digunakan untuk memilih elemen berdasarkan ID.

**Kesimpulan:** Selector ID lebih diprioritaskan daripada selector Class ketika keduanya mengatur properti yang sama dan tidak ada aturan cascade lain yang mengubah hasilnya. Jika keduanya mengatur properti yang berbeda, kedua deklarasi dapat diterapkan secara bersamaan.

## Kesimpulan Umum

CSS digunakan untuk mengatur tampilan halaman web agar lebih menarik dan terstruktur. Dalam penggunaannya, kita perlu memahami properti CSS, jenis selector, serta aturan prioritas atau cascade CSS. Dengan memahami konsep tersebut, kita dapat mengatur tampilan halaman web sesuai kebutuhan.
