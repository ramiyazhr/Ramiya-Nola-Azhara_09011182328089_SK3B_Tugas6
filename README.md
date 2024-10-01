# TUGAS 6 

## Nama : Ramiya Nola Azhara
## Kelas : SK3B
## NIM : 09011182328089

### Tugas Cara Memasang dan Mengonfigurasi SSH di Ubuntu 22.04
### Langkah 1: Persiapan Ubuntu
Pertama, pastikan semua paket apt diperbarui ke versi terbaru. Gunakan perintah berikut untuk melakukan pembaruan:





<br>

### Langkah 2: Instal SSH di Ubuntu
Jika OpenSSH belum terpasang, maka perlu diinstal secara manual. Jalankan perintah berikut untuk memulai proses instalasi:



<br>
Proses instalasi akan berjalan, dan pastikan untuk menyetujui semua permintaan konfirmasi dari sistem dengan memilih "Ya". Setelah instalasi selesai, lanjut ke langkah berikutnya untuk mengaktifkan layanan SSH.
<br>

### Langkah 3: Jalankan SSH
Setelah instalasi selesai, aktifkan layanan SSH yang baru terpasang dengan menjalankan perintah berikut:




<br>
Setelah itu, periksa apakah layanan SSH sudah aktif dan berjalan dengan perintah ini:





<br>
Jika output menampilkan "Aktif: aktif (berjalan)", artinya layanan SSH sudah berhasil dijalankan. Jika sewaktu-waktu perlu menonaktifkannya, gunakan perintah berikut:






<br>
Perintah ini akan menonaktifkan layanan SSH dan mencegahnya berjalan secara otomatis saat booting.

<br>

### Langkah 4: Konfigurasikan firewall

Sebelum mencoba koneksi ke server melalui SSH, pastikan firewall sudah dikonfigurasi dengan benar. Jika UFW sudah terpasang, gunakan perintah berikut untuk memeriksa:.





<br>
Jika output menunjukkan bahwa lalu lintas SSH diizinkan, berarti konfigurasi sudah benar. Namun, jika belum, perintah berikut bisa digunakan untuk membuka akses SSH:






<br>

### Langkah 5: Koneksi ke server

Setelah semua langkah sebelumnya selesai, kini bisa mencoba masuk ke server menggunakan SSH. Diperlukan alamat IP atau nama domain server serta username yang ada di server tersebut. Gunakan perintah ini untuk menghubungkan:





<br>
Pastikan SSH sudah terpasang dan dikonfigurasi baik di server jarak jauh maupun di komputer yang digunakan untuk memastikan koneksi berjalan dengan baik.
