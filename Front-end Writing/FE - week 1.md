# **React JS, Intro to React**

> ## _Apa itu `React`?_
>
> ### _<div align="justify">`React` adalah `framework view library javascript` untuk membuat user interface pada website._
>
> <br>
>
> ## _Untuk apa kita menggunakan `React`?._
>
> ### _<div align="justify">`React` berguna untuk mempermudah developer dalam membuat suatu webste agar lebih efisien dan efektif_.
>
> ### _<div align="justify">Contohnya kita bisa lebih mudah mengakses elemen dengan menggunakan `Virtual DOM`, ketika kita mau membuat elemen yang sama pada suatu page maka kita tidak perlu copy paste karna bisa menggunakan `Component`._
>
> <br>
>
> ## _install React_
>
> ### _<div align="justify">Ada beberapa cara yang harus di siapkan untuk menginstal react, yaitu menginstall `Node JS` atau `Vite`. Sederhananya `Node JS` adalah mesin yang bisa menjalankan javascript agar dapat dijalankan diluar web browser. Sedangkan Vite adalah tools frontend untuk develop suatu website._
>
> <br>
>
> ## 1. Cara pertama
>
> - ### _Siapkan node js untuk menginstall react_
>
>       nodejs.org/en/
>
> - ### _Untuk dapat menginstall react, dibutuhkan minimal `Node JS versi 14`, yang compatible `minimal` pada windows 8. Jadi windows dibawah 8 tidak bisa menginstall Node JS versi 14, tapi bisa untuk versi dibawahnya._
>
> <br>
>
> - ### _Buka terminal untuk mendownload react._
>
>       npx ceate-react-app nama-project
>
> <br>
>
> - ### _Ukuran satu file React sebesar -+ 100mb. Jika ingin membuat file baru menggunakan react, maka harus install react lagi menggunakan npx pada terminal._
>
> <br>
>
> - ### _Ketika React sudah terinstall, maka jalankan perintah npm._
>
>       npm start
>
> <br>
>
> ## 2. Cara kedua
>
> - ### _Siapkan Vite untuk menginstall react_
>
>       vitejs.dev/guide/
>
> <br>
>
> - ### _Buka bash untuk mendownload react._
>
>       npm ceate vite@latest nama-project --template react
>
> <br>
>
> - ### _Ketika folder sudah dibuat, maka jalankan perintah npm ._
>
>       npm install
>
> <br>
>
> - ### _Ketika npm sudah di install, maka jalankan perintah npm._
>
>       npm run dev
>
> <br>
>
> - ### _Lalu akan dikirim link dari host local kita yang sudah jadi._
>
> <br>
>
> ## _Single Page Application_
>
> ### _<div align="justify">Single Page Application adalah teknologi yang bisa kita pakai ketika menggunakan React yang memungkinkan kita tidak lagi susah payah membuat halaman atau elemen satu persatu, tetapi bisa membuat template 1 kali agar bisa dipanggil berkali-kali._
>
> <br>
>
> ## _JSX_
>
> ### _<div align="justify">Javascript XML adalah syntax extension dari React yang memungkinkan syntax HTML bisa ditulis didalam javascript._
>
> ```jsx
> class Message extends React.Component {
>   render() {
>     return <div> Hello {this.props.name}</div>;
>   }
> }
> ```
>
> <br>
>
> ### _<div align="justify"> Dalam Javascript XML hanya bisa melakukan return 1 element._
>
> <br>
>
> ## _Virtual DOM_
>
> ### _<div align="justify"> `Virtual DOM (VDOM)` adalah representasi JavaScript ringan dari Model Objek Dokumen (DOM) yang digunakan dalam kerangka kerja web deklaratif seperti React. Memperbarui DOM virtual relatif lebih cepat daripada memperbarui DOM yang sebenarnya (melalui JavaScript)._
>
> ![Virtual DOM](https://www.petanikode.com/img/react/komponen/virtualdom.png)
>
> <br>

# **Component**

> ### _<div align="justify">Component adalah suatu/kumpulan element HTML yang dibuat sekali saja sebagai template dan nantinya dipanggil ketika dibutuhkan. Component membagi UI dalam satuan-satuan kecil, yang artinya dalam satu page bisa memanggil component lebih dari satu._
>
> <br>
>
> contoh :
>
> - Buat Component Home.
>
>   ```js
>   function Home() {
>     return (
>       <div>
>         <h1>ini home</h1>
>       </div>
>     );
>   }
>
>   export default Home;
>   ```
>
> <br>
>
> - lalu panggil pada `App.js`.
>
>   ```js
>   import Home from "./components/Home";
>
>   function App() {
>     return (
>       <div>
>         <Home />
>       </div>
>     );
>   }
>
>   export default App;
>   ```
>
> <br>
>
> ## _Styling pada React_
>
> ### _<div align="justify"> Untuk memberi styling pada file tertentu, kita bisa panggil menggunakan import._
>
> <br>
>
> contoh:
>
> ### Misalkan ingin memberi styling pada App.js, maka panggil `App.css` yang sebelumnya sudah dibuat, ke dalam file `App.js`.
>
>       import "./App.css";
>
> <br>
>
> ## _State & Props_
>
> ### <div align="justify">`State` adalah sebuah object untuk menyimpan data di dalam React dan nanti di render ketikamelakukan perubaan data di dalam react.
>
> ### `Props` (properties) adalah komunikasi dari component parent dan child berbentuk pengiriman data dan ditampung ke state.
>
> <br>
>
> contoh:
>
> ```js
> import Home from "./components/Home";
>
> function App() {
>   return (
>     <div>
>       <Home name={"Abil"} age={20} />
>     </div>
>   );
> }
>
> export default App;
> ```
>
> Buat Component Home.
>
> ```js
> function Home(props) {
>   return (
>     <div>
>       <h1>
>         My name is {props.name}. My age is {props.age} years old
>       </h1>
>     </div>
>   );
> }
>
> export default Home;
> ```
>
> // hasilnya ( My name is `Abil.` My age is `20` years old.)
>
> <br>

# Lifecycle Hooks

> ### _<div align="justify"> Lifecycle (Siklus Hidup), Lifecycle pada React Native adalah aktifitas method yang dilakukan oleh React Native ketika aplikasi di > jalankan. Jenis-Jenis Lifecycle React Native._
>
> - ### _<div align="justify"> Initialization adalah sebuah siklus React Native untuk menset State dan Props sebelum aplikasi di jalankan._
> - ### _<div align="justify"> Mounting adalah sebuah siklus ketika aplikasi baru saja di buka ada 2 jenis yaitu componentDidMount() ketika memuat aplikasi sebelum render dilakukan. componentWillMount yaitu siklus setelah render proses dilakukan. Tapi sekarang disarankan kamu menggunakan componentDidmount()._
> - ### \_<div align="justify"> Updatating yaitu ketika kamu mengubah data yang telah di Mounting.
> - ### _<div align="justify"> Unmount adalah proses menghancurkan atau mendestroy komponen yang sebelumnya di definisikan._
>
> <br>
>
> ## _1. useState_
>
> ### _<div align="justify">`useState` adalah cara menyimpan variable. Kenapa kitta harus mengunakan usestate? karena di dalam React ada yg namanya `Immutable` atau tidak bisa mengubah data secara langsung._
>
> <br>
>
> ```js
> import { useState } from "react";
>
> function Home(props) {
>   const [name, setname] = useState("Abil");
> }
>
> export default Home;
> ```
>
> <br>
>
> ### _<div align="justify"> Didalam `useState` terdapat array yang isinya terdapat `[ variableName, setName ]`._
>
> ### _<div align="justify"> `variableName` berfungsi untuk menampilkan value saja, sedangkan `setName` untuk mengubah value nya._
>
> <br>
>
> ## _2. UseEffect_
>
> ### _<div align="justify"> `UseEffect` pada React Hooks seperti ComponentDoMount dan ComponentWillUnmount, jadi dengan menggunakan UseEffect penulisan kode nya jadi lebih simple dan clean. `UseEffect` merupakan Hooks yang bisa digunakan untuk menggunakan lifecyle functional component dengan mudah._
>
> <br>
>
> ## _3. useCallback dan useMemo_
>
> ### _<div align="justify"> `useCallback` akan mengembalikan versi panggilan balik dari memoise yang hanya berubah jika salah satu dari dependensi telah berubah._
>
> ### _<div align="justify"> Ini berguna ketika meneruskan panggilan balik ke komponen turunan optimal yang mengandalkan kesetaraan referensi untuk mencegah perenderan yang tidak perlu (mis. `ShouldComponentUpdate`)._
>
> ### _<div align="justify"> `useMemo`, Mengirim function "create" dan berbagai dependensi._
>
> ### _<div align="justify"> `useMemo` hanya akan menghitung ulang nilai memoized ketika salah satu dependensi telah berubah. Optimalisasi ini membantu menghindari perhitungan mahal pada setiap render._
>
> <br>
>
> ## _4. useRef_
>
> ### _<div align="justify"> Refs menyediakan cara untuk mengakses `Node DOM` atau Bereaksi elemen yang dibuat dalam metode render._

<br>
