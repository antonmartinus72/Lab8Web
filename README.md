

# PRAKTIKUM PEMROGRAMAN WEB

## Praktikum Pertemuan 10

Praktikum dilakukan dengan modul praktikum yang sudah disediakan.

- File praktikum terdapat pada folder **lab8_php_datababase**.
- File database terdapat pada folder **lab8_php_datababase** dengan nama **database.sql**.
- 

## 1. Membuat Database

Membuat database diawali dengan membuka alamat **localhost/phpmyadmin/** dan masuk ke tab SQL pada user interface phpMyAdmin lalu memasukan kode `CREATE DATABASE latihan1;`.

Pada kasus saya **localhost/phpmyadmin/** tidak dapat digunakan karena port default yang digunakan oleh aplikasi xampp  sudah digunakan oleh aplikasi lain.
Maka dari itu saya menggunakan **localhost:8080/phpmyadmin/** dengan mengubah konfigurasi yang terdapat pada server.

## 2. Membuat Tabel

Tabel akan dibuat didalam database sebelumnya. Maka dari itu harus masuk terlebih dahulu ke tabel yang sudah dibuat dan memasukan kode pada tab SQL seperti gambar dibawah ini.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/2.jpg)

Masukan kode seperti di atas untuk membuat kategori tabel seperti di bawah ini.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/2a.jpg)

## 2. Mengisi Tabel

Masukan kode berikut untuk mengisi nilai ke dalam tabel yang sudah dibuat.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/3.jpg)

Tabel yang sudah diisi akan terlihat seperti ini.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/3a.jpg)

## 2. Membuat Folder Untuk Program

Folder yang akan dibuat biasanya disimpan pada folder tertentu tergantung aplikasi server yang digunakan.
Di sini saya menggunakan **xampp versi 3.2.4** yang disimpan di partisi penyimpanan C pada sistem operasi windows.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/4.jpg)

Setelah folder dibuat, folder dapat dilihat pada browser.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/4a.jpg)

## 3. Membuat File Koneksi

Selanjutnya membuat file koneksi.php program didalam folder yang dibuat tadi.

Tujuan dibuat file koneksi adalah agar server dapat memberikan akses bagi program untuk dapat mengakses database yang ada pada server.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/5_code.jpg)

Jika koneksi berhasil, maka akan muncul pesan seperti ini dengan mengakses file koneksi.php pada browser. 

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/5.jpg)

## Menampilkan data

Menampilkan data dari database menggunakan operasi **read** dari empat operasi dasar yaitu **Create** (membuat), **Read** (membaca), **Update** (memperbarui) dan **Delete** (menghapus). Operasi read dapat membaca data  yang dipilih yang ada pada database dan menampilkannya pada browser.

Program dibuat didalam file **index.php**.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/6.jpg)

Kode yang digunakan :

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/6_code.jpg)

## Menambah data

Menambah data menggunakan operasi Create. Data yang di submit pada halaman ini akan disimpan ke dalam tabel pada database.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/7.jpg)

Kode yang digunakan :

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/7_code_a.jpg)

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/7_code_b.jpg)

## Memperbarui data

Memperbarui data (update) dilakukan dengan mengambil data dari database ke browser lalu mengirimkannya kembali ke server untuk disimpan setelah data selesai diubah.

Pada praktikum ini, aplikasi ubah data tidak dapat dilakukan dengan mengakses langsung file ubah.php karena tidak ada data yang dikirim terlebih dahulu ke halaman ubah.php maka dari itu akan muncul tampilan seperti berikut :

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/8.jpg)

Kode yang digunakan :

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/8_code_a.jpg)

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/8_code_b.jpg)

## Menghapus data

Menghapus data (Delete) digunakan untuk menghiangkan record pada tabel database.

Halaman hapus.php ini tidak akan melakukan dan menampilkan operasi apapun dengan membukanya langung pada browser.
Halaman ini hanya dapat melakukan operasi jika ada data yang dikirim dari halaman yang mengimkan data ke halaman hapus.php.

![enter image description here](https://github.com/antonmartinus72/Lab8Web/raw/main/Screenshoot/9_code.jpg)

## Kesimpulan

Program sederhana ini belum dapat melakukan seluruh operasi khususnya operasi update dan delete di karenakan halaman yang melakukan operasi tersebut tidak menerima data apapun dari halaman lainnya.

## Sekian & Terimakasih.