# Tahapan Install Laravel

## INSTALL PHP
•	Download php di website https://windows.php.net/download#php-8.1 

•	Ekstrak file php, kemudian copy di lokasi “ C:\Program Files “.

•	Cari file bernama php.ini development, buat salinan dan ubah nama file salinan menjadi  “php.ini”. 

•	Buka file salinan tersebut menggunakan text editor, ubah script dibeberapa part, kemudian simpan.

•	Buka “Edit The System Environment Variables”, klik Environment Variables

•	Pilih variabel path untuk menambahkan alamat dari file php, kemudian pilih ok.

•	Buka terminal dan ketikkan php –v, untuk memeriksa apakah php sudah berhasil terinstall

## INSTALL COMPOSER
•	Downlaod Composer https://getcomposer.org/download/

•	Install file composer seperti biasa. Jika sudah buka terminal dan ketik “composer”, untuk memeriksa composer sudah terinstall atau belum.

## INSTALL LARAVEL VIA COMPOSER
•	Buka website https://laravel.com/docs/9.x#installation-via-composer, untuk menyalin command installasi laravel via composer

•	Buat folder baru di komputer untuk menginstall laravel (bebas lokasinya). Klik kanan dan buka dengan Git Bash Here (jika sudah menginstall git).

•	Buat project untuk install laravel dengan command

``composer create-project laravel/laravel nama_project``

•	Masuk  terlebih dahulu ke folder project yang sudah dibuat dengan command

``cd pintegratif/``

•	Dan jalankan project dengan command

``php artisan serve``

•	Copy server laravel, untuk dibuka di browser
