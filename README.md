# Ubuntu

## Perintah dasar terminal

#### Navigasi dan Manajemen Direktori:

- `pwd`: Menampilkan direktori kerja saat ini.
- `ls`: Menampilkan daftar file dan direktori di direktori saat ini.
- `cd`: Mengganti direktori kerja.
  - Contoh: `cd /path/ke/direktori`

#### Manipulasi File dan Direktori:

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

#### Perintah Pencarian:

- `find`: Mencari file atau direktori.
  - Contoh: `find /path -name nama_file`

#### Perintah Informasi Sistem:

- `uname`: Menampilkan informasi kernel sistem.
  - Contoh: `uname -a`
- `lsb_release`: Menampilkan informasi distribusi.
  - Contoh: `lsb_release -a`

#### Manajemen Proses:

- `ps`: Menampilkan daftar proses yang berjalan.
  - Contoh: `ps aux`
- `kill`: Menghentikan proses.
  - Contoh: `kill PID` (PID adalah ID proses)

#### Paket dan Manajemen Aplikasi:

- `apt-get` (atau `apt`): Manajemen paket Debian.
  - Contoh: `sudo apt-get install nama_paket`
- `dpkg`: Manajemen paket yang terinstal.
  - Contoh: `dpkg -l`

#### Perintah Izin File:

- `chmod`: Mengubah izin file/direktori.
  - Contoh: `chmod permissions nama_file`

#### Perintah Pencarian Teks:

- `grep`: Mencari teks dalam file.
  - Contoh: `grep kata_kunci nama_file`

#### Perintah Kompresi/Decompression:

- `tar`: Mengompresi/dekompresi file/direktori.
  - Contoh: `tar -czvf arsip.tar.gz direktori`

#### Networking:

- `ifconfig`: Menampilkan informasi antarmuka jaringan.
- `ping`: Mengirim paket ke host jaringan.
- `ssh`: Menghubungkan ke mesin jarak jauh dengan SSH.
- `netstat`: Menampilkan informasi koneksi jaringan.

