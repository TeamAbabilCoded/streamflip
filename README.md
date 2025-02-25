<br>
<div align="center">
<img alt="LOGO" src="https://raw.githubusercontent.com/TeamAbabilCoded/streamflip/refs/heads/main/public/img/logo.png" width="420" height="auto" />
</div>
<br>



# StreamFlow: Aplikasi Live Streaming Multi-Window

StreamFlow adalah aplikasi live streaming yang memungkinkan kamu untuk melakukan siaran langsung ke berbagai platform seperti YouTube, Facebook, dan lainnya menggunakan protokol RTMP. Aplikasi ini berjalan di VPS (Virtual Private Server) dan mendukung streaming ke banyak platform sekaligus dengan fitur multi-window. StreamFlow juga dilengkapi dengan fitur login dan history streaming untuk melacak history streaming.
   <p align="center">
   <img alt="screenshot" src="https://raw.githubusercontent.com/TeamAbabilCoded/streamflip/refs/heads/main/public/img/screenshot.jpg" width="500px" height="auto" />
   </p>

## Fitur Utama:

* **Multi-Window Streaming:** Bisa melakukan streaming ke beberapa platform sekaligus dalam satu aplikasi.
* **Dukungan Banyak Platform:** Bisa streaming ke YouTube, Facebook, dan platform lain yang mendukung RTMP.
* **Login Page:** Ada fitur login supaya hanya pemilik akun yang bisa akses aplikasi.
* **Riwayat Streaming:** Semua aktivitas streaming tersimpan, jadi bisa dilihat kembali kapan saja.

## Cara Instalasi:

**Sebelum mulai:** Pastikan server / VPS kamu sudah terinstall Node.js, npm, dan FFmpeg sebelum meng-clone repositori ini.

1. **Install Node.js dan npm melalui NodeSource PPA:**

   ```bash
   curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
   sudo apt-get install -y nodejs
   sudo apt-get install -y npm
   ```
   Cek apakah instalasi berhasil:
   ```bash
   node -v
   npm -v
   ```

2. **Install FFmpeg:**

   ```bash
   sudo apt-get update
   sudo apt-get install -y ffmpeg
   ```
   Cek apakah instalasi berhasil:
   ```bash
   ffmpeg -version
   ```
   
3. **Install PM2:**

   ```bash
   npm install -g pm2
   ```

4. **Clone Repositori:**
   ```bash
   git clone https://github.com/TeamAbabilCoded/streamflip/
   cd streamflow
   ```

5. **Install Dependensi:**
   Jalankan `npm install` untuk menginstal semua modul Node.js yang dibutuhkan seperti Express.js, SQLite3, bcryptjs, dan lainnya.

   ```bash
   npm install
   ```

6. **Jalankan Aplikasi:**

   Kembali ke directory root (jika masih di directory streamflip)
   ```bash
   cd ..
   ```

   🚀 Perintah menjalankan aplikasi ✨
   ```bash
   pm2 start streamflip
   pm2 logs sstreamflip -i 0 --lines 1
   ```

   📈 Melihat status aplikasi berjalan
   ```bash
   pm2 status streamflip
   ```

   ⛔ Menghentikan aplikasi
   ```bash
   pm2 stop streamflip
   ```

8. **Konfigurasi:**
    * Pastikan kamu sudah mengatur URL RTMP yang sesuai untuk setiap platform yang ingin digunakan. Konfigurasi ini bisa dilakukan langsung melalui tampilan aplikasi.
    * Silahkan dapatkan Stream Key dari platform streaming yang kamu gunakan.

## Informasi Tambahan:

* Aplikasi ini menggunakan Express.js sebagai backend, SQLite sebagai database, dan FFmpeg untuk encoding serta streaming.
* Antarmuka pengguna dibuat dengan HTML, CSS, dan JavaScript, serta menggunakan Tailwind CSS untuk styling.
* Aplikasi ini dirancang untuk berjalan di server dengan Node.js, bukan di browser lokal.

## Kontribusi:

Jika teman-teman punya ide atau perbaikan koding aplikasi ini, silakan buat pull request 🤝

## Traktir Kopi:

[Traktir Kopi](https://saweria.co/KarDeBleach)

## Ucapan:

☺️ Thank you udah support [Kar De Bleach](https://youtube.com/KarDeBleach) dalam pengembangan aplikasi ini.

## Lisensi:

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/TeamAbabilCoded/streamflip/blob/main/LICENSE)

Hak Cipta © 2025 - [Kar De Bleach](https://youtube.com/KarDeBleach)
