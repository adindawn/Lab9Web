# PRAKTIKUM 9: PHP MODULAR 

Nama   : ADINDA AULIA NABILA PUTRI

Nim    : 312410309

Kelas  : TI.24.A.4 

# LANGKAH-LANGKAH PRAKTIKUM 

# 1. MEMBUAT FILE DENGAN NAMA HEADER.PHP 

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

  Membuat folder ```lab9_php_modular``` pada docroot webserver```(htdocs)``` dengan file didalamnya ```header.php```. Pada file tersebut terdapat strukur dasar HTML yang terdiri dari ```header``` berisi judul "Modularisasi menggunakan Require" serta sebuah navigasi yang menyediakan tiga tautan menuju halaman ```home.php```, ```about.php```, dan ```kontak.php```. Seluruh elemen ditempatkan dalam sebuah ```div``` dengan ```class``` container agar tampilan lebih rapi dan teratur. Selain itu, halaman ini juga terhubung dengan file ```style.css```. 

  Berikut hasil pada Browser 

<img width="1363" height="390" alt="Screenshot 2025-11-27 222632" src="https://github.com/user-attachments/assets/53fb4bd6-98f0-43fc-93c0-7c24034d48ab" />

# 2. MEMBUAT FILE DENGAN NAMA FOOTER.PHP

```
 <footer> 
           <p>&copy; 2021, Informatika, Universitas Pelita Bangsa</p> 
       </footer> 
   </div> 
</body> 
</html>
```

  Membuat file baru di VSCode dengan nama ```footer.php```. Pada file tersebut terdapat informasi hak cipta berupa tulisan "2021, Informatika, Universitas Pelita Bangsa" sebagai identitas pemilik atau pembuat halaman. 

  Berikut hasil pada Browser 





# 3. MEMBUAT FILE DENGAN NAMA HOME.PHP 

```
<?php require('header.php'); ?> 
  
<div class="content"> 
   <h2>Ini Halaman Home</h2> 

    <p>Ini adalah bagian content dari halaman.</p> 
</div> 
  
<?php require('footer.php'); ?>
```

   Membuat file baru di VSCode dengan nama ```home.php```. Pada baris pertama file ini, terdapat file ```header.php``` ini untuk menampilkan bagian header dan navigasi secara otomatis tampa harus menuliskan ulang struktur di setiap halaman. Setelah itu, teerdapat sebuah ```div``` dengan ```class content```  yang berisi judul "ini Halaman Home" serta paragraf penjelasan sebagai isi utama halaman. Bagian akhir kode memanggil  ```footer.php``` yang berisi elemen footer sehingga halaman memiliki penutup yang konsisten dengan halaman lainnya. 

   Berikut hasil pada Browser 




# 4. MWMBUAT FILE DENGAN NAMA ABOUT.PHP 

```
<?php require('header.php'); ?> 
  
<div class="content"> 
   <h2>Ini Halaman About</h2> 
   <p>Ini adalah bagian content dari halaman.</p> 
</div> 
  
<?php require('footer.php'); ?>
```

   Membuat file baru di VSCode dengan nama ```about.php```. Pada baris pertama file ini, terdapat file ```header.php```  ini untuk menampilkan bagian header dan navigasi secara otomatis tampa harus menuliskan ulang struktur di setiap halaman. Setelah itu, terdapat  ```div```  dengan ```class content```  yang mrnsmpilkan judul halaman "ini Halaman About" serta paragraf penjelasan yang menjadin isi dari halaman tersebut. 

   Berikut Hasil pada Browser 




# PERTANYAAN DAN TUGAS 

<img width="601" height="503" alt="Screenshot 2025-11-28 103401" src="https://github.com/user-attachments/assets/d7bcc364-e6b7-47f5-a0c3-a68a98098f74" />


