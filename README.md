# Final-Project-OS-Server
- Nama : Muhammad Arita Hilmi
- Nim : 23.83.0981
- Judul : Pembuatan Web Server untuk Sistem Pemesanan Online dengan Apache

## Server
- Apache Web Server
- MySQL Database Server
- PHP
- HTTPS dengan Let's Encrypt
- Firewall (UFW)

## Progress
Berikut dibawah ini hanya proses minggu pertama dan bukan final!

## Install Apache web server
```bash
#Update sistem:
sudo apt update && sudo apt upgrade -y
#Instal Apache
sudo apt install apache2 -y
```

## Install PHP untuk Apache
```bash
#Instal PHP dan modul pendukung:
sudo apt install php libapache2-mod-php php-mysql -y
#file info.php
sudo nano /var/www/html/info.php
```

## Install MySQL
```bash
#Instal MySQL:
sudo apt install mysql-server -y
#Konfigurasi database
sudo mysql -u root -p
```

Konfigurasi HTTPS dengan Let's Encrypt
```bash
#Instal Certbot:
sudo apt install certbot python3-certbot-apache -y
#Dapatkan sertifikat SSL
sudo certbot --apache
```

Konfigurasi Firewall dengan UFW
```bash
#Aktifkan UFW:
sudo ufw enable
#Izinkan akses HTTP dan HTTPS
sudo ufw allow 'Apache Full'
```

