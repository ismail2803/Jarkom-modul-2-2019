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

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNTg3MTQ4NywxMDUzNDYwMjEzLDcxNj
Y2OTQ1OCwtMTY2MDc3NTg2MCwtMTE0NDA2NTk3MCwtNTMxMzI1
NDA1LC02Nzc5MzkwMzEsMTMxOTQwOTM1LC03OTA1NjAyOTZdfQ
==
-->