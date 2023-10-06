# Nama  : Roswanda Nuraini

# NIM  : 312210328

# Kelas  : TI.22.A3

# <p align="center">Praktikum2 : CSS Dasar</p>

# Membuat Dokumen HTML

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

  ![Screenshot (334)](https://github.com/roswanda11/lab2web/assets/115516632/26c641f1-b52d-40d0-9d61-5ec5b16b96b7)

  - Maka hasilnya akan seperti berikut

![Screenshot (333)](https://github.com/roswanda11/lab2web/assets/115516632/f70dcb97-a8f8-4a4b-962b-0772746a3e85)

# Mendeklarasikan CSS Internal

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
                    
![Screenshot (337)](https://github.com/roswanda11/lab2web/assets/115516632/51d7e658-2040-4822-b3d1-c983588cdf07)

- Maka hasilnya akan seperti berikut
  
![Screenshot (336)](https://github.com/roswanda11/lab2web/assets/115516632/c0652848-a37e-45ca-ae9b-8d9e8577e68d)

- CSS internal adalah css yang filenya di letakan dalam html dengan pendeklarasian style.

# Menambahkan Inline CSS

- Menambahkan Inline CSS Kemudian tambahkan deklarasi inline CSS pada tag

          <p style="text-align: center; color: cc8e4;>

![Screenshot (340)](https://github.com/roswanda11/lab2web/assets/115516632/733d05a3-a249-4979-b62f-ff6f716504a3)

- CSS inline adalah css yang pendeklarasiannya di dalam elemen HTML dengan code style inline memiliki prioritas lebih kuat di banding internal dan external.
  
          <p style="text-align: center; color: palevioletred;">Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
                      Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
                  adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
                  dan CSS.</p>

# Membuat CSS Eksternal

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
  
![Screenshot (344)](https://github.com/roswanda11/lab2web/assets/115516632/7f1fb22e-b562-4edc-aef1-382494919efc)

- CSS ekternal adalah CSS yang file di tempatkan di luar file HTML dengan menambahkan link dalam HTML agar tertaut dengan file CSS

# Menambahkan CSS Selector

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
          
  ![Screenshot (350)](https://github.com/roswanda11/lab2web/assets/115516632/8ed11abe-eeaf-4dff-a2d1-a73451d49538)

- CSS Selector terdiri atas selector ID, Selector Class, Dan Selector elemen Selector ID pendeklarasiannya yaitu dengan (#), Sedangkan Class pendeklarasiannya yaitu dengan (.), Dan Selector elemen pendeklarasiannya dengan elemen HTML sebagai contoh (p) yang akan di beri gaya pada CSS.
          

