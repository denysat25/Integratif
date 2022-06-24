# Tugas Besar Pemrograman Integratif
**Deny Satria Ardi  1202190026 || IT 02-01** 

<br />

-----

### Tahap 1 
#### Install PHP

•	Download php di website https://windows.php.net/download#php-8.1. Pilih file zip Thread Safe

  ![](Assets/001.jpg)

•	Ekstrak file php, kemudian copy di lokasi “ C:\Program Files “. Cari file bernama "php.ini development", buat salinan dan ubah nama file salinan menjadi  “php.ini”.     buka menggunakan text editor, dan jadikan seperti pada gambar, kemudian simpan.

  ![](Assets/002.png)
  ![](Assets/003.jpg)
  
•	Buka “Edit The System Environment Variables”, klik Environment Variables

  ![](Assets/004.png)
  
•	Pilih variabel path untuk menambahkan alamat dari file php, kemudian pilih ok.

  ![](Assets/005.png)

•	Buka terminal dan ketikkan ``php –v``, maka akan muncul tampilan seperti digambar, yang artinya php berhasil terinstall.

  ![](Assets/006.png)

### INSTALL COMPOSER

•	Downlaod Composer https://getcomposer.org/download/

  ![](Assets/007.png)

•	Install file composer seperti biasa. Jika sudah buka terminal dan ketik “composer”, maka akan muncul tampilan seperti digambar, yang mana composer sudah terinstall.

  ![](Assets/008.png)

### INSTALL LARAVEL VIA COMPOSER 

•	Buka website https://laravel.com/docs/9.x#installation-via-composer, untuk menyalin command installasi laravel via composer

•	Buat folder baru di komputer untuk menginstall laravel (bebas lokasinya). Klik kanan dan buka dengan Git Bash Here

  ![](Assets/009.png)
 
 •	Buat project untuk install laravel dengan command
 
```
composer create-project laravel/laravel nama_project
```
  ![](Assets/010.png)
  ![](Assets/011.png)

•	Masuk  terlebih dahulu ke folder project yang sudah dibuat dengan command
```
cd pintegratif/
```
• Kemudian buka file installasi laravel dengan text editor (disini dengan visual studio code) dengan command 
```
code ./pintegratif
```
  ![](Assets/012.png)
  
• Maka akan secara otomatis membuka aplikasi visual studio code
•	Klik menu terminal pada bagian atas, pilih terminal baru, lalu masukkan command
```
php artisan serve
```
  ![](Assets/013.png)
  
•	Copy server laravel, untuk dibuka di browser

  ![](Assets/014.png)
  
<br />

-----
### Tahap 2
•	Ubah DB_DATABASE di .env sesuai dengan nama database yang dibuat di phpmyadmin

  ![](Assets/015.jpg)
  ![](Assets/016.jpg)

• Buat 2 table rss dan news dengan fitur migrations menggunakan perintah
  ```
  php artisan make:migration create_rss_table
  
  php artisan make:migration create_news_table
  ```
• Tambahkan kolom name dan url pada tabel rss, seperti pada gambar dibawah
  ![](Assets/017.jpg)

• Tambahkan kolom title, img_url, description, source_url,  dan rss_id pada tabel news, seperti pada gambar dibawah
  ![](Assets/018.jpg)

• Untuk menjalankan migrasi yang dibuat jalankan perintah diterminal seperti dibawah, lalu cek database
  ```
  php artisan migrate
  ```
  ![](Assets/019.jpg)

• Buat koneksi  model  ke database  dengan membuat seeder dan controller untuk tabel Rss dan News, dengan perintah
  ```
  php artisan make:model Rss –seed –controller
  ``
  ![](Assets/020.jpg)
  ```
  php artisan make:model Rss –seed –controller
  ``
  ![](Assets/021.jpg)
• Edit file Rss.php, RssSeeder.php serta DatabaseSeeder.php seperti pada gambar dibawah
  ![](Assets/022.jpg)
  ![](Assets/023.jpg)
  ![](Assets/024.jpg)
  
• Kemudian cek koneksi dengan perintah
  ```
  php artisan db:seed
  ```
  ![](Assets/025.jpg)
  
• Edit file News.php, NewsController.php, web.php, serta file migration News seperti pada gambar dibawah
  ![](Assets/026.jpg)
  ![](Assets/027.jpg)
  ![](Assets/028.jpg)
  ![](Assets/029.jpg)

• Cek localhost di http://127.0.0.1:8000/aggregrate/1 dan di database phpmyadmin
  ![](Assets/030.jpg)
  ![](Assets/031.jpg)
  
