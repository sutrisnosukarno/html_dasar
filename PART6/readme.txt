Belajar HTML Dasar Part 6: Blok dan Inline di HTML
.
- Di dalam HTML, semua element memiliki nilai display, tergantung dari jenis element yang digunakan
- Ada dua nilai untuk display, block dan inline
.
Display Block
.
- Element yang memiliki nilai display block, selalu dimulai dengan baris baru. 
- Web browser secara otomatis menambahkan jarak / margin sebelum dan setelah element
- Dan element dengan nilai display block, selalu mengambil ukuran penuh yang tersedia, yag artinya dia akan full dari kiri dan kanan
- Contoh tag yang menggunakan nilai display block adalah : h1-h6, p, header, body, ul, li, ol, table, form, dan lain-lain
.
Display Inline
.
- Sedangkan dalam display inline, element tidak dimulai dengan baris baru
- Selain itu dalam display inline, element hanya menggunakan ukuran seperlunya saja
- Contoh tag yang menggunakan nilai display inline : a, b, i, em, button, strong, input, dan lain-lain
.
Elemen Div
.
- Div adalah salah satu tag di HTML yang memiliki nilai display block
- Div biasanya digunakan sebagai container (wadah) untuk beberapa element HTML
- Div banyak digunakan ketika kita ingin membedakan bagian-bagian dalam element HTML, misal ada bagian menu, content, footer, navigasi, header dan lain-lain
- Biasanya semua itu dibungkus dalam Div
.
contoh latihan Div

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Latihan Div di HTML</title>
</head>
<body>
    <div id="header">
        <h3>Ini adalah Header</h3>
    </div>
    <div id="menu">
        <ul>
            <li>Menu1</li>
            <li>Menu2</li>
            <li>Menu3</li>
        </ul>
    </div>
    <div id="content">
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi, esse voluptatum ullam voluptas accusamus expedita perferendis alias enim nihil possimus ea quos cum, reprehenderit odio delectus eligendi omnis? Voluptate, accusamus.</p>
    </div>
    <div id="footer">
        <p>Ini adalah Footer</p>
    </div>
</body>
</html>
.
Elemen SPAN 
.
- Jika Div menggunakan nilai display block, ada lagi tag span, yang menggunakan nilai display inline
- Span biasa digunakan pada kasus kita ingin menggunakan display inline, misal kita mau membuat tulisa Belajar HTML Dasar, namun tiap kata berbeda warna
- Hal itu tidak bisa dilakukan jika menggunakan p, karena p akan mengubah seluruh warna tulisan
- Kita bisa gunakan span di tiap kata, agar bisa menambah style di tiap span



