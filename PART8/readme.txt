Materi: Image Map di HTML

Pengertian Image Map
Image map adalah sebuah gambar yang memiliki area-area tertentu yang dapat diklik, di mana setiap area mengarahkan pengguna ke tautan (link) berbeda. Dengan image map, satu gambar dapat memiliki beberapa link tanpa perlu membagi gambar tersebut menjadi beberapa bagian kecil.

Jenis Image Map
1. Client-side Image Map: Map ini didefinisikan di dalam HTML dan di proses oleh browser. Semua logika ada di sisi klien (browser), sehingga lebih cepat dan sederhana.
2. Server-side Image Map: Map ini didefinisikan di server, di mana server menentukan area yang dapat diklik dan tanggapannya.

Pada umumnya, yang sering digunakan adalah **Client-side Image Map**.

Cara Membuat Image Map
Untuk membuat image map di HTML, ada beberapa tag utama yang digunakan:

1. <img>: Menampilkan gambar.
2. <map>: Mendefinisikan image map.
3. <area>: Menentukan area tertentu yang bisa diklik dalam image map.

Struktur Dasar
html
<img src="gambar.jpg" usemap="#peta" alt="Deskripsi Gambar">

<map name="peta">
  <area shape="rect" coords="34,44,270,350" alt="Area 1" href="https://link1.com">
  <area shape="circle" coords="120,150,100" alt="Area 2" href="https://link2.com">
  <area shape="poly" coords="130,130,130,180,180,180,180,130" alt="Area 3" href="https://link3.com">
</map>


Penjelasan
1. <img src="gambar.jpg" usemap="#peta" alt="Deskripsi Gambar">
   Gambar akan ditampilkan, dan `usemap` menghubungkannya ke image map yang memiliki `name="peta"`.
   
2. <map name="peta">
   Mendefinisikan area interaktif pada gambar. Name `peta` menghubungkan image map dengan gambar yang menggunakan atribut `usemap`.

3. <area>
   Menentukan area klik dalam gambar. Setiap area memiliki beberapa atribut:
   - shape: Menentukan bentuk area klik. Nilainya bisa `rect` (persegi panjang), `circle` (lingkaran), atau `poly` (poligon).
   - coords: Kordinat area. Nilai yang diberikan tergantung pada bentuknya:
     - rect: x1, y1, x2, y2 (pojok kiri atas dan pojok kanan bawah).
     - circle: x, y, radius (pusat lingkaran dan jari-jari).
     - poly: Serangkaian titik x, y yang terhubung membentuk poligon.
   - alt: Teks alternatif, untuk accessibility.
   - href: Tautan yang akan dituju ketika area tersebut diklik.

#### Contoh Kode Lengkap
Berikut adalah contoh image map dengan 3 area yang bisa diklik:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Image Map</title>
</head>
<body>
    <h2>Contoh Penggunaan Image Map</h2>

    <img src="peta.jpg" alt="Peta Dunia" usemap="#duniapeta" width="600" height="400">

    <map name="duniapeta">
        <!-- Area Persegi Panjang -->
        <area shape="rect" coords="34,44,270,350" href="https://example.com/area1" alt="Area 1">
        
        <!-- Area Lingkaran -->
        <area shape="circle" coords="300,200,50" href="https://example.com/area2" alt="Area 2">
        
        <!-- Area Poligon -->
        <area shape="poly" coords="400,300,500,300,450,350" href="https://example.com/area3" alt="Area 3">
    </map>

</body>
</html>
```

Atribut Tambahan
1. target: Jika ingin membuka tautan di tab atau jendela baru, bisa ditambahkan ke tag `<area>`.
   
   <area shape="rect" coords="34,44,270,350" href="https://example.com" target="_blank">
   

2. nohref: Jika ada area yang tidak ingin dijadikan tautan, tambahkan `nohref`.
  
   <area shape="rect" coords="34,44,270,350" nohref alt="No Link Area">
   

Keuntungan Menggunakan Image Map
- Penghematan Ruang: Dapat menggunakan satu gambar dengan banyak area klik tanpa harus membagi gambar tersebut.
- Interaktif: Menambahkan interaktivitas pada gambar dengan navigasi yang lebih kaya.
- Penggunaan yang Sederhana: Cukup dengan beberapa tag HTML, Anda bisa membuat gambar yang lebih interaktif.

Kekurangan
- Kurang Responsif: Tidak selalu responsif untuk layar yang berbeda-beda, sehingga perlu penyesuaian lebih lanjut dengan CSS atau JavaScript untuk pengalaman yang optimal di perangkat seluler.

Kesimpulan
Image map di HTML adalah cara yang efektif untuk membuat gambar yang interaktif dengan beberapa area klik. Dengan menggunakan tag `<map>` dan `<area>`, kita bisa mendefinisikan berbagai area dalam satu gambar yang bisa mengarahkan pengguna ke berbagai tautan.

Studi Kasus
Misalnya, Anda memiliki peta interaktif untuk situs wisata dan setiap kota di peta dapat diklik untuk mendapatkan informasi lebih lanjut tentang kota tersebut.

