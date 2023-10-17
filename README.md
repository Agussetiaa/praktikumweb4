# praktikumweb4
## Langkah-langkah Praktikum
- Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1> Box Element</h1>
    <header>
</body>
</html>
```

- Membuat Box Element
- Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.

```
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
</section>
```

- CSS Float Property Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.
```
<style>
div {
    float:left;
    padding: 10px;
}
.div1 {
    background: red;
}
.div2 {
      background: yellow;
}
.div3 {
      background: green;
}
</style>
```
Kemudian buka browser untuk melihat hasilnya.

<img width="476" alt="111" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/00c78a6a-86dd-4ab3-b2a6-94df96440463">

- Mengatur Clearfix Element
- Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya.

- Tambahkan element div lainnya seteleah div3 seperti berikut.

```
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
</section>
```
```
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```
- Kemudian atur property clear pada CSS, seperti berikut.
```
.div4 {
background-color: blue;
clear: left;
float: none;
}
```

- Selanjutnya buka browser dan refresh kembali.

<img width="478" alt="222" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/6c2fdcae-6f2c-4bcc-b334-fae20e3b9695">

- Lakukan eksperimen terhadap penggunaan property clear dengan nilai lainnya (left, both, right),
- dan amati perubahannya.

## Membuat Layout Sederhana
- Kita akan membuat layout web sederhana seperti gambar berikut.

gambar

## Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        
    </div>
</body>
</html>
```

- Kemudian buat kerangka layout dengan semantics element seperti berikut.

<img width="396" alt="Screenshot 2023-10-17 200907" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/f46ca0ad-22fc-4d2d-8474-b846e1f2cbb7">

- Kemudian tulis kode berikut.
```
<header>
    <h1>Layout Sederhana</h1>
</header>
<nav>
    <a href="home.html" class="active">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
</nav>
    <section id="hero"></section>
    <section id="wrapper">
    <section id="main"></section>
    <aside id="sidebar"></aside>
    </section>
<footer>
    <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

- Kemudian buka browser dan lihat hasilnya.

<img width="478" alt="Screenshot 2023-10-17 081155" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/219efd55-c99f-4fa7-80f5-757fab89b04f">


## Kemudian tambahkan kode CSS untuk membuat layoutnya.
```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
    padding: 20px;
}
header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

- Kemudian lihat hasilnya pada browser.

<img width="480" alt="Screenshot 2023-10-17 081820" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/48633152-654d-4496-9113-3956abd559c0">

## Membuat Navigasi
- Kemudian selanjutnya mengatur navigasi.
```
/* navigasi */
nav {
    display: block;
    background-color: #1f5faa;
}
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
```
- Kemudian lihat hasilnya.

<img width="479" alt="Screenshot 2023-10-17 082055" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/4413eae6-c05a-477d-8155-26a0d3f9b402">

## Membuat Hero Panel.
- Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.
```
 <section id="hero">
                <h1>Hello World!</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
                elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
                vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
                pretium ac.</p>
                <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
            </section>
```

```
/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
    #hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
}
    #hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
```

<img width="960" alt="Screenshot 2023-10-17 082914" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/c34fe4e5-2141-4296-aed8-be641b7e1804">

## Mengatur Layout Main dan Sidebar
- Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
```
/* main content */
#wrapper {
    margin: 0;
}
#main {
    float: left;
    width: 640px;
    padding: 20px;
}
    /* sidebar area */
    #sidebar {
    float: left;
    width: 260px;
    padding: 20px;
}
```

## Membuat Sidebar Widget
- Kemudian selanjutnya menambahkan element lain dalam sidebar.
```
<aside id="sidebar">
                <div class="widget-box">
                <h3 class="title">Widget Header</h3>
                <ul>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                <li><a href="#">Widget Link</a></li>
                </ul>
                </div>
                <div class="widget-box">
                <h3 class="title">Widget Text</h3>
                <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
                arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
                pharetra est nunc, nec pretium nunc pretium ac.</p>
                </div>
            </aside>
```

- Kemudian tambahkan CSS.
```
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
    }
    .widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
    }
    .widget-box ul {
    list-style-type:none;
    }
    .widget-box li {
    border-bottom:1px solid #eee;}
    .widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
    }
    .widget-box li:hover a {
    background-color:#eee;
    }
    .widget-box p {
    padding:15px;
    line-height:25px;
    }
```


## Mengatur Footer
- Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
```
/* footer */
    footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
    }
```
gambar

## Menambahkan Element lainnya pada Main Content.
```
 <section id="main">
                    <div class="row">
                    <div class="box">
                    <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
                    class="image-circle">
                    <h3>Heading</h3>
                    <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                    euismod.</p>
                    <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                    <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
                    class="image-circle">
                    <h3>Heading</h3>
                    <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                    euismod.</p>
                    <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                    <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
                    class="image-circle">
                    <h3>Heading</h3>
                    <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                    euismod.</p>
                    <a href="#" class="btn btn-default">View detail</a>
             </div>
         </div>
 </section>
```

- Kemudian tambahkan CSS.
```
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;padding:0 10px;
    text-align:center;
    }
    .box h3 {
    margin: 15px 0;
    }
    .box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
    }
    box img {
    border: 0;
    vertical-align: middle;
    }
    .image-circle {
    border-radius: 50%;
    }
    .row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
    }
    .row:after, .row:before,
    .entry:after, .entry:before {
    content:'';
    display:table;
    }
    .row:after,
    .entry:after {
    clear:both;
    }
   
```

- Lihat hasilnya dibrowser.

<img width="960" alt="Screenshot 2023-10-17 083639" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/7240eca7-6dd4-49ba-af86-72710eb4c1d3">

## Menambahkan Content Artikel
- Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
```
 <hr class="divider" />
            <article class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
            elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
            vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
            pretium ac.</p>
            </article>
            <hr class="divider" />
            <article class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
            class="right-img">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
            elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
            vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
            pretium ac.</p>
            </article>
```

- Kemudian tambahkan CSS.
```
.divider {
        border:0;
        border-top:1px solid #eeeeee;
        margin:40px 0;
        }
        /* entry */
        .entry {
        margin: 15px 0;
        }
        .entry h2 {
        margin-bottom: 20px;}
        .entry p {
        line-height: 25px;
        }
        .entry img {
        float: left;
        border-radius: 5px;
        margin-right: 15px;
        }
        .entry .right-img {
        float: right;
        }
```

<img width="960" alt="Screenshot 2023-10-17 084122" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/2c077b4e-e90c-4e6b-827a-3d924bf9d339">

### Pertanyaan dan Tugas
### 1. Tambahkan Layout untuk menu About
### => buat single layout yang berisi deskripsi, portfolio, dll


### 2. Tambahkan layout untuk menu Contact
### => yang berisi form isian: nama, email, message, dll

<img width="477" alt="Screenshot 2023-10-17 203348" src="https://github.com/Agussetiaa/praktikumweb4/assets/115542822/8abae999-7edc-4492-b6a9-39cca198d4fb">






