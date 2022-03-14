# Web2Lab2

**Nama    : Aning Kinanti** <br>
**NIM     : 312010364** <br>
**Kelas   : TI.20.A2** <br>
**Matkul  : Pemrograman Web** <br>

## Belajar CSS Dasar

### 1. Membuat dokumen HTML
Buatlah dokumen HTML seperti contoh dibawah ini :
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>CSS Dasar</title>
    </head>
    <body>
        <header>
            <h1>CSS Internal dan <i>Inline CSS</i></h1>
        </header>
        <nav>
            <a href="lab2_css_dasar.html">CSS DASAR</a>
            <a href="lab2_css_eksternal.html">CSS EKSTERNAL</a>
            <a href="lab1_tag_dasar.html">HTML DASAR</a>
        </nav>

        <!-- CSS ID SELECTOR -->
        <div id="intro">
            <h1>Hello World</h1>
            <p> Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman 
                Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat 
                adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML 
                dan CSS.</p>

            <!-- CSS CLASS SELECTOR -->
            <a href="#intro" class="button btn-primary">Informasi Selengkapnya.</a>

        </div>
    </body>
    </html>
```
<br>

Ini adalah hasil dari sintaks diatas :
![Gambar 1](screenshot/ss1.PNG) <br>

### 2. Mendeklarasikan CSS Internal
Penulisan Internal CSS menggunakan tag `<style>` yang diletakkan pada `<head>` dokumen. <br>
CSS selector berupa elemen selector berlaku pada semua elemen tersebut. <br>
Elemen selector dideklarasikan berdasarkan tag HTML seperti :
```
body {color:blue;}
p {font-family:"sans-serif"}
h1 {text-align:center;color:red';}
```
<br>

Selanjutnya tambahkan deklarasi CSS Internal pada bagian head seperti contoh dibawah ini :
```
    <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
    <!-- menyisipkan link -->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
    <style>
        body {
            font-family:'Open Sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom: 1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #800000;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color: #6d6a6b;
        }
    </style>
    </head>
```
<br>

Ini adalah hasil dari sintaks diatas :
![Gambar 2](screenshot/ss2.PNG) <br>

### 3. Menambahkan Inline CSS
Inline CSS dengan menambahkan kode CSS pada tag HTML sebagai atribut dan value. <br>
Penempatan CSS secara inline hanya akan mempengaruhi satu bagian baris kode. <br>
Kemudian tambahkan deklarasi inline CSS pada tag `<p>` seperti berikut.:
```
    <p style="text-align: center; color: #ccd8e4;">
```
<br>

Ini adalah hasil dari sintaks diatas :
![Gambar 3](screenshot/ss3.PNG) <br>

### 4. Membuat CSS Eksternal
Penulisan Eksternal CSS menggunakan tag `<link>` menggunakan atribut href untuk merujuk 
kepada file css yang diletakkan pada `<head>` dokumen. <br>
Buatlah file baru dengan nama "style_eksternal.css" kemudian buatlah deklarasi CSS seperti berikut. <br>
```
    nav {
    background: #f08080;
    color: #fff;
    padding: 10px;
    }

    nav a {
        color: #fff;
        text-decoration: none;
        padding: 10px 20px;
    }

    nav .active,
    nav a:hover {
        background: #800000;
    }
```
<br>

Ini adalah hasil dari sintaks diatas :
![Gambar 4](screenshot/ss4.PNG) <br>


