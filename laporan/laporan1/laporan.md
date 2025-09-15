# Laporan Modul 1: Perkenalan Laravel
**Mata Kuliah:** Workshop Web Lanjut
**Nama:** Firdhila Ananda Syahputri
**NIM:** 2024573010014
**Kelas:** TI-2C

---

## Abstrak

Laporan ini berfungsi untuk memahami dasar-dasar framework laravel. Laporan ini disusun agar dapat memahami konsep dasar laravel, tujuan penggunaan laravel, kemudian juga mengenal komponen utama laravel, dan mengetahui struktur folder dan file laravel agar bisa memahami fungsi setiap direktori dan file dalam sebuah project.

---

## 1. Pendahuluan

   Laravel merupakan salah satu framework PHP yang populer digunakaan saat ini dan bersifat open-source. Framework web adalah  Laravel dikembangkan oleh Taylor Otwell pada tahun 2011. Laravel dirancang untuk membuat pengembangan web menjadi lebih cepat dan mudah. Framework ini menggunakan pola arsitektur MVC (Model-View-Controller).

   MVC (Model-View_Controller) merupakan desain arsitektur yang membantu menjaga kode tetap terorganisir dan memudahkan pengembangan, pemeliharaan, dan skalabilotas aplikasi. MVC memisahkan aplikasi menjadi tiga komponen utama Model, View, dan Controller. Laravel cocok untuk jenis aplikasi berbasis web yang butuh struktur jelas, keamanan, dan fitur lengkap. Contoh aplikasi yang cocok dibuat dengan laravel yaitu seperti E-commerce, aplikasi edukasi, dan aplikasi lainnya yang membutuhkan struktur yang rapi, yang banyak fitur CRUD.

---

## 2. Komponen Utama Laravel 
- Blade (templating)
  Blade Tamplating Engine adalah fitur laravel untuk membuat tampilan web. Dengan Blade, kita bisa mencampur kode HTML dan logika laravel seperti perulangan atau kondisi dengan cara yang sederhana. 

- Eloquent (ORM)
  Eloquent adalah fitur ORM (Object Relational Mapping) bawaan laravel yang sederhana namun fleksibel. Elequent memungkinkan pengembang untuk berinteraksi dengan basis data menggunakan sintaksis yang lebih mudah, rapi, dan intuitif.

- Routing
  Routing berfungsi untuk mengatur jalur atau alamat URL dalam aplikasi. Dengan fitur ini, bisa menentukan halaman atu fungsi mana yang akan dijalankan ketika pengguna membuka sebuah URL. Cara penulisannya sederhana dan mudah dimengerti.

- Controllers
  Controller di laravel adalah kelas yang berisi logika utama aplikasi. Controller bertugas menjadi penghubung antara data dari model dan tampilan di view. Dengan adanya controller, kode aplikasi lebih terstruktur, rapi, dan mudah dikelola.

- Migrations & Seeders
  Migrations di laravel berfungsi untuk membuat atau mengubah struktur tabel di database tanpa perlu menulis query SQL secara manual. Seeder digunakan untuk mengisi tabel dengan data awal atau data contoh supaya aplikasi bisa langsung diuji.

- Artisan CLI
  Artisan adalah alat berbasis command line di laravel yang berisi banyak perintah siap pakai untuk mempermudah pengembangan. Dengan artisan, kita bisa membuat kontroler, model, dan komponen lainnya hanya dengan beberapa perintah.

- Testing (PHPUnit)
  Testing dengan PHPUnit adalah fitur laravel untuk menguji aplikasi secara otomatis. Melalui testing, kita bisa memastikan setiap fungsi berjalan sesuai harapan tanpa harus mencoba manual satu per satu.

---

## 3. Berikan penjelasan untuk setiap folder dan files yang ada didalam struktur sebuah project laravel.

   - Folder
      1. App
         Folder ini berisi kode inti aplikasi yang kita buat. 
      2. Bootstrap
         Folder Bootstrap berisi app.php yang berfungsi untuk melakukan bootstrap pada kerangka kerja. Ini merupakan tahap awal agar framework laravel siap dipakai.
      3. Config
         Direktori config berisi semua berkas konfigurasi aplikasi.
      4. Database
         Folder database berisi migrasi basis data, pabrik model, dan seed.
      5. Public
         Folder public berisi index.php berkas yang merupakan titik masuk untuk semua permintaan yang masuk ke aplikasi dan mengonfigurasi pemuatan otomatis.
      6. Resource
         Folder resource berisi tampilan serta aset mentah yang belum dikompilasi seperti CSS atau JavaScript.
      7. Routes
         Folder routes berisi semua definisi rute untuk aplikasi. Secara default, laravel menyertakan dua berkas rute web.php dan console.php. web.php berisi rute-rute yang ditempatkan laravel di web grup middleware. console.php adalah tempat anda dapat mendefinisikan semua perintah konsol berbasis closure.
      8. Storage
         Folder storage berisi log, tamplate blade yang dikompilasi, sesi berbasis berkas, cache berkas.
      9. Vendor
         Folder vendor berisi dependensi Composer.
      
   - File
      1. .editorconvig
         File ini digunakan untuk memberi IDE/text editor instruksi tentang standar coding laravel.
      2. .env dan env.example
         File ini tempat dimana variabel environment aplikasi ditempatkan seperti nama database, username database.
      3. .gitattributes dan .gitignore
          File konfigurasi git.
      4. artisan
         File ini berfungsi untuk menjalankan perintah artisan dari command line.
      5. composer.json dan composer.lock
         File konfigurasi untuk composer.
      6. package.json
         File package.json digunakan untuk aset-aset dan dependencies front end.
      7. phpunit.xml
          File phpunit.xml merupakan dile konfigurasi untuk PHPUnit, tools yang digunakan laravel untuk testing.
      8. README.md
          File ini merupakan markdown yang memberikan pengenalan dasar tentang laravel.
---

## 4. Diagram MVC dan Cara kerjanya

  <img src="D:\KULIAH\SEMESTER 3\WORKSHOP WEB LANJUT\web-lanjut-2024573010014\laporan\laporan1\gambar\gambarmvc.jpg" alt="gambar alur MVC">

  - Proses pertama adalah view akan meminta data untuk ditampilkan dalam bentuk grafis kepada pengguna.
  - Permintaan tersebut diterima oleh controller dan diteruskan ke model untuk diproses.
  - Model akan mencari dan mengolah data yang diminta di dalam database.
  - Setelah data ditemukan dan diolah, model akan mengirimkan data tersebut kepada controller untuk ditampilkan di view.
  - Controller akan mengambil data hasil pengolahan model dan mengaturnya di bagian view untuk ditampilkan kepada pengguna.

---

## 5. Kelebihan & Kekurangan (refleksi singkat)
- Kelebihan
Menurut saya laravel cocok digunakan untuk pemula, karena struktur kodenya yang rapi jadi mudah untuk dipelajari. Laravel juga sudah menyediakan banyak fitur bawaan seperti login, routing, sampai database, jadi tidak perlu mulai dari awal.

- Kekurangan
Kekurangannya yaitu laravel sangat bergantung pada jaringan, jadi jika jaringan kita sedang tidak stabil performanya akan menurun.


---

## 6. Referensi
- https://www.dicoding.com/blog/apa-itu-mvc-pahami-konsepnya/
- https://www.hostinger.com/id/tutorial/- apa-itu-laravel#Artisan_CLI
- https://www.dicoding.com/blog/- kenalan-dengan-laravel-framework-php-yang-keren-dan-serbaguna/
- https://medium.com/@darshitabaldha2001/laravel-fundamentals-components-f03e8c2874b7
- https://www.barajacoding.or.id/mengenal-struktur-folder-dan-file-pada-laravel/
- https://www.dicoding.com/blog/apa-itu-mvc-pahami-konsepnya/
- https://laravel.com/docs/12.x/structure#the-resources-directory
---