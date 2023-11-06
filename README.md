# Lab6Web

# 1. Membuat file html dengan nama `lab6_css_framework`

# 2. Membuat Layout Sederhana menggunakan Bootstrap

## Pertama, kita mulai dengan tamplate codingan html dari bootstrap. Sebagai berikut:

```
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">

    <title>Hello, world!</title>
  </head>
  <body>
    <h1>Hello, world!</h1>

    <!-- Optional JavaScript; choose one of the two! -->

    <!-- Option 1: Bootstrap Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>

    <!-- Option 2: Separate Popper and Bootstrap JS -->
    <!--
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js" integrity="sha384-IQsoLXl5PILFhosVNubq5LC7Qb9DXgDA9i+tQ8Zj3iwWAwPtgFTxbJ8NT4GN1R8p" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.min.js" integrity="sha384-cVKIPhGWiC2Al4u+LWgxfKTRIcfu0JTxR+EQDz/bgldoEyl4H0zUF0QKbrJ0EcQF" crossorigin="anonymous"></script>
    -->
  </body>
</html>
```
Nah, disini saya hanya memakai yang option 1. Kenapa? Karena, lebih mudah. satu file JavaScript mencakup Bootstrap dan Popper.js.

## Kedua, Saya mulai membuat Navbar

### Berikut CODE nya:

```
<!-- Navbar -->
    <nav
      class="navbar navbar-expand-lg navbar-dark shadow fixed-top"
      style="background-color: #001c30"
    >
      <div class="container">
        <a class="navbar-brand" href="#">Aliyah Asmarani</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavAltMarkup"
          aria-controls="navbarNavAltMarkup"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
          <div class="navbar-nav ms-auto">
            <a class="nav-link" aria-current="page" href="#home"
              >Home <i class="bi bi-house-heart-fill"></i
            ></a>
            <a class="nav-link" href="#about"
              >About <i class="bi bi-person-heart"></i
            ></a>
            <a class="nav-link" href="#hobi"
              >Hobi <i class="bi bi-palette-fill"></i
            ></a>
            <a class="nav-link" href="#kontak"
              >Contact <i class="bi bi-person-lines-fill"></i
            ></a>
          </div>
        </div>
      </div>
    </nav>
    <!-- Akhir Navbar -->
```

### OUTPUT nya:

![image](https://github.com/Aliyahasmarani/Lab6Web/assets/115197672/32240d85-e0b4-4e46-918c-0eaa2a922bef)

### PENJELASAN NAVBAR

Di bagian navbar, saya juga memakai tamplate dari bootstrap. 

`-> <nav>: Ini adalah elemen HTML yang digunakan untuk membuat bagian Navbar, yang biasanya berisi tautan menu dan judul situs web.`

`-> class="navbar navbar-expand-lg navbar-dark shadow fixed-top" style="background-color: #001c30": Ini adalah atribut yang digunakan untuk mengatur tampilan Navbar. Navbar ini memiliki warna latar belakang gelap (dengan kode warna #001c30), dan juga memiliki bayangan (shadow) untuk memberikan efek visual.`

`-> <a class="navbar-brand" href="#">Aliyah Asmarani</a>: Ini adalah judul atau nama situs web Anda yang akan ditampilkan di Navbar. Dalam kasus ini, judulnya adalah "Aliyah Asmarani".`

`-> <button class="navbar-toggler" ...>: Ini adalah tombol yang muncul saat tampilan situs sangat kecil (misalnya, pada perangkat seluler). Ketika tombol ini diklik, itu akan membuka menu navigasi. Ini adalah cara untuk membuat situs web responsif.`

`-> <div class="navbar-collapse" ...>: Ini adalah bagian menu navigasi yang akan muncul ketika tombol "navbar-toggler" diklik. Ini berisi daftar tautan menu seperti "Home", "About", "Hobi", dan "Contact". Setiap tautan menu juga memiliki ikon yang sesuai.`

## Ketiga, Lanjut saya membuat bagian home 

### Berikut CODE nya:

```
<!-- Jumbotron -->
    <section class="jumbotron text-center">
      <img
        src="me1.jpeg"
        alt="Aliyah Asmarani"
        width="15%"
        class="rounded-circle img-thumbnail"
      />
      <h1 class="display-4">
        <i class="bi bi-lightning"></i> Aliyah Asmarani
        <i class="bi bi-lightning"></i>
      </h1>
      <p class="lead">Rani | 312210203</p>
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path
          fill="#ffffff"
          fill-opacity="1"
          d="M0,64L34.3,85.3C68.6,107,137,149,206,144C274.3,139,343,85,411,101.3C480,117,549,203,617,208C685.7,213,754,139,823,122.7C891.4,107,960,149,1029,138.7C1097.1,128,1166,64,1234,64C1302.9,64,1371,128,1406,160L1440,192L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"
        ></path>
      </svg>
    </section>
<!-- Akhir Jumbotron -->
```

### OUTPUT nya:

![image](https://github.com/Aliyahasmarani/Lab6Web/assets/115197672/0da282b2-9964-4ec2-bbd5-dc77ab15c237)

### PENJELASAN HOME

Disini, saya menggunakan tamplate boostrap yang versi 4

`-> <section class="jumbotron text-center">: Ini adalah elemen HTML yang digunakan untuk membuat bagian Jumbotron. Ini biasanya digunakan untuk menampilkan informasi penting di tengah halaman web. "text-center" mengatur teks di dalamnya menjadi rata tengah.`

`-> <img src="me1.jpeg" alt="Aliyah Asmarani" width="15%" class="rounded-circle img-thumbnail">: Ini adalah elemen gambar yang menampilkan gambar "me1.jpeg." Gambar ini biasanya adalah foto atau ilustrasi yang terkait dengan konten halaman. "rounded-circle" memberikan efek bulatan pada gambar dan "img-thumbnail" memberikan tampilan border.`

`-> <h1 class="display-4"> ... </h1>: Ini adalah judul besar di Jumbotron. Judul ini ditampilkan dalam font besar dan memiliki ikon "bi-lightning" di sekitarnya.`

`-> <p class="lead">Rani | 312210203</p>: Ini adalah paragraf yang berisi informasi tambahan. Di sini, Anda memiliki teks "Rani | 312210203" yang mungkin adalah informasi identitas atau keterangan tambahan.`

`-> <svg>...</svg>: Ini adalah elemen SVG (Scalable Vector Graphics) yang digunakan untuk membuat latar belakang dengan efek gelombang di bawah gambar dan teks. Ini memberikan tampilan estetis yang menarik pada Jumbotron.`

## Keempat, Berikutnya saya membuat bagian about

### Berikut CODE nya:

```
 <!-- About -->
    <section id="about" style="background-color: #ffffff">
      <div class="container">
        <div class="row text-center mb-3">
          <div class="col">
            <h2>About Me</h2>
            <br />
          </div>
        </div>
        <div class="text-center mb-5">
          <img src="me2.jpeg" class="rounded-circle img-thumbnail" width="25%" alt="me">
        </div>
        </div>
        <div class="row justify-content-center fs-5 text-center">
          <div class="col-md-4">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque
              eos quod maiores facilis est in tenetur veritatis ducimus earum
              debitis.
            </p>
          </div>
          <div class="col-md-4">
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt
              mollitia tenetur optio magni nam? Aspernatur voluptatem inventore
              sed aut harum sint amet at adipisci velit.
            </p>
          </div>
        </div>
      </div>
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path
          fill="#e0f4ff"
          fill-opacity="1"
          d="M0,64L34.3,101.3C68.6,139,137,213,206,245.3C274.3,277,343,267,411,229.3C480,192,549,128,617,96C685.7,64,754,64,823,106.7C891.4,149,960,235,1029,272C1097.1,309,1166,299,1234,245.3C1302.9,192,1371,96,1406,48L1440,0L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"
        ></path>
      </svg>
    </section>
<!-- Akhir About -->
```

### OUTPUT nya:















