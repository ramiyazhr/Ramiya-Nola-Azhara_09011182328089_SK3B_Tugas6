# TUGAS 6 

## Nama : Ramiya Nola Azhara
## Kelas : SK3B
## NIM : 09011182328089

### Tugas Cara Memasang dan Mengonfigurasi SSH di Ubuntu 22.04
### Langkah 1: Siapkan Ubuntu
Memperbarui semua paket apt ke versi terbaru. Untuk melakukannya, gunakan perintah berikut:





<br>

### Langkah 2: Instal SSH di Ubuntu
OpenSSH belum terinstal di sistem, jadi mari kita instal secara manual. Untuk melakukannya, ketik di terminal:



<br>
Instalasi semua komponen yang diperlukan akan dimulai. Jawab "Ya" untuk semua perintah sistem.
Setelah instalasi selesai, lanjutkan ke langkah berikutnya untuk memulai layanan.
<br>

### Langkah 3: Jalankan SSH
Sekarang Anda perlu mengaktifkan layanan yang baru saja Anda instal menggunakan perintah di bawah ini:





<br>
Untuk memverifikasi bahwa layanan diaktifkan dan berjalan dengan sukses





<br>
Outputnya harus berisi baris Aktif: aktif (berjalan), yang menunjukkan bahwa layanan berhasil berjalan.
<br>Jika Anda ingin menonaktifkan layanan, jalankan:





<br>
Ini menonaktifkan layanan dan mencegahnya memulai saat boot.

<br>

### Langkah 4: Konfigurasikan firewall

Sebelum menghubungkan ke server melalui SSH, periksa firewall untuk memastikannya dikonfigurasi dengan benar.
<br>Dalam kasus kami, kami telah menginstal UFW, jadi kami akan menggunakan perintah berikut:




<br>
Pada output, Anda akan melihat bahwa lalu lintas SSH diizinkan. Jika tidak tercantum, Anda perlu mengizinkan koneksi SSH yang masuk. Perintah ini akan membantu Anda:






<br>

### Langkah 5: Hubungkan ke server

Setelah Anda menyelesaikan semua langkah sebelumnya, Anda dapat masuk ke server menggunakan protokol SSH.
<br>Untuk melakukannya, Anda memerlukan alamat IP atau nama domain server dan nama pengguna yang dibuat di server. Masukkan perintah:






<br>
Agar berhasil tersambung ke server jarak jauh, SSH harus diinstal dan dikonfigurasi di server jarak jauh dan komputer pengguna tempat Anda membuat sambungan.
