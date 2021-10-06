# How To Use

<br>

# Installation step / Langkah Instalasi
## Step2 (Indonesia)


- Download versi (ID) / (ENG) [Pilih satu]

- Extract Zip file

- Pindahkan ke folder web server Seperti <b>var/www/html</b> atau yang lainnya

- Jika kamu menggunakan paket seperti xampp / mamp / wampp pindahkan ke htodcs folder

- SetUp WordPress <a href='https://www.hostinger.co.id/tutorial/cara-install-wordpress-di-xampp/'>Disini</a>

<hr>

## Step2 (English)
- Download (ID) / (ENG) Version [Choose one]

- Extract Zip file

- Move to web server folder like var/www or something else

- If u use xampp / mamp / wampp move to htodcs folder

- SetUp WordPress <a href='https://themeisle.com/blog/install-xampp-and-wordpress-locally/'</a>
<br>
<br>
# Konfigurasi (Configuration) [php.ini file]

- Set up / setting file <i>"php.ini"</i> pada php nya 
- Ubah file nya dengan text editor
- Ubah Bagian : 
```
post_max_size = 750M 
upload_max_filesize = 750M 
max_execution_time = 5000
max_input_time = 5000  
memory_limit = 1000M
```
- <sub>Tujuan : Agar tidak terjadi limit pada upload file</sub>
<br>
<br>

# Nonaktifkan FTP (FTP / FTP SSL REDIRECT) [wp-config.php file]
- Buka File <i>"wp-config.php"</i> pada folder wordpress yang di extract tadi.
- Tambahkan ini di file "<i>wp-config.php</i>" : 
```
define('FS_METHOD', 'direct');
```
- <sub>Tujuan : Agar tidak terjadi ftp force redirect</sub>
- nonaktifkan server lalu aktifkan kembali.
- buka localhost, lalu arahkan ke path folder dan filenya.