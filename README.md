# PRAKTIKUM 9: PHP MODULAR 

Nama   : ADINDA AULIA NABILA PUTRI

Nim    : 312410309

Kelas  : TI.24.A.4 

# LANGKAH-LANGKAH PRAKTIKUM 


# MEMBUAT FILE KONEKSI.PHP 

```
<?php 
$host = "localhost"; 
$user = "root"; 
$pass = ""; 
$db   = "latihan1"; 

$conn = mysqli_connect($host, $user, $pass, $db); 
if ($conn == false) 
{ 
   echo "Koneksi ke server gagal."; 
   die(); 
} #else echo "Koneksi berhasil"; 
?>
```

  Membuat folder ```lab9_php_modular``` pada docroot webserver```(htdocs)``` dengan file didalamnya ```koneksi.php```. File ini berfungsi untuk membuat koneksi antara aplikasi PHP dengan database MySQL. Didalam file ini ditulis konfigurasi seperti nama host, username, password, dan nama database yang digunakan, yaitu latihan 1. Selanjutnya, fungsi ```mysql_connect()``` dipakai untuk menghubungkan PHP dengan database bedasarkan data konfigurasi tersebut. Setelah itu dilakukan pengecekkan, apakah koneksi berhasil atau gagal. Jika gagal, maka program akan menampilkan pesan "koneksike server gagal" dan proses akan dihentikan menggunakan ```die()```.

# MEMBUAT FILE DENGAN NAMA HEADER.PHP 

```
<!DOCTYPE html> 
<html lang="en"> 
<head> 
   <meta charset="UTF-8"> 
   <title>Contoh Modularisasi</title> 
   <link href="style.css" rel="stylesheet" type="text/stylesheet" 
media="screen" /> 
</head> 
<body> 
   <div class="container"> 
       <header> 
           <h1>Modularisasi Menggunakan Require</h1> 
       </header> 
       <nav> 
           <a href="home.php">Home</a> 
           <a href="about.php">Tentang</a> 
           <a href="kontak.php">Kontak</a> 
       </nav>
```

  Membuat file baru di VSCode dengan nama ```header.php```. Pada file tersebut terdapat strukur dasar HTML yang terdiri dari ```header``` berisi judul "Modularisasi menggunakan Require" serta sebuah navigasi yang menyediakan tiga tautan menuju halaman ```home.php```, ```about.php```, dan ```kontak.php```. Seluruh elemen ditempatkan dalam sebuah ```div``` dengan ```class``` container agar tampilan lebih rapi dan teratur. Selain itu, halaman ini juga terhubung dengan file ```style.css```. 


# MEMBUAT FILE DENGAN NAMA FOOTER.PHP

```
 <footer> 
           <p>&copy; 2025, Informatika, Universitas Pelita Bangsa</p> 
       </footer> 
   </div> 
</body> 
</html>
```

  Membuat file baru di VSCode dengan nama ```footer.php```. Pada file tersebut terdapat informasi hak cipta berupa tulisan "2025, Informatika, Universitas Pelita Bangsa" sebagai identitas pemilik atau pembuat halaman.


# MEMBUAT FILE DENGAN NAMA HOME.PHP 

```
<?php require('header.php'); ?> 
  
<div class="content"> 
   <h2>Ini Halaman Home</h2>

    <p>Selamat Datang di Aplikasi PHP Modular. Ini adalah halaman utama yang dibuat menggunakan 
        konsep Modularisasi.</p> 
</div> 

```

   Membuat file baru di VSCode dengan nama ```home.php```. Pada baris pertama file ini, terdapat file ```header.php``` ini untuk menampilkan bagian header dan navigasi secara otomatis tampa harus menuliskan ulang struktur di setiap halaman. Setelah itu, teerdapat sebuah ```div``` dengan ```class content```  yang berisi judul "ini Halaman Home" serta paragraf penjelasan sebagai isi utama halaman. Bagian akhir kode memanggil  ```footer.php``` yang berisi elemen footer sehingga halaman memiliki penutup yang konsisten dengan halaman lainnya. 

   Berikut hasil pada Browser 

<img width="1022" height="260" alt="Screenshot 2025-11-28 161722" src="https://github.com/user-attachments/assets/9df51510-c3ca-4ffb-bbd4-9813e2470547" />



# MEMBUAT FILE DENGAN NAMA ABOUT.PHP 

```
<?php require('header.php'); ?> 
  
<div class="content"> 
   <h2>Ini Halaman About</h2> 
   <p>Aplikasi ini dibuat sebagai latihan Penerapan Modularisasi pada PHP, matakuliah Pemrograman Web 1.
    Konsep Modularisasi pada Aplikasi PHP, yaitu memisahkan bagian-bagian halaman seperti header, footer, dan konten dalam file terpisah.
    Dengan Modularisasi, struktur program menjadi lebih rapi.</p> 
</div> 
```

   Membuat file baru di VSCode dengan nama ```about.php```. Pada baris pertama file ini, terdapat file ```header.php```  ini untuk menampilkan bagian header dan navigasi secara otomatis tampa harus menuliskan ulang struktur di setiap halaman. Setelah itu, terdapat  ```div```  dengan ```class content```  yang menampilkan judul halaman "ini Halaman About" serta paragraf penjelasan yang menjadin isi dari halaman tersebut. 

   Berikut Hasil pada Browser 

<img width="1021" height="277" alt="Screenshot 2025-11-28 162003" src="https://github.com/user-attachments/assets/9076604a-3abc-473e-a7dd-1cb4aef32dee" />

# MEMBUAT FILE DENGAN NAMA KONTAK.PHP

```
<?php require('header.php'); ?>

<div class="content">
    <h2>Kontak</h2>
    <p>Jika Anda memiliki pertanyaan atau membutuhkan informasi lebih lanjut, Anda dapat menghubungi kami melalui Informasi di bawah ini.</p>

    <p><strong>Telepon:</strong> 0823-1043-0259</p>
    <p><strong>Email:</strong> adindaaulia806@gmail.com</p>
    <p><strong>Alamat:</strong> Bekasi, Jawa Barat</p>
</div>
```

  Membuat file baru di VSCode dengan nama ```kontak.php```. File ini dibuat untuk halaman kontak sederhana yang menampilkan informasi yang dapat dihubungkan oleh pengguna. Halaman ini tetap menggunakan konsep modular dengan memanggil ```header.php``` dan ```footer.php```, sehingga tampilannya konsisten dengan halaman lainnya. 

  Berikut hasil pada Browser 

<img width="1009" height="349" alt="Screenshot 2025-11-28 162928" src="https://github.com/user-attachments/assets/db6cce0b-876c-4e6c-a4d9-6b230d0095b0" />


# PERTANYAAN DAN TUGAS 

<img width="601" height="503" alt="Screenshot 2025-11-28 103401" src="https://github.com/user-attachments/assets/d7bcc364-e6b7-47f5-a0c3-a68a98098f74" />

# DATA BARANG 

<img width="1193" height="381" alt="Screenshot 2025-11-28 161041" src="https://github.com/user-attachments/assets/2a35383d-08a3-4be3-9e5d-b6631453a9bb" />

# TAMBAH BARANG 

<img width="1192" height="589" alt="Screenshot 2025-11-28 160906" src="https://github.com/user-attachments/assets/2725dec7-e8da-4204-9f1f-bd380a185b48" />

# UBAH BARANG

<img width="1184" height="594" alt="Screenshot 2025-11-28 160958" src="https://github.com/user-attachments/assets/21c9aa54-3769-4fca-bb0e-f7a9328427d4" />

# HAPUS BARANG 

<img width="1365" height="501" alt="Screenshot 2025-11-28 161103" src="https://github.com/user-attachments/assets/97ebc739-a6a6-44f5-8324-97a609ca18a7" />



