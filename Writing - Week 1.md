# **Unix Command Line**

> ## _Shell_
>
> ### <div align="wjustify">Secara sederhana, `shell` adalah jenis program komputer yang disebut interpreter baris perintah yang memungkinkan pengguna mengontrol dan berkomunikasi secara efisien dengan sistem operasi mereka dengan `command-line interface`.
>
> <br>
>
> ## _Command Line Interface_
>
> ### <div align="justify"> CLI adalah `UI (User Interface)` berbasis teks yang digunakan untuk menjalankan program, mengelola file komputer, dan berinteraksi dengan komputer.
>
> <br>
>
> ## _Cara mengakses CLI dan menggunakan terminal_
>
> ### <div align="justify">Sebenarnya mengakses CLI ini bisa menggunakan beberapa cara, bisa menggunakan `shell` bawaan seperti Command Prompt, terminal atau Bash.
>
> <br>
>
> ## _File system structure_
>
> ### <div align="justify">File System menyediakan akses yang efisien ke `disk` dengan memungkinkan data disimpan, ditempatkan, dan diambil dengan cara yang nyaman
>
> <br>
>
> ## _Command untuk melihat current working directory_
>
> ```
> pwd
> ```
>
> <br>
>
> ## _Command untuk melihat isi sebuah directory_
>
> ```
> dir
> ```
>
> <br>
>
> ## _Command untuk berpindah directory_
>
> ```
> cd directory_name
> ```
>
> <br>
>
> ## _Command untuk melihat isi files_
>
> ```
> type <file_name>
> ```
>
> <br>
>
> ## _Command untuk membuat file & direktori_
>
> - ### _untuk membuat file_
>
>   ```
>   touch <file_name>
>   ```
>
> - ### _untuk membuat direktori_
>
>   ```
>   mkdir <directory_name>
>   ```
>
> <br>
>
> ## _Command untuk menyalin file & direktori_
>
> - ### _untuk menyalin file_
>
>   ```
>   cp <file_name>
>   ```
>
> - ### _untuk menyalin direktori_
>
>   ```
>   cp <directory_name>
>   ```
>
> <br>
>
> ## _Command untuk memindahkan atau me-rename file dan direktori_
>
> - ### _untuk memindahkan atau me-rename file_
>
>   ```
>   mv <file_name>
>   ```
>
> - ### _untuk memindahkan atau me-rename direktori_
>
>   ```
>   mv <directory_name>
>   ```
>
> <br>
>
> ## _Command untuk menghapus file & direktori_
>
> - ### _untuk menghapus file_
>
>   ```
>   rm <file_name>
>   ```
>
> - ### _untuk menghapus direktori_
>
>   ```
>   rm <directory_name>
>   ```
>
>   <br>

<br>

# **Git & GitHub dasar**

> ## _Perbedaan antara Git dan Github_
>
> ### <div align="justify">Sederhananya, `Git` adalah sistem kontrol versi yang memungkinkan Anda mengelola dan melacak riwayat kode sumber Anda. `GitHub` adalah layanan hosting berbasis cloud yang memungkinkan Anda mengelola repositori Git.
>
> <br>
>
> ## _Kenapa Git dan Github tools yang wajib digunakan_
>
> - ### _Mengapa kita harus menggunakan Git dan Github?_
>
>   - #### <div align="justify">Karena, `Git` memungkinkan individu dan sekelompok tim untuk bekerja sama, semuanya menggunakan file yang sama. Dan ini membantu tim mengatasi kebingungan yang cenderung terjadi ketika banyak orang mengedit file yang sama.
>
>   - #### <div align="justify">`GitHub` adalah perangkat lunak yang sangat sering digunakan yang biasanya digunakan untuk kontrol versi. Akan sangat membantu ketika lebih dari satu orang mengerjakan sebuah proyek. Katakanlah misalnya, tim `Software developer` ingin membangun situs web dan setiap orang harus memperbarui kode mereka secara bersamaan saat mengerjakan proyek.
>
> <br>
>
> ## _Alur kerja dari Git dan Github_
>
> - ### _Alur kerja Git_
>
>   - #### <div align="justify">Alur kerja Git adalah inisialisasi projek untuk membuat repository di file lokal, melacak perubahan projek dengan menambahkan file baru di repository yang dipilih, menambah komen untuk menyimpan perubahan projek yang di lacak.
>
> - ### _Alur kerja GitHub_
>
>   - #### <div align="justify">Alur kerja GitHub adalah membuat `repository` di github untuk menampung perubahan git, menghubungkan projek yang dilacak dengan repository menggunakan `remote`, kembali ke alur kerja Git, mengirimkan perubahan file yang dilakukan setelah perubahan disimpan ke repository GitHub..
>
> <br>
>
> ## _Repository Git_
>
> Repositori Git melacak dan menyimpan riwayat semua perubahan yang dibuat pada file dalam projek Git. Ini menyimpan data ini dalam direktori bernama `.git`.
>
> <br>
>
> ## _Melakukan commit pada Git_
>
> Untuk melakukan commit pada Git harus melewati beberapa langkah, yaitu :
>
> - _Menginsialisasi Git_
>
>       git init
>
> - _Menambahkan projek baru di `repository` yang dipilih_
>
>       git add .
>
> - _Menyimpan perubahan yang sudah dilakukan_
>
>       git commit -m "pesan"
>
>   <br>
>
> ## _Mempublish aplikasi ke Github_
>
> Ada beberapa langkah yang juga harus ditempuh untuk mempublish aplikasi atau projek kita ke GitHub, diantaranya :
>
> - _Membuat `Repository` di GitHub Untuk menampung projek_
>
>   ![Cara buat repository baru](./assets/Repo-baru.png)
>
> - _Mengelola server Pusat untuk hosting repositori git menggunakan `remote`_
>
>   ![Remote repository baru](./assets/Remote-repo.png)
>
>       git remote add origin https://github.com/BILIIIIIII/repo_baru.git
>
> - _Menambahkan projek baru di `repository` yang dipilih_
>
>       git add .
>
> - _Menyimpan perubahan yang sudah dilakukan_
>
>       git commit -m "pesan"
>
> - _Mengirimkan perubahan projek ke repository GitHub_
>
>       git push -u origin master
>
> <br>
>
> ## _Melakukan cloning Github ke local_
>
> - kita bisa menggunakan Https atau SSH.
>
> <br>

<br>

# **HTML**

> ## _Peran HTML pada web development_
>
> HTML berperan sebagai struktur pada halaman web.
>
> <br>
>
> ## _Tools pendukung dalam menggunakan HTML_
>
> - Code Editor. Contoh, `Visual Studio Code`, `Sublime`, `Notepad++`, etc.
> - Browser. Contoh, `Google Chrome`, `Mozilla Firefox`, `Operamini`, etc.
>
> <br>
>
> ## _Membuat HTML sederhana_
>
>       <!DOCTYPE html>
>       <html>
>       <head>
>       <title>
>           Writing & Presentation
>       </title>
>       </head>
>       <body>
>           <h1> tes Membuat HTML sederhana </h1>
>       </body>
>       </html>
>
> <br>
>
> ## _Menjalankan HTML secara manual dan menggunakan live server dari VS Code_
>
> ![Live server web HTML](./assets/liveServer-VSC.png)
>
> <br>
>
> ## _Mengimplementasikan tag HTML yang populer_
>
> - _Tag untuk menambahkan/menampilkan gambar_
>
>       <img src="..." alt=""></img>
>
> - _Tag untuk membuat sebuah paragraph_
>
>       <p> Belajar tentang tag di HTML </p>
>
> - _Tag untuk membuat list_
>
>   - Unordered List
>
>           <ul>
>               hewan
>               <li>kucing</li>
>               <li>anjing</li>
>               <li>tikus</li>
>           </ul>
>
>   - Ordered List
>
>           <ol>
>              tumbuhan
>               <li>bunga</li>
>               <li>rumput</li>
>               <li>raflesia arnoldi</li>
>           </ol>
>
> - _Tag HTML Untuk Membuat tulisan dengan link_
>
>        <a href="...">tulisan ini berupa link</a>
>
> <br>
>
> ## _Mengimplementasikan semantic HTML_
>
> <div align="justify">HTML yang memperkenalkan makna ke halaman web bukan hanya presentasi.
>
> <div align="justify">Misalnya, tag menunjukkan bahwa teks terlampir adalah paragraf. Ini bersifat semantik dan presentasional karena orang tahu apa itu paragraf, dan browser tahu cara menampilkannya.
>
> - _Contoh HTML tidak semantic_
>
>       <div class="paragraph">
>           <div>
>               <div>
>               tag ini tidak semantic
>               </div>
>           </div>
>       </div>
>
> - _Contoh HTML semantic_
>
>          <p> tag ini semantic </p>
>
> <br>
>
> ## _Mempublish website sampai ke tahap deployment_
>
> `Deployment` adalah tahap di mana Anda memindahkan situs web dari lingkungan lokal ke server langsung. Ini disebut live website.
>
> Jika aplikasi kita HTML atau Web App kita perlu mendeploy ke server, maka kita bisa menggunakan layanan hosting static site yang bernama `Netlify`, `GitHub`, `000webhost`, `Vercel`, `Heroku` dan lain-lain.
>
> <br>

<br>

# **CSS**

> ## _Peran CSS pada web development_
>
> `CSS` digunakan untuk menata halaman web. CSS dapat digunakan untuk menyesuaikan ukuran konten, spasi, warna dan font atau menambahkan fitur dekoratif, seperti animasi atau membagi konten menjadi kolom.
>
> ## _Beberapa cara menyisipkan CSS ke dalam HTML_
>
> Ada 3 cara menyisipkan CSS ke HTML, diantaranya :
>
> 1.  _Inline CSS (CSS di baris element suatu tag, di dalam tag body)_
>
>           <div class="css" style="color:black;">
>               <h1>bola</h1>
>           </div>
>
> <br>
>
> 2.  _Internal CSS (CSS didalam tag head, masih di file HTML)_
>
>           <!DOCTYPE html>
>            <html lang="en">
>
>          <head>
>            <meta charset="UTF-8" />
>            <meta http-equiv="X-UA-Compatible" content="IE=edge" />
>            <meta name="viewport" >content="width=device-width, initial-scale=1.0" />
>            <title>Document</title>
>
>            <style>
>              css {
>                color: black;
>              }
>            </style>
>          </head>
>
>          <body>
>            <div class="css">
>              <h1>bola</h1>
>            </div>
>          </body>
>
>        </html>
>
> <br>
>
> 3.  _External CSS (CSS diluar file HTML)_
>
>           css {
>                color: black;
>              }
>
> <br>
>
> ## _Menggunakan sintaks dasar dari CSS_
>
> - _Selector_
>
>   Pola elemen dan istilah lain yang memberi tahu browser bahwa elemen HTML mana yang harus dipilih agar nilai properti CSS di dalam aturan diterapkan padanya.
>
>           html {
>
>           }
>
>           //html tersebut adalah selector
>
> - _Property_
>
>   karakteristik yang nilai terkaitnya menentukan satu aspek tentang bagaimana browser seharusnya menampilkan elemen.
>
>           html {
>           color: ;
>           }
>
>           //color tersebut adalah property
>
> - _Value_
>
>   Nilai dari suatu property.
>
>           html {
>           color: whitesmoke;
>           }
>
>           //whitesmoke tersebut adalah value
>
>   Pola elemen dan istilah lain yang memberi tahu browser bahwa elemen HTML mana yang harus dipilih agar nilai properti CSS di dalam aturan diterapkan padanya.
>
> <br>
>
> ## _Menerapkan styling CSS pada sebuah halaman HTML_
>
> ![Live server web HTML](./assets/Styling-CSS.png)
>
> <br>
>
> ## _Menggunakan flexbox_
>
> Ada dua komponen utama sebuah layout Flexbox yaitu container dan item.
>
>           // File HTML
>
>           <nav class="container">
>             <div> Home </div>
>             <div> Search </div>
>             <div> Logout </div>
>           </nav>
>
> Untuk mengubah layout ini untuk menggunakan Flexbox, cukup berikan kelas container properti CSS berikut:
>
>           .container {
>               display: flex;
>           }
>
> Penambahkan properti tadi akan membuat layout sebelumnya menjadi sejajar secara horizontal.

<br>

# **Algoritma**

> ## _Perbedaan antara Algoritma dan Data Structures_
>
>   <div align="justify">`Struktur data` adalah lokasi bernama yang dapat digunakan untuk menyimpan dan mengatur data. Dan, `algoritma` adalah kumpulan langkah-langkah untuk memecahkan masalah tertentu. Mempelajari struktur dan algoritme data memungkinkan kita menulis program komputer yang efisien dan optimal.
>
> <br>
>
> ## _Manfaat dari algoritma dan data structure_
>
>   <div align="justify">`Struktur Data` dan `Algoritma` membahas solusi untuk masalah standar secara mendetail dan memberi Anda wawasan tentang seberapa efisien penggunaan masing-masing masalah tersebut, kedua hal tersbut juga mengajarkan Anda ilmu mengevaluasi efisiensi suatu algoritma. Hal ini memungkinkan Anda untuk memilih yang terbaik dari berbagai pilihan.
>
> <br>
>
> ## _Membuat algoritma sederhana_
>
> - ### Algoritma Membuat kopi
>      <div align="justify">Contoh algoritma dalam kehidupan sehari-hari pertama adalah terkait dengan cara membuat kopi. Yaitu berisi panduan mulai dari membuka kemasan kopi, tuangkan bubuk kopi ke cangkir, tuangkan gula ke cangkir, panaskan air hingga mendidih, tuangkan air panas ke cangkir, aduk kopi dan gula hingga merata, Setelah semua tercampur rata, kopi siap dihidangkan.
>
> <br>
>
> ## _Menerapkan algoritma ke dalam bahasa pemrograman_
>
> ![Live server web HTML](./assets/flowchart.png)
>
> <br>
>
> ## _Memahami Big-O Notation_
>
> ### `Big-O Notation` adalah cara untuk mengkonversi keseluruhan langkah-langkah suatu algoritma kedalam bentuk Aljabar.
>
> <br>
>
> ## _Mempraktikkan pendekatan menyelesaikan suatu masalah untuk diselesaikan melalui program_
>
> <br>
>
> ## _Menerapkan salah satu algoritma dengan JavaScript_
>
> ### `Sequence` atau berurutan.
>
> <br>
>
> ## _Menerapkan salah satu struktur data dengan JavaScript_
>
> ### Object.
>
> <br>

<br>

# **Javascript Dasar**

> ## _Peran JavaScript pada web development_
>
> ### JavaScript bahasa pemrograan yang digunakan oleh sisi client dan sisi server yang dapat membuat suatu web menjadi interakktif.
>
> ## _Menjalankan JavaScript_
>
> ## _Membedakan berbagai tipe data_
>
> - Null
> - Undefined
> - string
> - number
> - boolean
> - object
> - array
> - function
>
> ## _Menggunakan operator_
>
> 1. Operator aritmatika;
>
> - Penjumlahan +
> - Pengurangan –
> - Perkalian \*
> - Pemangkat \*\*
> - Pembagian /
> - Sisa bagi %
>
> 2. Operator Penugasan (Assignment);
>
> - Pengisian nilai =
> - Pengisian penambahan +=
> - Pengisian pengurangan -=
> - Pengisian perkalian \*=
> - Pengisian pemangkatan \*\*=
> - Pengisian pembagian /=
> - Pembagian sisa bagi %=
>
> 3. Opeartor relasi atau perbandingan;
>
> - Lebih besar >
> - Lebih kecil <
> - Sama dengan ==
> - Sama dengan tipe data ===
> - Tidk sama dengan != atau !==
> - Lebih besar sama dengan >=
> - Lebih kecil sama dengan <=
> -
>
> 4. Operator Logika;
>
> - Logika AND &&
> - Logika OR ||
> - Negasi !
>
> 5. Operator Bitwise;
>
> - AND &
> - OR |
> - XOR ^
> - Negasi !
>
> 6. Operator Ternary;
>
> - Opertor ternary pada Javascript, biasanya digunakan untuk membuat sebuah percabangan if/else.
> - Simbol opertor ternary terdiri dari tanda tanya dan titik dua (?:).
> - Bentuknya seperti ini:
> - <kodisi> ? "benar" : "salah"
> -
>
> ## Membedakan control flow (conditional dan looping)
>
> Conditional
>
> Sebuah metode dasar untuk menjalankan program pada kondisi yang berbeda.
>
> - If
> - Else if
> - Switch case
>
> LOOPING
>
> Berbeda dengan Conditional statement, looping adalah sebuah pengulangan dalam programming sampai nilai tersebut false. Para programmer bisa membuat sebuah sistem program bekerja lebih dari 1 kali di dalam looping. Looping menggunakan 2 operator yaitu Operator decrement (pengurangan) dan increment (penambahan).
>
> - For, fix
> - While do
>
>        Kita dapat lihat bahwa while diperiksa belakangan dibandingan dengan while…do.
>
>   Logikanya seperti ini, jika dengan While Do program akan memeriksa kondisi terlebih dahulu, namun jika dengan Do While, program akan memeriksanya setelah melakukan perintah sesuai yang dituliskan pada bagian do.
