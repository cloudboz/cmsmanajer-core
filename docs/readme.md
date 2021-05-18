# Business Flow

# Requirements
- Your server must be Ubuntu 18.04 or 20.04 (64-bit). 
- Only clean servers (no Nginx, Apache, or MySQL installed) can be connected to CMS Manajer.
- Installed python2.7 or python3.
- Minimum of RAM 256MB

# How to Use

## Todo
- [ ] Generate ssh-key with  `ssh-keygen` > files/`id_rsa` & files/`id_rsa.pub`
- [ ] Create user `cmsmanajer`
- [ ] Copy files/`id_rsa` & files/`id_rsa.pub` > `~/.ssh/`
- [ ] Install LEMP (Linux, Engine-X, MariaDB and PHP)
- [ ] Install LAMP (Linux, Apache, MariaDB and PHP)
- [ ] Install LEMP + CMS `WordPress`
- [ ] Install SFTP
Enabling automatic package updates.
install postfix
php-fpm
testing server configuration

---

Step by step

{Koneksi vps ke cmsmanajer}

- Membuat sebuah vps di salah satu provider contoh : vultr / digitalocean
- Copy semua data username, password dan ip servernya
- Login / Register di cmsmanajer
- Klik tambahkan server kemudian masukkan ip, username dan password vps
- Terdapat pilihan :
    - Checklist - optimize your server jika ingin mengoptimasi servernya (update dan upgrade sistem, mengganti konfigurasi default menjadi optimize pada ulimit, kernel sistem).
    - Checklist - monitoring server seperti penggunaan memory, cpu dan storage.
    - Secara default cmsmanajer akan install sftp, membuat user baru (cmsmanajer), generate ssh-key dan copy ssh-key ke server

- Melakukan git push code ansible ke repo cmsmanajer

---

{Instalasi aplikasi pada cmsmanajer}

- Pada menu apps pilih aplikasi yang akan di setup :
    - LEMP (Linux, Engine-X, MariaDB dan PHP)
    - LAMP (Linux, Apache2, MariaDB dan PHP)
    - WordPress (Bisa milih Apache / Nginx)
    - Drupal (Bisa milih Apache / Nginx)
    - Joomla (Bisa milih Apache / Nginx)
    - Masih banyak lagi listnya

- Contoh klik install WordPres, kemudian ada pilihan Apache / Nginx.

- Masukkan nama domain yang akan digunakan (bisa menggunakan subdomain / ip:port jika aplikasi lebih dari 1 pada server)

- Klik deploy setelah itu akan melakukan proses setup (tunggu hingga selesai)

---

