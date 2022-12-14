# _Javascript Scope_
   
   Scope dalam JavaScript mendefinisikan aksesibilitas variabel, objek, dan fungsi.Ada dua jenis cakupan di JavaScript yaitu :

 - **Global Scope**
     
     Semua variabel yang dibuat di luar fungsi disebut variabel global JavaScript. Objek semacam itu dapat diakses di seluruh situs web. Global Scope harus mempunyai nama yang unik agar tidak terjadi error.

     Contoh Global Scope :

     ```javascript
     let sepatu = "Warrior Sparta";

     // Variabel sepatu bisa dimanfaatkan disini.
     
     function myShoes(){
     // Variabel sepatu bisa dimanfaatkan di dalam fungsi ini.
     };

     // Variabel sepatu bisa dimanfaatkan disini.
     ```
     

   - **Local Scope**
    
     Variable local scope atau variable fungsi lokal adalah variabel yang dideklarasikan di dalam fungsi pada JavaScript. Dan hanya bisa di akses di dalam fungsi tersebut.

     Contoh Global Scope :

     ```javascript
     // Variabel sepatu tidak bisa dimanfaatkan disini.
     
     function myShoes(){
        let sepatu = "Warrior Sparta";
     };

     // Variabel sepatu tidak bisa dimanfaatkan disini.
     ```

 # _Javascript Function_
   
   Fungsi JavaScript adalah blok kode yang dirancang untuk melakukan tugas tertentu Fungsi JavaScript dijalankan ketika "sesuatu" memanggilnya.

   Javscript Funtion Syntax :

   ```javascript
   function name(parameter1, parameter2){
    // Kode yang akan dieksekusi
   }
   ```

   Ketika JavaScript mencapai "return", fungsi akan berhenti dijalankan.

   ```javascript
   function name(parameter1, parameter2){
    return parameter1 * parameter2;
   }

   let result = name(4,10); // Memanggil fungsi name dengan mengisikan argumennya.

   console.log(result);

   40 // return value
   ```

 # _Data Type Built in Prototype & Method_

   Dalam pemrograman, tipe data merupakan konsep penting. Untuk dapat beroperasi pada variabel, penting untuk mengetahui sesuatu tentang tipenya. Tanpa tipe data, komputer tidak dapat menyelesaikan masalah ini dengan baik. Berikut macam-maca data type pada Javascript :

   - **Javascript Strings**

     String adalah serangkaian karakter seperti "John Doe". String ditulis dengan tanda kutip. Anda dapat menggunakan tanda kutip tunggal ('') atau ganda ("").

     ```javascript
     let name = "Abil Khairi";
     let name = 'Abil Khairi';
     ```
   - **Javascript Numbers**

     JavaScript hanya memiliki satu jenis angka. Angka dapat ditulis dengan desimal atau tanpa desimal.

     ```javascript
     let result = 52000;
     let result = 52.000;
     ```
   - **Javascript Booleans**

     Pada javascript, data type booleans hanya memiliki dua nilai yaitu, true atau false.

     ```javascript
     let x = 10;
     let y = 20;
     let z = 20;

     (X == y) // return false
     (Y == z) // return true
     ```

   - **Javascript Arrays**

     Array JavaScript ditulis dengan tanda kurung siku. Item array dipisahkan dengan koma. Index pada array dimulai dari [0].Array dapat menampung tipe data apapun.

     ```javascript
     const handphone = ["Asus","Samsung","Sony"];

     console.log(handphone[1]); // memanggil salah satu item.
     ```

   - **Javascript Objects**

     Objek JavaScript ditulis dengan kurung kurawal {}. Objects dapat menampung tipe data apapun.

     ```javascript
     const handphone = {
      brand: "Asus",
      type: "Asus ROS phone 6",
      build: "2022"
     };

     console.log(handphone.brand); // memanggil salah satu properti.
     ```

   - **Contoh Javascript Data Type**

     ```javascript
     const Mahasiswa = {
      name: "Abil Khairi",
      age: 21,
      hometown: "Aceh",
      detail: [
        {
          eyes: "coklat"
        },
        {
          hair: "Hitam"
        }
      ]
     };

     console.log(person.detail[0]); // memanggil salah satu properti yang di dalamnya ada sebuah array.
     ```
 # _DOM (Document Object Model)_

   DOM merupakan kependekan dari Document Object Model, DOM ini yakni object model standar bagi XML dan HTML yang memiliki sifat platform independent. Objek dari dokumen tersebut menyediakan sekumpulan fungsi serta data atau atribut yang dapat dimanfaatkan ketika membuat program Javascript. 

   - **Manfaat penggunaan DOM**

     > Dapat merubah HTML element, HTML attributes pada halaman.

     > Dapat merubah style di halaman.

     > Dapat menambah atau menghapus HTML element, HTML attributes.

     > Dapat memberikan reaksi user terhadap peristiwa yang terjadi di halaman.

   - **DOM menemukan HTML element**
     
     | Method                             | Description                                |
     |------------------------------------|--------------------------------------------|
     | document.querySelector()           | Menemukan element berdasarkan selector CSS |
     | document.getElementsById()         | Menemukan element berdasarkan Id           |
     | document.getElementsByClassName()  | Menemukan element berdasarkan nama kelas   |
     | document.getElementsByTagName      | Menemukan element berdasarkan tag          |

   - **DOM CSS**

     Untuk mengubah gaya elemen HTML, gunakan sintaks ini:

     ```javascript
     document.getElementById(id).style.property = new style
     ```

   - **DOM Event Listener**
    
     ```javascript
     element.addEventListener(event, function, useCapture);
     ```

   - **Contoh DOM Sederhana**

     Berikut contoh sederhana dari penggunaan DOM yang mencakup finding element, 
     dan memakai event listener.

     ```html
     <h1 class="heading">HOLAAAAAA</h1>
     <button class="btn">Click Me</button>
     ```

     ```javascript
     const heading = document.querySelector(".heading");
     const btn = document.querySelector(".btn");

     btn.addEventListener("click", function(){
        heading.style.backgroundColor = "red";
     });
     ```
   
  
