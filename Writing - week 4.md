# **Asynchronous - Fetch, Async await**

> ## _fetch_
>
> ### _<div align="justify">Secara sederhana, `fetch` adalah sebuah object promise yang sudah disediakan oleh `Javascript`. Fetch bisa ditangkap atau dijalankan menggunakan `then catch` atau `async await`._
>
> <br>
>
> contoh :
>
> - ### _Siapkan API (promise yang sudah tersedia)_
>
>       https://digimon-api.vercel.app/api/digimon
>
> - ### _Ambil data API menggunakan fetch `.then`_
>
>   ```js
>   fetch("https://digimon-api.vercel.app/api/digimon")
>     //then pertama untuk menerima fetch
>     .then((result) => {
>       //return fetch yang sudah diunboxing dengan .json()
>       return result.json();
>     })
>     //then kedua menangkap fetch untuk ditampilkan
>     .then((result) => {
>       console.log(result);
>     });
>   ```
>
> <br>
>
> ## _Async await_
>
> ### _<div align="justify">`Async await` adalah metode untuk menjalankan atau menangkap sebuah object promise . Harus ada object promise untuk dapat Menjalankan function Async wait ._
>
> <br>
> contoh:
>
> - ### _Membuat promise `nonton()`._
>
>   ```js
>   let nonton = (kondisi) => {
>     return new Promise((resolve, reject) => {
>       if (kondisi == "jalan") {
>         resolve("nonton terpenuhi");
>       }
>       reject("batal nonton");
>     });
>   };
>   ```
>
> - ### _Lalu buat function Async await untuk menjalankan/menangkap object promise `nonton()`._
>
>   ```js
>   async function asyncNonton() {
>     let result = await nonton("jalan");
>     console.log(result); //nonton terpenuhi karena promise nonton() berisi argument "jalan"
>   }
>   ```
>
> - ### _Cara menangkap error didalam Async await menggunakan `try catch`._
>
>   ```js
>   async function asyncNonton() {
>     try {
>       let result = await nonton();
>       console.log(result);
>     } catch (error) {
>       console.log(error); //batal nonton karena promise nonton() tidak berisi argument
>     }
>   }
>   ```
>
> <br>

 <br>

# Git dan GitHub lanjutan

> ## _Set up `Organization`_
>
> - ### _Pilih paket `Organization`_
>
>   <img src="assets/O-pickPlan.png">
>
> - ### _Atur `Organization`_
>
>   <img src="assets/O-accountName.png">
>
> - ### _Tambah Member_
>
>   <img src="assets/O-addMembers.png">
>
> - ### _Tampilan awal `Organization`_
>
>   <img src="assets/O-welcomeToOrganization.png">

# **Responsive Web Design & Bootstrap 5**

> ## _Responsive Web Design_
>
> ### _Responsive web design adalah desain website yang dapat diakses dalam device apapun._
>
> <br>
>
> ## _Website yang responsif_
>
> ### _Menggunakan max-width_
>
> - ### _siapkan element `img`_
>
>   ```html
>   <!DOCTYPE html>
>   <html lang="en">
>     <head>
>       <meta charset="UTF-8" />
>       <meta http-equiv="X-UA-Compatible" content="IE=edge" />
>       <meta name="viewport" content="width=device-width, initial-scale=1.0" />
>       <title>Document</title>
>     </head>
>     <body>
>       <img src="assets/imgur_com.jpg" alt="" />
>     </body>
>   </html>
>   ```
>
> - ### _Sebelum diberi property `max-width`_
>
>   <img src="assets/beforeMax-width.png">
>
> - ### _Setelah diberi property `max-width`_
>
>   <img src="assets/afterMax-width.png">
>
>   ```css
>   img {
>     max-width: 100%;
>   }
>   ```
>
> <br>
>
> ## _Viewport_
>
> - ### _Viewport adalah area website yang dapat diakses user._
>
> - ### _Setting viewport pada website:_
>
> ```html
> <meta name="viewport" content="width=device-width, initial-scale=1.0" />
> ```
>
> <br>
>
> ## _Relative CSS Unit_
>
> ### _CSS relative unit ada beberapa macam:_
>
> - ### _em_
>
>   Size tergantung font-size element nya.
>
> - ### _rem_
>
>   Size tergantung font-size HTML (16px).
>
> - ### _vw_
>
>   Size tergantung 1% lebar viewport.
>
> - ### _vh_
>
>   Size tergantung 1% tinggi viewport.
>
> - ### _%_
>
>   Size tergantung parent element nya.
>
> <br>
>
> ## _Media Query_
>
> ### _Media query adalah metode untuk mengatur beberapa styling tergantung beberapa device tertentu._
>
> ### _Penggunaan `media query`_
>
> ```css
> @media only screen (max-width: 500px) {
>   background-color: aquamarine;
> }
>
> // warna latar akan berubah jika breakpoint dibawah atau menyentuh 500px.
> ```
>
> <br>
>
> ## _Bootsrap 5_
>
> ## _Mobile responsive website dan komponen website menggunakan Bootstrap_
>
> ### _Bootstrap merupakan framework CSS._
>
> ### _Cara mengimplementasikannya agar bisa dipakai pada website:_
>
> - ### _Salin `CDN via jsDelivr`_
>
>       <link>
>
> - ### _Tempel `CDN via jsDelivr` ke dalam head HTML_
>
>   ```html
>   <!DOCTYPE html>
>   <html lang="en">
>     <head>
>       <meta charset="UTF-8" />
>       <meta http-equiv="X-UA-Compatible" content="IE=edge" />
>       <meta name="viewport" content="width=device-width, initial-scale=1.0" />
>       <title>Document</title>
>       <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous" />
>       <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3" crossorigin="anonymous"></script>
>     </head>
>     <body></body>
>   </html>
>   ```
>
> ### _Lalu tinggal gunakan Bootstrap tersebut dengan menyisipkan code html dan class yang telah disediakan_
>
> <br>
>
> contoh:
>
> ### _Membuat form menggunakan bootstrap_
>
> ```html
> <div class="card" style="width: 18rem;">
>   <img src="..." class="card-img-top" alt="..." />
>   <div class="card-body">
>     <h5 class="card-title">Card title</h5>
>     <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
>     <a href="#" class="btn btn-primary">Go somewhere</a>
>   </div>
> </div>
> ```
>
> <br>
>
> <img src="assets/cardBootstrap.png">
