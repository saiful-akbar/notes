# Catatan

# 1. Linux Ubuntu
## 1.1. Perintah dasar terminal ubuntu

### 1.1.1. Navigasi dan Manajemen Direktori:
- `pwd`: Menampilkan direktori kerja saat ini.
- `ls`: Menampilkan daftar file dan direktori di direktori saat ini.
- `cd`: Mengganti direktori kerja.
  - Contoh: `cd /path/ke/direktori`

### 1.1.2. Manipulasi File dan Direktori:
- `mkdir`: Membuat direktori baru.
  - Contoh: `mkdir nama_direktori`
- `touch`: Membuat file kosong.
  - Contoh: `touch nama_file`
- `cp`: Menyalin file atau direktori.
  - Contoh: `cp sumber tujuan`
- `mv`: Memindahkan atau mengganti nama file/direktori.
  - Contoh: `mv sumber tujuan`
- `rm`: Menghapus file atau direktori.
  - Contoh: `rm nama_file` (hati-hati dengan perintah ini)

### 1.1.3. Perintah Pencarian:
- `find`: Mencari file atau direktori.
  - Contoh: `find /path -name nama_file`

### 1.1.4. Perintah Informasi Sistem:
- `uname`: Menampilkan informasi kernel sistem.
  - Contoh: `uname -a`
- `lsb_release`: Menampilkan informasi distribusi.
  - Contoh: `lsb_release -a`

### 1.1.5. Manajemen Proses:
- `ps`: Menampilkan daftar proses yang berjalan.
  - Contoh: `ps aux`
- `kill`: Menghentikan proses.
  - Contoh: `kill PID` (PID adalah ID proses)

### 1.1.6. Paket dan Manajemen Aplikasi:
- `apt-get` (atau `apt`): Manajemen paket Debian.
  - Contoh: `sudo apt-get install nama_paket`
- `dpkg`: Manajemen paket yang terinstal.
  - Contoh: `dpkg -l`

### 1.1.7. Perintah Izin File:
- `chmod`: Mengubah izin file/direktori.
  - Contoh: `chmod permissions nama_file`

### 1.1.8. Perintah Pencarian Teks:
- `grep`: Mencari teks dalam file.
  - Contoh: `grep kata_kunci nama_file`

### 1.1.9. Perintah Kompresi/Decompression:
- `tar`: Mengompresi/dekompresi file/direktori.
  - Contoh: `tar -czvf arsip.tar.gz direktori`

### 1.1.10. Networking:
- `ifconfig`: Menampilkan informasi antarmuka jaringan.
- `ping`: Mengirim paket ke host jaringan.
- `ssh`: Menghubungkan ke mesin jarak jauh dengan SSH.
- `netstat`: Menampilkan informasi koneksi jaringan.

# 2. Windows

## 2.1. Activasi MS Office.
- Buka folder di local disk `C:/`
- Lalu cari folder `Program Files (x86)` atau `Program Files`.
- Buka Program `Files (x86)` untuk Office 32-bit `Program Files` untuk Office 64-bit.
- Cari dan masuk ke folder `Microsoft Office`.
- Lalu masuk ke dalam folder Office sesuai dengan versi yang kamu gunakan. (Office10, Office13, Office16, atau Office19)
- Cari dan jalankan `OSPPREARM.EXE` dengan Administrator
- Tekan YES dan tunggu beberapa waktu sampai proses selesai.
