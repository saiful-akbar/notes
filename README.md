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
- Buka file `~/.bashrc` pada text editor lalu tambahkan script berikut agar php dapat dijalankan pada semua directory:
  ```bash
  export PATH=$PATH:/opt/lampp/bin
  ```
- Kembali ke terminal dan jalankan perintah berikut:
  ```bash
  source ~/.bashrc
  ```

## 1.3. Hapus Instalasi

### 1.3.1. menghapus instalasi yang dipasang menggunakan `dpkg`

- Mengetahui Nama Paket:
  ```bash
  dpkg -l | grep example
  ```
- Menghapus Paket aplikasi tanpa menghapus file konfigurasi:
  ```bash
  sudo dpkg --remove nama_paket
  ```
- Menghapus paket aplikasi dan file konfigurasi:
  ```bash
  sudo dpkg --purge nama_paket
  ```
- Memperbarui Database Paket:
  ```bash
  sudo apt-get update
  ```

### 1.3.2. menghapus instalasi yang dipasang menggunakan `apt`

- Cari nama paket:
  ```bash
  apt list --installed | grep nama_aplikasi
  ```
- Hapus aplikasi

  ```bash
  # Hapus hanya aplikasi tanpa menghapus file konfigurasi.
  sudo apt remove nama_paket

  # Hapus aplikasi beserta semua file konfigurasinya.
  sudo apt purge nama_paket
  ```

- Bersihkan paket yang tidak digunakan:
  ```bash
  sudo apt autoremove && sudo apt autoclean
  ```

Jangan lupa menggantikan "nama_paket" dengan nama paket yang sesuai dengan aplikasi yang ingin Anda hapus. Dan selalu berhati-hati saat menghapus paket, pastikan bahwa Anda menghapus paket yang benar-benar tidak dibutuhkan untuk mencegah potensi masalah dengan sistem.

# 2. Windows

## 2.1. Activasi MS Office.

- Buka folder di local disk `C:/`
- Lalu cari folder `Program Files (x86)` atau `Program Files`.
- Buka Program `Files (x86)` untuk Office 32-bit `Program Files` untuk Office 64-bit.
- Cari dan masuk ke folder `Microsoft Office`.
- Lalu masuk ke dalam folder Office sesuai dengan versi yang kamu gunakan. (Office10, Office13, Office16, atau Office19)
- Cari dan jalankan `OSPPREARM.EXE` dengan Administrator
- Tekan YES dan tunggu beberapa waktu sampai proses selesai.

# 3. Laravel

## 3.1. Install Laravel Installer

- Buka terminal `ctrl+alt+t` lalu ketikan perintah berikut:
  ```bash
  composer global require laravel/installser
  ```
- Buka file `~/.bashrc` dan tambahkan script berikut agar installer dapat dijalankan di seluruh directory.
  ```python
  export PATH="~/.config/composer/vendor/bin:$PATH"
  ```
- Kembali ke terminal dan jalan perintah berikut untuk mengetesnya.
  ```bash
  laravel -v
  ```

## 3.2. Masalah izin pada folder Storage laravel pada linux ubuntu.

- Buka terminla `ctrl+alt+t` dan arahkan pada folder project laravel
  ```bash
  sudo chmod -R 777 ./storage
  sudo chmod -R 777 ./storage/logs
  ```
# 4. Struktur Folder Project Aplikasi.

## 4.1. ReactJS Typescript.

```
my-react-app/
├── public/                     # File statis yang diakses langsung dari root (favicon, manifest, dll.)
│   ├── index.html              # Template utama HTML
│   └── assets/                 # File aset seperti gambar atau font
│       ├── images/
│       └── fonts/
├── src/                        # Folder utama untuk kode aplikasi
│   ├── assets/                 # Aset internal seperti gambar dan stylesheet
│   │   ├── images/
│   │   └── styles/
│   │       ├── global.scss     # Gaya global
│   │       └── variables.scss  # Variabel SCSS
│   ├── components/             # Komponen UI yang dapat digunakan ulang
│   │   ├── common/             # Komponen umum seperti button, input
│   │   ├── layout/             # Komponen layout seperti header, footer, sidebar
│   │   └── specific/           # Komponen khusus untuk halaman tertentu
│   ├── features/               # Folder khusus untuk fitur aplikasi (per domain/feature)
│   │   ├── auth/               # Fitur autentikasi (login, register)
│   │   ├── dashboard/          # Fitur dashboard
│   │   └── profile/            # Fitur profil pengguna
│   ├── hooks/                  # Hook React yang dapat digunakan ulang
│   │   ├── useAuth.ts          # Hook untuk autentikasi
│   │   └── useFetch.ts         # Hook untuk pengambilan data
│   ├── layouts/                # Layout utama aplikasi
│   │   ├── AdminLayout.tsx
│   │   └── MainLayout.tsx
│   ├── pages/                  # Halaman utama aplikasi
│   │   ├── Home/               # Halaman Home
│   │   │   ├── HomePage.tsx
│   │   │   └── HomePage.module.scss
│   │   ├── Login/              # Halaman Login
│   │   │   ├── LoginPage.tsx
│   │   │   └── LoginPage.module.scss
│   │   └── Profile/            # Halaman Profile
│   │       ├── ProfilePage.tsx
│   │       └── ProfilePage.module.scss
│   ├── routes/                 # Definisi rute aplikasi
│   │   ├── AppRoutes.tsx       # Konfigurasi rute utama
│   │   └── ProtectedRoute.tsx  # Komponen untuk rute yang membutuhkan autentikasi
│   ├── services/               # API calls atau fungsi untuk komunikasi dengan server
│   │   ├── api.ts              # File utama untuk konfigurasi API
│   │   └── userService.ts      # Contoh service untuk pengguna
│   ├── store/                  # State management (Redux, Zustand, dll.)
│   │   ├── slices/             # Slice Redux (per domain)
│   │   │   ├── authSlice.ts
│   │   │   └── userSlice.ts
│   │   └── store.ts            # Konfigurasi store utama
│   ├── types/                  # Tipe TypeScript untuk aplikasi
│   │   ├── auth.d.ts           # Tipe untuk autentikasi
│   │   └── user.d.ts           # Tipe untuk pengguna
│   ├── utils/                  # Fungsi utilitas yang dapat digunakan ulang
│   │   ├── formatDate.ts       # Format tanggal
│   │   └── validateForm.ts     # Validasi form
│   ├── App.tsx                 # Komponen utama aplikasi
│   ├── index.tsx               # Entry point aplikasi
│   └── react-app-env.d.ts      # Deklarasi global untuk TypeScript
├── tsconfig.json               # Konfigurasi TypeScript
├── package.json                # Konfigurasi dependensi
└── README.md                   # Dokumentasi proyek
```

## Penjelasan

### `public/`
Folder untuk file yang tidak akan diubah oleh Webpack, seperti favicon, manifest.json, dan gambar publik.

### `src/assets/`
Menyimpan file statis seperti gambar, ikon, atau stylesheet khusus aplikasi.

### `src/components/`
Untuk komponen kecil dan dapat digunakan ulang, seperti tombol, formulir, atau komponen layout.

### `src/features/`
Untuk pengelompokan kode yang spesifik pada fitur (domain-driven).

### `src/hooks/`
Tempat menyimpan custom hooks untuk menghindari pengulangan logika.

### `src/layouts/`
Layout utama untuk halaman (Admin, User, dll.).

### `src/pages/`
Menyimpan halaman utama aplikasi, dengan satu folder per halaman.

### `src/routes/`
Untuk konfigurasi rute aplikasi, termasuk rute yang dilindungi.

### `src/services/`
Untuk memisahkan logika API dari komponen.

### `src/store/`
Untuk pengelolaan state global (misalnya, Redux atau Zustand).

### `src/types/`
Deklarasi tipe untuk entitas aplikasi (seperti pengguna, produk, dll.).

### `src/utils/`
Fungsi pembantu yang dapat digunakan di seluruh aplikasi.

## Keuntungan
- **Organisasi yang Jelas**: Setiap fitur atau domain aplikasi memiliki tempat yang jelas.
- **Kemudahan Skalabilitas**: Struktur ini mendukung penambahan fitur atau komponen baru tanpa memengaruhi folder lain.
- **Reusable Components & Hooks**: Komponen dan hook yang umum dapat digunakan di berbagai fitur.
- **Code Splitting**: Halaman dan fitur dipisahkan, memudahkan implementasi **lazy loading**.
