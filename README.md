<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Roswanda Nuraini</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210328</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A3</td>
  </tr>
</table>

# <p align="center">Praktikum2 : CSS Dasar</p>

# Langkah 1

## Membuat Dokumen HTML

- Buka VS Code dan buat file HTML baru. Setelah itu buat struktur HTML
  
Disini sudah terdapat file Dokumen HTML yang belom terdapat file css nya

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Dasar</title>
    </head>
    <body>
        <header>
            <h1>CSS Internal dan <i>Inline CSS</i></h1>
        </header>
        <nav>
            <a href="lab2_css_dasar.html">CSS Dasar</a>
            <a href="lab2_css_eksternal.html">CSS Eksternal</a>
            <a href="lab1_tag_dasar.html">HTML Dasar</a>
        </nav>
        <!-- CSS ID Selector -->
        <div id="intro">
            <h1>Hello World</h1>
            <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
    Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
    adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
    dan CSS.</p>
            <!-- CSS Class Selector -->
            <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
        </div>
    </body>
    </html>

  - Maka hasilnya akan seperti berikut

![Screenshot (333)](https://github.com/roswanda11/lab2web/assets/115516632/f70dcb97-a8f8-4a4b-962b-0772746a3e85)

# Langkah 2

## Mendeklarasikan CSS Internal

- Kemudian tambahkan deklarasi CSS Internal di dalam html seperti berikut pada bagian head

      <head> 
          <style>
              body {
                   font-family: 'Open Sans', sans-serif;
                   }
              header {
                   min-height: 80px;
                   border-bottom: 1px solid #77ccef;
                   }
              h1 {
                   font-size: 24px;
                   color: slateblue;
                   text-align: center;
                   padding: 20px 10px;
              }
              h1 i {
                   color:blueviolet;
                   }
          </style>
      </head>

- Maka hasilnya akan seperti berikut
  
![Screenshot (336)](https://github.com/roswanda11/lab2web/assets/115516632/c0652848-a37e-45ca-ae9b-8d9e8577e68d)

- CSS internal adalah css yang filenya di letakan dalam html dengan pendeklarasian style.

# Langkah 3

## Menambahkan Inline CSS

- Menambahkan Inline CSS Kemudian tambahkan deklarasi inline CSS pada tag

          <p style="text-align: center; color: cc8e4;>

- Maka hasilnya sebagai berikut

![Screenshot (340)](https://github.com/roswanda11/lab2web/assets/115516632/733d05a3-a249-4979-b62f-ff6f716504a3)

- CSS inline adalah css yang pendeklarasiannya di dalam elemen HTML dengan code style inline memiliki prioritas lebih kuat di banding internal dan external.
  
          <p style="text-align: center; color: palevioletred;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
                      Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
                  adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
                  dan CSS.</p>

# Langkah 4

## Membuat CSS Eksternal

- Membuat CSS Eksternal dengan membuat file baru dengan nama style_eksternal.css kemudian buat deklarasi css seperti berikut ini.

      nav{
          background: #ff595e;
          color: white;
          padding: 15px;
      }
      nav a{
          color: #fff;
          text-decoration: none;
          padding: 15px 20px;
      }
      nav .active,
      nav a:hover{
          background: black;
      }

- Kemudian tambahkan <link untuk merujuk File CSS yang telah dibuat pada bagian Head

        <head>
            <!--menyisipkan css eksternal-->
            <link rel="stylesheet" href="style_eksternal.css" type="text/css">
        </head>

- Maka hasilnya sebagai berikut
  
![Screenshot (353)](https://github.com/roswanda11/lab2web/assets/115516632/98587bfe-9bfc-4955-80e4-e8b12295b195)

- CSS ekternal adalah CSS yang file di tempatkan di luar file HTML dengan menambahkan link dalam HTML agar tertaut dengan file CSS

# Langkah 5

## Menambahkan CSS Selector

- Selanjutnya menambahkan CSS Selector menggunkan ID dan class Selector pada file style_eksternal.css dan menambahkan kode seperti berikut

            /* Menambahkan ID Selector */
            #intro {
                background: #d9f1fc;
                border: 1px solid #099249;
                min-height: 100px;
                padding: 10px;
            }
            #intro h1 {
                text-align: left;
                border: 0;
                color:#0d6e46;
            }
            
            /* Menambahkan Class Selector */
            .button {
                padding: 15px 20px;
                background: #bebcbd;
                color: #fff;
                display: inline-block;
                margin: 10px;
                text-decoration: none;
            }
            button .active
            button:hover{
                background: #fff;
            }
            .btn-primary {
                background: #e91e4a;
            }
            .btn-primary:hover{
                animation-duration: 10ms;
                background: #099249;
            }

- Maka hasilnya sebagai berikut
          
![Screenshot (351)](https://github.com/roswanda11/lab2web/assets/115516632/b4741c25-cfe9-43ca-9efa-35e622d3a9b3)

- CSS Selector terdiri atas selector ID, Selector Class, Dan Selector elemen Selector ID pendeklarasiannya yaitu dengan (#), Sedangkan Class pendeklarasiannya yaitu dengan (.), Dan Selector elemen pendeklarasiannya dengan elemen HTML sebagai contoh (p) yang akan di beri gaya pada CSS.

# Langkah 6

## Melakukan Validasi dokumen CSS dengan mengakses https://jigsaw.w3.org/css-validator/

![Screenshot (363)](https://github.com/roswanda11/lab2web/assets/115516632/88ac779f-2bdf-436e-89cc-f0caad87c4e5)

- Maka hasilnya sebagai berikut

![Screenshot (362)](https://github.com/roswanda11/lab2web/assets/115516632/1f1b5cc8-4b52-4e17-8b8a-959873698e99)

# Pertanyaan dan Tugas

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

<b>JAWABAN</b>

      <link rel="stylesheet" href="w.css">
      
      <h1 class="title">Roswanda Nuraini</h1>
      <p class="text">Praktikum 2- CSS Dasar</p>

### contoh hasil dan code
![Screenshot (359)](https://github.com/roswanda11/lab2web/assets/115516632/0e8c9d33-b582-4303-b8d1-1767a67925e4)

![Screenshot (360)](https://github.com/roswanda11/lab2web/assets/115516632/b20e9685-cade-40c5-8b4e-25baadded060)

- Pada contoh ini, terdapat elemen ```<h1> dengan class "title"``` dan ```elemen <p> dengan class "text"```. Class tersebut akan digunakan sebagai selector dalam CSS untuk mengubah properti dan nilai. Dalam file CSS (style.css), terdapat aturan CSS yang dideklarasikan untuk ```class "title" dan "text"```. Aturan tersebut mengubah properti ```"color"``` pada elemen dengan class tersebut. Anda dapat mengubah nilai properti ```"color"``` pada file CSS sesuai keinginan Anda untuk melihat perubahan yang terjadi pada ```judul (h1)``` dan ```paragraf (p)``` dalam hal warna teks.

2. Apa perbedaan pendeklarasian CSS elemen ```h1 {...}``` dengan ```#intro h1 {...}```? berikan penjelasannya!

<b>JAWABAN</b>
 
- ```h1 {...}``` : Deklarasi ini akan merubah semua elemen "h1"

- ```#intro h1 {...}``` : Deklarasi ini lebih spesifik, maksud nya adalah pendeklarasian yang mengacu kepada pemberian atribut pada elemen "h1" dengan menambahkan id "intro"
   
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

<b>JAWABAN</b>

- Ketika kita mendeklarasikan secara bersamaan antara ```INTERNAL EKSTERNAL``` dan ```INLINE``` yang akan ditampilkan pada Browser adalah ```INLINE``` Karena ```INLINE``` Memiliki prioritas dibanding ```EKSTERNAL``` atau pun ```INTERNAL``` seperti contoh yang saya buat, saya membuat dokumen baru HTML kemudian saya buat Elemen ```{h1}```yang kemudian saya akan deklarasikan di CSS ```INTERNAL EKSTERNAL``` dan juga ```INLINE``` Dengan property ```{color}``` dengan warna yang berbeda,jika ```INTERNAL``` {color: red} sementara ```EKSTERNAL``` {color:blue;} dan ```INLINE``` {color: green;} yang terpanggil dibrowser adalah ```INLINE``` karena memiliki prioritas.

### contoh hasil dan code

![Screenshot (361)](https://github.com/roswanda11/lab2web/assets/115516632/fce95e5e-b184-41ad-96a7-dc367f7fb3da)

- Di atas adalah deklarasi <b>INLINE</b> dan <b>INTERNAL</b> sementara foto di bawah adalah deklarasi <b>EKSTERNAL</b> nya
  
![Screenshot (355)](https://github.com/roswanda11/lab2web/assets/115516632/694b34f7-d47f-448f-a483-689a248a037a)

- Jadi yang terpanggil adalah <b>CSS INLINE</b> karena memiliki prioritas tinggi dibanding CSS deklarasi lain nya.

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya!

<b>JAWABAN</b>

      ( <p id="paragraf-1" class="text-paragraf"> )

- Yang terpanggil dibrowser adalah <b>ID</b> karena <b>ID</b> bersifat unik berbeda dengan <b>Class</b> .<b>Class</b> bisa digunakan banyak sementara <b>ID</b> hanya tertentu saja itu kenapa <b>ID</b> unik dan yang terpanggil di browser adalah <b>ID</b> .

### contoh hasil dan code 

![Screenshot (357)](https://github.com/roswanda11/lab2web/assets/115516632/dcb23999-8e20-4ec2-9c1b-cc66ce892998)

- Disitu saya menambahkan property {color} dan {text-align} untuk <b>ID {color: orchid}</b> dan {text-align: center} sementara <b>Class yaitu {color:palegreen}</b> dan <b>{text-align: left}</b>. Namun yang terpanggil di browser adalah <b>ID</b> yang property nya <b>{color: orchid}</b> dan juga <b>{text-align: center}</b>


