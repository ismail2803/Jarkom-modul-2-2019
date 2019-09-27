# Web Server
## A. Persyaratan Tambahan untuk Mengikuti Sesi Lab
Record A dan PTR pada jarkomtc.com mengarah ke IP MEWTWO

<img src="Gambar/1.png" width="500">

<img src="Gambar/2.png" width="500">

## B. Penting Untuk Dibaca
1. Pastikan semua UML bisa connect ke internet baik dapat melakukan koneksi ke luar maupun dapat ping dari luar (Khusus DMZ)
2. Pastikan Mewtwo dan Articuno sudah memiliki memory 256M
3. Ketika mengalami kendala/error __cek syntax dan samakan seperti modul__ terlebih dahulu __sebelum__ angkat tangan dan berkata __"Mas/Mbak ini kok gak bisa ya?"__

## C. Dasar Teori
### 1. Web Server
Terdapat dua pengertian dari web server. Secara _hardware_, web server berarti sebuah storage yang digunakan untuk menyimpan semua data dari aplikasi web (file HTML, CSS, JavaScript, dll.). Sedangkan secara _software_,  web server adalah sebuah perangkat yang bertugas untuk menyediakan layanan akses menggunakan protokol HTTP atau HTTPS melalui aplikasi web.

### 2. Load Balancing
#### Kenapa dibutuhkan load balancing?

### 3. Apache Web Server

## D. Instalasi Apache
#### 1. Buka UML _MEWTWO_
Lalu jalankan perintah
```
apt-get install apache2
```
jika muncul tulisan _"Do you want to continue? [Y/n]"_  input `Y` lalu tekan ___enter___. 

<img src="Gambar/3.png" width="500">

#### 2. Buka browser laptop/komputer masing-masing
Buka web __IP Mewtwo Masing-Masing Kelompok__ sampai muncul halaman Apache seperti di bawah ini.

<img src="Gambar/4.png">

## E. Instalasi PHP
#### 1. Buka UML Mewtwo
Lalu jalankan perintah
```
apt-get install php5
```
jika muncul tulisan _"Do you want to continue? [Y/n]"_  input `Y` lalu tekan ___enter___. 

<img src="Gambar/5.png" width="500">

#### 2. Test apakah php sudah ter-install
Jalankan perintah di bawah ini untuk memeriksa versi dari __php__ kalian.
```
php -v
```
Bila _output_-nya mirip dengan yang di bawah ini, maka __php__ kalian telah ter-_install_.

<img src="Gambar/6.png" width="500">

## F. Mengenal Apache
Web server Apache memiliki _directory_  berisi berbagai konfigurasi yang terletak di `/etc/apache2/`

<img src="Gambar/7.png" width="500">

Berikut beberapa hal yang penting untuk diketahui:
+ File Konfigurasi di 	`/etc/apache2`

|__Nama File__ | __Kegunaan__ |
| --- | --- |
| __apache2.conf__ | file |

+ _Command_ yang sering digunakan

|__Command__ | __Kegunaan__ |
| --- | --- |
| __a2ensite__ | file |
| __a2dissite__ | file |
| __a2enmod__ | file |
| __a2dismod__ | file |

## G. Konfigurasi Apache Sederhana
### A. Penggunaan Sederhana
#### A.1. Pindah ke _directory_ `/etc/apache2/sites-available`
Gunakan perintah `cd /etc/apache2/sites-available`

<img src="Gambar/8.png" width="500">

Dapat dilihat di sana terdapat dua buah file:
+ file __default__, ....
+ file __default-ssl__, ....
#### A.2. Buka file ___default___
Gunakan perintah `nano /etc/apache2/sites-available/default`

<img src="Gambar/9.png" width="500">

#### 3.  Pada file _default_ terdapat konfigurasi standar apache
Beberapa diantaranya adalah:
+ __Port__ yang digunakan
```
```
+ Nama __Domain__
```
```
+ ___Directory___ tempat file website kita berada
```
```
#### 4. Pindah ke _directory_ yang ditunjuk oleh _DocumentRoot_ pada file _default_
Gunakan perintah `cd /var/www/html`
#### 5. Buat file _index.php_
Gunakan perintah `nano index.php` dan isi file  tersebut dengan
```
<?php
	phpinfo();
?>
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3NjgzMDQzNDMsMTM4NzM3NzA1NCwyMD
QyOTkxNzcxLC0xNjE3MTQ2MzMsLTg4MjQxNjIzMCwtNTYwNTQy
MTE0LC02NTA0OTE2MTEsLTIwNTg3MTQ4NywxMDUzNDYwMjEzLD
cxNjY2OTQ1OCwtMTY2MDc3NTg2MCwtMTE0NDA2NTk3MCwtNTMx
MzI1NDA1LC02Nzc5MzkwMzEsMTMxOTQwOTM1LC03OTA1NjAyOT
ZdfQ==
-->