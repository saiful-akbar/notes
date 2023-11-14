# 1. Linux Ubuntu

## 1.1. Perintah dasar terminal ubuntu

### 1.1.1. Navigasi dan Manajemen Direktori:
- **`pwd`** : Menampilkan direktori kerja saat ini.
- **`ls`** : Menampilkan daftar file dan direktori di direktori saat ini.
- **`cd`** : Mengganti direktori kerja.

### 1.1.2. Manipulasi File dan Direktori:
- **`mkdir`** : Membuat direktori baru.
- **`touch`** : Membuat file kosong.
- **`cp`** : Menyalin file atau direktori.
- **`mv`** : Memindahkan atau mengganti nama file/direktori.`
- **`rm`** : Menghapus file atau direktori.

### 1.1.3. Perintah Pencarian:
- **`find`** : Mencari file atau direktori.

### 1.1.4. Perintah Informasi Sistem:
- **`uname`** : Menampilkan informasi kernel sistem.
- **`lsb_release`** : Menampilkan informasi distribusi.

### 1.1.5. Manajemen Proses:
- **`ps`** : Menampilkan daftar proses yang berjalan.
- **`kill`** : Menghentikan proses.

### 1.1.6. Paket dan Manajemen Aplikasi:
- **`apt-get` (atau apt)`**: Manajemen paket Debian.
- **`dpkg`** : Manajemen paket yang terinstal.

### 1.1.7. Perintah Izin File:
- **`chmod`** : Mengubah izin file/direktori.

### 1.1.8. Perintah Pencarian Teks:
- **`grep`** : Mencari teks dalam file.

### 1.1.9. Perintah Kompresi/Decompression:
- **`tar`** : Mengompresi/dekompresi file/direktori.

### 1.1.10. Networking:
- **`ifconfig`** : Menampilkan informasi antarmuka jaringan.
- **`ping`** : Mengirim paket ke host jaringan.
- **`ssh`** : Menghubungkan ke mesin jarak jauh dengan SSH.
- **`netstat`** : Menampilkan informasi koneksi jaringan.

## 1.2 Install XAMPP
- Download xampp untuk linux [disini](https://www.apachefriends.org/download.html).
- Buka terminal `ctrl+alt+t` dan arahkan pada folder tempat aplikasi berada, contoh: download.
  ```bash
  cd ~/Download
  ```
- Jalankan perintah berikut untuk merubah permission (izin) file agar bisa diinstal.
  ```bash
  sudo chmod +x ./{nama_aplikasi}.run
  ```
- Jalankan perintah berikut untu memulai proses instalasi.
  ```bash
  sudo ./{nama_aplikasi}.run
  ```
- Buka file `~/.bashrc` pada text editor lalu tambahkan script berikut:
  ```bash
  export PATH=$PATH:/opt/lampp/bin
  ```
- Kembali ke terminal dan jalankan perintah berikut:
  ```bash
  source ~/.bashrc
  ```

# 2. Windows

## 2.1. Activasi MS Office.
- Buka folder di local disk `C:/`
- Lalu cari folder `Program Files (x86)` atau `Program Files`.
- Buka Program `Files (x86)` untuk Office 32-bit `Program Files` untuk Office 64-bit.
- Cari dan masuk ke folder `Microsoft Office`.
- Lalu masuk ke dalam folder Office sesuai dengan versi yang kamu gunakan. (Office10, Office13, Office16, atau Office19)
- Cari dan jalankan `OSPPREARM.EXE` dengan Administrator
- Tekan YES dan tunggu beberapa waktu sampai proses selesai.
