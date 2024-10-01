# TUGAS 6 

## Nama : Ramiya Nola Azhara
## Kelas : SK3B
## NIM : 09011182328089

### Tugas Cara Memasang dan Mengonfigurasi SSH di Ubuntu 22.04
### Langkah 1: Persiapan Ubuntu
Pertama, pastikan semua paket apt diperbarui ke versi terbaru. Gunakan perintah berikut untuk melakukan pembaruan:

![sudo apt update](https://github.com/user-attachments/assets/64ff87ce-5af8-4839-a4c6-75a25182abc5)

<br>

### Langkah 2: Instal SSH di Ubuntu
Jika OpenSSH belum terpasang, maka perlu diinstal secara manual. Jalankan perintah berikut untuk memulai proses instalasi:

![sudo apt install](https://github.com/user-attachments/assets/d49f2b0a-7e37-4e73-8c10-2d2d4edeb6b6)

<br>
Proses instalasi akan berjalan, dan pastikan untuk menyetujui semua permintaan konfirmasi dari sistem dengan memilih "Ya". Setelah instalasi selesai, lanjut ke langkah berikutnya untuk mengaktifkan layanan SSH.
<br>

### Langkah 3: Jalankan SSH
Setelah instalasi selesai, aktifkan layanan SSH yang baru terpasang dengan menjalankan perintah berikut:

![sudo systemctl enable](https://github.com/user-attachments/assets/905723e9-ce8d-4e02-bc32-7f13fcf1c610)

<br>
Setelah itu, periksa apakah layanan SSH sudah aktif dan berjalan dengan perintah ini:

![sudo status ssh](https://github.com/user-attachments/assets/91cd3928-7130-47f4-940a-3e126df060ba)

<br>
Jika output menampilkan "Aktif: aktif (berjalan)", artinya layanan SSH sudah berhasil dijalankan. Jika sewaktu-waktu perlu menonaktifkannya, gunakan perintah berikut:

![sudo disable](https://github.com/user-attachments/assets/372beef2-5dd2-4d0e-bbb2-a46521c1ed4b)

<br>
Perintah ini akan menonaktifkan layanan SSH dan mencegahnya berjalan secara otomatis saat booting.

<br>

### Langkah 4: Konfigurasikan firewall

Sebelum mencoba koneksi ke server melalui SSH, pastikan firewall sudah dikonfigurasi dengan benar. Jika UFW sudah terpasang, gunakan perintah berikut untuk memeriksa:.

![sudo ufw status active](https://github.com/user-attachments/assets/ad315747-4fd7-4e59-a695-01b4ff61aebd)

<br>
Jika output menunjukkan bahwa lalu lintas SSH diizinkan, berarti konfigurasi sudah benar. Namun, jika belum, perintah berikut bisa digunakan untuk membuka akses SSH:

![sudo ufw allow ssh](https://github.com/user-attachments/assets/e15bb0c3-7c95-4abb-869b-52f62fcdc2ab)

<br>

### Langkah 5: Koneksi ke server

Setelah semua langkah sebelumnya selesai, kini bisa mencoba masuk ke server menggunakan SSH. Diperlukan alamat IP atau nama domain server serta username yang ada di server tersebut. Gunakan perintah ini untuk menghubungkan:

![ssh peni-ilhami@](https://github.com/user-attachments/assets/6b90d286-19d9-48d9-82c3-4b2c986cc27d)

<br>
Pastikan SSH sudah terpasang dan dikonfigurasi baik di server jarak jauh maupun di komputer yang digunakan untuk memastikan koneksi berjalan dengan baik.
