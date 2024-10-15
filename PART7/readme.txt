Belajar HTML Dasar Part 7 - Menampilkan Gambar di HTML
.
- Gambar dapat kita tambakan di HTML dengan menggunakan tag <img>. Tag ini memiliki atribut wajib, yakni src.
- Jika kita tidak mengisi atribut src, maka gambar tidak akan ditampilkan.
- Alamat URL gambar pada atribut src dapat berupa URL maupun alamat path. Lalu tag <img> harus ditutup dengan menambahkan garis miring.
----------
Contoh: buat file html dengan nama gambar1.html dan simpan salah satu gambar di folder utama / 1 folder dengan file html
----------

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Latihan Gambar satu folder di HTML - Sutrisno Sukarno</title>
</head>
<body>
    <img src="gambardiluar.jpeg" alt="latihan gambar 1">
</body>
</html>

============
menambahkan size di dalam gambar:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Latihan Gambar satu folder di HTML - Sutrisno Sukarno</title>
</head>
<body>
    <img src="gambardiluar.jpeg" alt="latihan gambar 1" style="width: 100px; height: 100px;">
</body>
</html>

=============

menambahkan gambar dengan sumber gambar dari internet:

<img src="https://samacosemestaniaga.com/wp-content/uploads/2023/05/9.jpg" alt="gambar dari internet" style="width: 200px;height: 200px;">

=============

Membuat background Image
==============
<body style="background-image: url(gambardiluar.jpeg);">

--------------
Silahkan dicoba beberapa opsi bg color sbb:

1. 
<style>
body {
  background-image: url('example_img_girl.jpg');
  background-repeat: no-repeat;
}
</style>

2.
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>

3.

<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>

4. 

<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
}
</style>

==================



