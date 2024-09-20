Belajar HTML Dasar Part 5 - Pembahasan Link, Relative dan Absolute URL, Bookmark di HTML
.
Tentang link:
- Saat membuat Web, biasanya kita akan membuat banyak sekali halaman HTML
- Untuk berpindah dari satu halaman ke halaman lain, kita biasanya jarang melakukannya secara manual dengan cara mengetikkannya di search bar Web Browser
- HTML memiliki fitur Link (Tautan), dimana kita bisa meng-klik Link tersebut, dan berpindah ke halaman HTML lain
- Link tidak harus dalam bentuk Text, Link juga bisa dalam bentuk Gambar misalnya (yang akan kita bahas di materi Image)
.
Tag a:
- Untuk membuat Link di HTML, kita bisa menggunakan tag a
- Isi konten tag a adalah isi dari tampilan Link, bisa Text atau yang lainnya
- Tag a memiliki attribute href, yang berisi lokasi tujuan Link tersebut
- Tag a juga memiliki attribute target, yang digunakan sebagai target jendela Web Browser, kita bisa gunakan nilai :target=”_self”, artinya halaman akan ditampilkan di halaman yang sama, ini adalah bawaan default target=”_blank”, artinya halaman akan ditampilkan di jendela baru di Browser
- Tag a juga memiliki attribute title, untuk menuliskan judul yang keluar ketika mouse berada di atas Link tersebut
.
Absolut URL
.
- Saat kita menulis halaman tujuan dari href di Link, kita bisa menggunakan absolute URL
- Absolute URL merupakan alamat lengkap sebuah tujuan Link
- Dalam absolute URL, kita wajib menuliskan seluruh detail domain dan halaman yang dituju, misal:
https://youtube.com/SoetrisnoSoekarno
https://facebook.com/SoetrisnoSoekarno
https://instagram.com/SoetrisnoSoekarno
- Kelebihan menggunakan Absolute URL adalah, kita bisa membuat Link menuju domain yang berbeda dengan website yang kita buat
.
Relative URL:
.
- Relative URL adalah lokasi href dimana tetap menggunakan domain website saat ini
- Relative URL memiliki dua format, bisa diawali dengan /, atau tidak diawali dengan /
- Misal sekarang kita berada di halaman http://127.0.0.1/belajar-link/index.html , lalu kita memiliki link sebagai berikut :
hello.html, artinya akan menuju ke http://127.0.0.1/belajar-link/hello.html
/hello.html, artinya akan menuju ke http://127.0.0.1/hello.html 
ss/hello.html, artinya akan menuju ke http://127.0.0.1/belajar-link/ss/hello.html 
. 
Bookmark
.
- Pada kasus halaman web yang sangat panjang, ada bagusnya kita menggunakan Bookmark
- Bookmark adalah link yang bisa digunakan untuk menampilkan HTML element dengan id tertentu
- Bookmark menggunakan # pada href, misal jika kita menggunakan index.html#tris, artinya ketika membuka halaman index.html, maka Web Browser akan otomatis menampilkan pada posisi HTML Element dengan id tris
- Jika kita ingin membuat link di halaman HTML itu sendiri, kita bisa langsung buat Link dengan href langsung berisi #bookmark nya
