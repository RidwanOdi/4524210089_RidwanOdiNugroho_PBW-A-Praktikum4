# 📘 LAPORAN PRAKTIKUM PERTEMUAN KE-4

**Mata Kuliah:** Pemrograman Berbasis Web (PBW)  
**Nama:** Ridwan Odi Nugroho  
**NPM:** 4524210089  
**Program Studi:** Teknik Informatika  
**Universitas:** Universitas Pancasila

# 💻 LaraPress — Website Manajemen Postingan

LaraPress merupakan aplikasi website berbasis Laravel yang dikembangkan untuk mempelajari pembuatan website dinamis menggunakan framework Laravel. Aplikasi ini berfokus pada pengelolaan akun pengguna, autentikasi, dashboard, manajemen profil, serta pengelolaan postingan menggunakan konsep CRUD (*Create, Read, Update, Delete*).

Dengan adanya aplikasi ini, pengguna dapat melakukan registrasi akun, login, mengakses dashboard, mengelola informasi profil, serta membuat, melihat, mengubah, dan menghapus postingan sesuai dengan hak akses yang tersedia.

Proyek ini juga menjadi sarana pembelajaran mengenai routing, controller, model, view, middleware, template Blade, dan integrasi basis data dalam pengembangan aplikasi web.

---

## 📋 Daftar Isi

- [Tentang Aplikasi](#-tentang-aplikasi)
- [Tujuan Praktikum](#-tujuan-praktikum)
- [Fitur Utama](#-fitur-utama)
- [Teknologi yang Digunakan](#-teknologi-yang-digunakan)
- [Konsep yang Dipelajari](#-konsep-yang-dipelajari)
- [Alur Kerja Aplikasi](#-alur-kerja-aplikasi)
- [Struktur Proyek](#-struktur-proyek)
- [Persyaratan Sistem](#-persyaratan-sistem)
- [Instalasi dan Konfigurasi](#-instalasi-dan-konfigurasi)
- [Panduan Penggunaan](#-panduan-penggunaan)
- [Pengujian Aplikasi](#-pengujian-aplikasi)
- [Penanganan Masalah](#-penanganan-masalah)
- [Pengembangan Selanjutnya](#-pengembangan-selanjutnya)
- [Kesimpulan](#-kesimpulan)

---

## 🎯 Tentang Aplikasi

LaraPress adalah aplikasi berbasis web yang menerapkan konsep pengembangan aplikasi dinamis menggunakan Laravel. Aplikasi ini dirancang untuk memberikan pengalaman dalam mengelola data melalui halaman website yang terhubung dengan proses backend.

Berbeda dengan website statis yang hanya menampilkan informasi, LaraPress menerapkan interaksi antara pengguna, sistem autentikasi, proses pengolahan data, dan basis data.

### Informasi Proyek

| Keterangan | Detail |
|---|---|
| Nama aplikasi | LaraPress |
| Jenis aplikasi | Website Manajemen Postingan |
| Mata kuliah | Pemrograman Berbasis Web |
| Pertemuan | Praktikum 4 |
| Framework | Laravel |
| Bahasa backend | PHP |
| Template | Blade |
| Basis data | MySQL, sesuai konfigurasi proyek |

## 🎓 Tujuan Praktikum

Praktikum ini bertujuan untuk:

1. Memahami penggunaan framework Laravel dalam pengembangan aplikasi web.
2. Memahami konsep routing untuk mengatur alamat halaman website.
3. Menerapkan controller untuk mengolah permintaan pengguna.
4. Memahami penggunaan model untuk berinteraksi dengan basis data.
5. Menggunakan Blade Template untuk menampilkan halaman web.
6. Menerapkan autentikasi pengguna melalui registrasi dan login.
7. Memahami konsep middleware untuk membatasi akses halaman.
8. Mengimplementasikan operasi CRUD pada data postingan.
9. Memahami konfigurasi koneksi basis data MySQL.
10. Melakukan pengujian untuk memastikan fungsi aplikasi berjalan sesuai kebutuhan.

## ✨ Fitur Utama

### 1. 🏠 Halaman Home

Halaman awal yang menjadi pintu masuk pengguna ke website LaraPress. Halaman ini berfungsi sebagai tempat untuk menampilkan informasi awal dan menyediakan navigasi menuju halaman lain.

### 2. 🔐 Registrasi dan Login

Fitur autentikasi digunakan untuk mengelola akses pengguna ke dalam aplikasi.

- **Register:** Membuat akun pengguna baru.
- **Login:** Memasuki aplikasi menggunakan akun yang terdaftar.
- **Logout:** Mengakhiri sesi penggunaan aplikasi.

### 3. 📊 Dashboard

Dashboard merupakan halaman yang dapat diakses setelah pengguna berhasil melewati proses autentikasi dan memenuhi persyaratan akses yang diterapkan aplikasi.

Halaman ini menjadi pusat navigasi untuk mengakses fitur yang tersedia bagi pengguna.

### 4. 📝 Manajemen Postingan

Fitur manajemen postingan menerapkan konsep CRUD:

| Operasi | Fungsi |
|---|---|
| Create | Membuat postingan baru |
| Read | Melihat atau menampilkan data postingan |
| Update | Mengubah postingan yang sudah ada |
| Delete | Menghapus postingan |

Melalui fitur ini, pengguna dapat mempelajari bagaimana data dikelola melalui formulir, diproses oleh aplikasi, dan disimpan ke basis data.

### 5. 👤 Manajemen Profil

Fitur profil digunakan untuk mengelola informasi akun pengguna. Bergantung pada implementasi proyek, fitur ini dapat mencakup pembaruan informasi profil, perubahan kata sandi, dan pengelolaan akun.

### 6. 🛡️ Middleware Autentikasi

Middleware digunakan untuk mengatur akses terhadap halaman tertentu. Halaman yang membutuhkan autentikasi tidak seharusnya dapat diakses secara langsung oleh pengguna yang belum memenuhi persyaratan login.

### 7. 🗄️ Integrasi Basis Data

Aplikasi menggunakan konfigurasi basis data untuk mendukung penyimpanan informasi pengguna dan data aplikasi. Pada referensi proyek, basis data yang digunakan adalah MySQL melalui lingkungan lokal XAMPP.

**Catatan:** Fitur yang dijelaskan di atas mengikuti dokumentasi repository referensi. Pastikan implementasinya tersedia pada kode proyekmu sebelum mencantumkannya sebagai fitur yang sudah selesai.

## 🛠️ Teknologi yang Digunakan

### Backend

- **PHP 8.2+:** Bahasa pemrograman untuk menjalankan proses backend.
- **Laravel 12:** Framework PHP untuk membangun aplikasi web.
- **Eloquent ORM:** Fasilitas Laravel untuk berinteraksi dengan basis data menggunakan model.
- **Laravel Routing:** Mengatur URL dan mengarahkan permintaan ke proses yang sesuai.
- **Middleware:** Mengatur akses terhadap halaman dan proses tertentu.

### Frontend

- **Blade Template:** Template engine Laravel untuk menampilkan halaman dinamis.
- **HTML5:** Menyusun struktur halaman website.
- **CSS:** Mengatur tampilan dan tata letak halaman.
- **Tailwind CSS:** Framework CSS apabila digunakan dalam konfigurasi proyek.
- **JavaScript:** Mendukung interaksi pada sisi frontend apabila diperlukan.

### Basis Data

- **MySQL:** Sistem manajemen basis data relasional.
- **XAMPP:** Lingkungan server lokal yang menyediakan layanan Apache dan MySQL/MariaDB.
- **phpMyAdmin:** Antarmuka untuk mengelola basis data melalui browser.

### Development Tools

- **Composer:** Mengelola dependensi PHP.
- **Node.js dan npm:** Mengelola dependensi dan proses build frontend.
- **PHP Artisan:** Menjalankan perintah pengembangan Laravel.
- **Git dan GitHub:** Mengelola versi kode serta menyimpan proyek secara daring.

## 📚 Konsep yang Dipelajari

### 1. Routing

Routing menentukan bagaimana aplikasi merespons permintaan berdasarkan URL dan metode HTTP.

Contoh sederhana:

```php
use Illuminate\Support\Facades\Route;

Route::get('/', function () {
    return view('welcome');
});
```

Kode tersebut mengatur agar permintaan GET ke halaman utama menampilkan view `welcome`.

### 2. Model

Model digunakan sebagai representasi data dan penghubung antara aplikasi dengan basis data melalui Eloquent ORM.

Model membantu proses pengambilan, penambahan, pembaruan, dan penghapusan data tanpa harus menulis seluruh query SQL secara manual.

### 3. View dan Blade Template

View bertanggung jawab menampilkan informasi kepada pengguna. Blade memungkinkan aplikasi menggabungkan struktur HTML dengan data yang dikirim dari controller.

Contoh:

```blade
<h1>Selamat Datang di LaraPress</h1>
<p>Website Manajemen Postingan</p>
```

### 4. Controller

Controller menangani proses yang berkaitan dengan permintaan pengguna. Controller dapat memvalidasi input, memanggil model, dan mengembalikan view atau respons lainnya.

### 5. Autentikasi dan Middleware

Autentikasi digunakan untuk memverifikasi identitas pengguna, sedangkan middleware dapat membatasi akses berdasarkan status autentikasi atau ketentuan lainnya.

### 6. CRUD

CRUD merupakan operasi dasar pengelolaan data:

- **Create:** Menambahkan data.
- **Read:** Membaca data.
- **Update:** Memperbarui data.
- **Delete:** Menghapus data.

Penerapan CRUD merupakan bagian penting dalam pengembangan aplikasi berbasis basis data.

## 🔄 Alur Kerja Aplikasi

Secara umum, alur aplikasi dapat digambarkan sebagai berikut:

```text
Pengguna
   |
   v
Membuka Website
   |
   v
Halaman Home
   |
   v
Registrasi / Login
   |
   v
Pemeriksaan Autentikasi
   |
   v
Dashboard
   |
   +----------------------+
   |                      |
   v                      v
Manajemen Postingan   Manajemen Profil
   |
   v
Create / Read / Update / Delete
   |
   v
Pemrosesan oleh Aplikasi
   |
   v
Basis Data
   |
   v
Hasil Ditampilkan kepada Pengguna
```

Alur tersebut merupakan gambaran konseptual. Alur aktual bergantung pada rute, controller, middleware, dan konfigurasi autentikasi yang terdapat dalam kode proyek.

## 📂 Struktur Proyek

Laravel memiliki struktur direktori yang memisahkan proses backend, konfigurasi, tampilan, dan basis data.

Berikut contoh struktur umum yang perlu disesuaikan dengan berkas proyek yang sebenarnya:

```text
LaraPress/
├── app/
│   ├── Http/
│   │   ├── Controllers/
│   │   │   ├── Auth/
│   │   │   ├── PostController.php
│   │   │   └── ProfileController.php
│   │   └── Requests/
│   └── Models/
│       └── User.php
├── bootstrap/
├── config/
│   └── database.php
├── database/
│   ├── migrations/
│   ├── factories/
│   └── seeders/
├── resources/
│   ├── css/
│   ├── js/
│   └── views/
│       ├── auth/
│       ├── components/
│       ├── layouts/
│       ├── profile/
│       ├── dashboard.blade.php
│       └── welcome.blade.php
├── routes/
│   ├── web.php
│   └── auth.php
├── tests/
├── .env.example
├── artisan
├── composer.json
└── package.json
```

### Penjelasan Direktori

| Direktori atau berkas | Kegunaan |
|---|---|
| `app/Http/Controllers/` | Menangani permintaan dan proses aplikasi |
| `app/Models/` | Menyimpan model untuk merepresentasikan data |
| `app/Http/Requests/` | Menangani validasi permintaan jika digunakan |
| `resources/views/` | Menyimpan tampilan halaman menggunakan Blade |
| `routes/web.php` | Mendefinisikan rute website |
| `routes/auth.php` | Mendefinisikan rute autentikasi jika tersedia |
| `database/migrations/` | Mendefinisikan perubahan struktur tabel |
| `database/seeders/` | Menyediakan data awal jika digunakan |
| `config/database.php` | Menyimpan konfigurasi koneksi basis data |
| `.env` | Menyimpan konfigurasi lingkungan lokal |
| `composer.json` | Mendefinisikan dependensi PHP |
| `package.json` | Mendefinisikan dependensi frontend |

Nama controller dan struktur direktori di atas adalah contoh berdasarkan pola proyek referensi. Hapus atau ubah entri yang tidak ditemukan pada proyekmu.

## 💻 Persyaratan Sistem

Untuk menjalankan proyek Laravel secara lokal, siapkan:

- PHP versi 8.2 atau lebih baru untuk Laravel 12.
- Composer.
- Node.js dan npm jika proyek menggunakan proses build frontend.
- MySQL atau MariaDB jika aplikasi dikonfigurasi menggunakan basis data tersebut.
- XAMPP apabila digunakan sebagai server lokal.
- Git untuk mengunduh kode dari GitHub.
- Browser modern untuk mengakses aplikasi.

## 🚀 Instalasi dan Konfigurasi

### 1. Clone Repository

Unduh repository milikmu sendiri:

```bash
git clone URL_REPOSITORY_MILIKMU
```

Masuk ke direktori proyek:

```bash
cd NAMA_FOLDER_PROYEK
```

Ganti URL dan nama folder dengan nilai yang sesuai. Jangan menggunakan URL repository referensi apabila kamu ingin menjalankan proyek milikmu sendiri.

### 2. Instal Dependensi PHP

Jalankan:

```bash
composer install
```

Perintah ini memasang dependensi PHP yang didefinisikan pada `composer.json`.

### 3. Instal Dependensi Frontend

Jika proyek menggunakan npm, jalankan:

```bash
npm install
```

### 4. Konfigurasi Environment

Pada Windows Command Prompt atau PowerShell, salin berkas konfigurasi contoh:

```powershell
Copy-Item .env.example .env
```

Jika berkas `.env` sudah tersedia dan berisi konfigurasi yang ingin dipertahankan, jangan menimpanya secara sembarangan.

Kemudian buat application key:

```bash
php artisan key:generate
```

### 5. Konfigurasi Database

Jika aplikasi menggunakan MySQL:

1. Buka XAMPP Control Panel.
2. Jalankan layanan MySQL.
3. Buka `http://localhost/phpmyadmin`.
4. Buat database dengan nama yang sesuai dengan konfigurasi proyek.
5. Buka file `.env`.
6. Sesuaikan pengaturan koneksi database.

Contoh konfigurasi lokal:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=larapress
DB_USERNAME=root
DB_PASSWORD=
```

Nama database, username, dan password harus disesuaikan dengan pengaturan pada perangkatmu. Contoh di atas menggunakan konfigurasi umum XAMPP, bukan ketentuan wajib.

### 6. Jalankan Migrasi

Jika proyek memiliki migration dan koneksi database sudah benar, jalankan:

```bash
php artisan migrate
```

Laravel akan menjalankan migration yang tersedia untuk membuat atau memperbarui struktur tabel database.

**Peringatan:** Jangan menjalankan perintah yang menghapus atau mereset tabel pada database berisi data penting tanpa membuat cadangan terlebih dahulu.

### 7. Jalankan Frontend

Untuk menjalankan frontend selama proses pengembangan:

```bash
npm run dev
```

Untuk membuat hasil build frontend:

```bash
npm run build
```

Gunakan perintah yang sesuai dengan skrip yang tersedia pada `package.json`.

### 8. Jalankan Aplikasi Laravel

Buka terminal pada direktori proyek dan jalankan:

```bash
php artisan serve
```

Kemudian buka alamat berikut melalui browser:

```text
http://127.0.0.1:8000
```

Jika aplikasi membutuhkan Vite selama pengembangan, biarkan `npm run dev` berjalan di terminal terpisah.

## 🧭 Panduan Penggunaan

Berikut urutan penggunaan aplikasi berdasarkan fitur yang dijelaskan pada repository referensi:

1. Buka halaman utama LaraPress melalui browser.
2. Pilih menu registrasi jika belum memiliki akun.
3. Masukkan informasi yang diminta pada formulir registrasi.
4. Login menggunakan akun yang sudah terdaftar.
5. Akses dashboard apabila persyaratan autentikasi sudah terpenuhi.
6. Buka fitur manajemen postingan.
7. Coba membuat postingan baru.
8. Lihat postingan yang telah tersedia.
9. Ubah postingan untuk menguji operasi update.
10. Hapus postingan uji untuk menguji operasi delete.
11. Buka menu profil dan periksa fitur pengelolaan akun.
12. Logout setelah selesai menggunakan aplikasi.

Langkah-langkah tersebut perlu disesuaikan apabila nama menu atau proses autentikasi pada implementasi proyek berbeda.

## 🧪 Pengujian Aplikasi

Pengujian dilakukan untuk memeriksa apakah fungsi aplikasi bekerja sesuai kebutuhan.

Jika proyek menyediakan konfigurasi pengujian Laravel, jalankan:

```bash
php artisan test
```

Perintah tersebut menjalankan pengujian otomatis yang tersedia dalam proyek. Hasil pengujian perlu diperiksa untuk mengetahui apakah terdapat pengujian yang gagal.

### Skenario Pengujian Manual

| No. | Skenario | Hasil yang Diharapkan |
|---|---|---|
| 1 | Membuka halaman Home | Halaman awal dapat ditampilkan |
| 2 | Registrasi akun baru | Akun dapat dibuat jika input valid |
| 3 | Login dengan akun terdaftar | Pengguna dapat masuk sesuai ketentuan |
| 4 | Login dengan data yang salah | Sistem menolak autentikasi yang tidak valid |
| 5 | Membuka dashboard | Akses mengikuti aturan autentikasi |
| 6 | Membuat postingan | Data baru dapat disimpan |
| 7 | Melihat daftar postingan | Data yang tersedia dapat ditampilkan |
| 8 | Mengubah postingan | Perubahan tersimpan sesuai ketentuan |
| 9 | Menghapus postingan | Data yang dipilih terhapus sesuai ketentuan |
| 10 | Membuka fitur profil | Halaman profil dapat diakses sesuai hak pengguna |
| 11 | Logout | Sesi pengguna diakhiri |
| 12 | Mengakses halaman terlindungi tanpa login | Akses ditolak atau dialihkan sesuai konfigurasi |

Tabel ini merupakan rencana pengujian. Tandai suatu skenario sebagai berhasil hanya setelah benar-benar menjalankan dan memeriksanya.

## 🛠️ Penanganan Masalah

### 1. Composer tidak ditemukan

Pastikan Composer sudah terinstal dan dapat dipanggil melalui terminal.

Periksa dengan:

```bash
composer --version
```

### 2. PHP tidak ditemukan

Pastikan PHP sudah terinstal dan direktori PHP sudah terdaftar pada environment variable `PATH`.

Periksa dengan:

```bash
php --version
```

### 3. Database tidak dapat terhubung

Periksa beberapa hal berikut:

- Layanan MySQL di XAMPP sudah berjalan.
- Nama database pada `.env` benar.
- Username dan password sesuai dengan konfigurasi MySQL.
- Port database sesuai dengan pengaturan perangkat.
- Konfigurasi Laravel sudah diperbarui jika sebelumnya berubah.

Setelah memperbaiki konfigurasi, jalankan:

```bash
php artisan config:clear
```

### 4. Tabel database belum tersedia

Jika tabel belum dibuat, periksa koneksi database dan migration yang tersedia. Kemudian jalankan:

```bash
php artisan migrate
```

### 5. Tampilan frontend tidak muncul dengan benar

Jika proyek menggunakan Vite, pastikan dependensi frontend sudah terpasang dan jalankan:

```bash
npm install
npm run dev
```

Jika ingin menghasilkan aset untuk penggunaan produksi, jalankan:

```bash
npm run build
```

### 6. Halaman dashboard tidak dapat dibuka

Periksa apakah pengguna sudah login dan memenuhi persyaratan autentikasi yang diterapkan. Jika proyek menggunakan verifikasi email atau middleware tambahan, pastikan persyaratan tersebut telah dipenuhi.

## 🚀 Pengembangan Selanjutnya

Beberapa ide pengembangan yang dapat dipertimbangkan untuk meningkatkan aplikasi:

1. **Pencarian postingan** — Memudahkan pengguna menemukan postingan berdasarkan judul atau kata kunci.
2. **Kategori postingan** — Mengelompokkan postingan berdasarkan kategori tertentu.
3. **Pagination** — Membagi daftar postingan menjadi beberapa halaman agar lebih mudah dibaca.
4. **Validasi formulir** — Memastikan data yang dimasukkan sesuai dengan ketentuan.
5. **Pengelolaan gambar** — Menambahkan fitur unggah gambar untuk melengkapi postingan.
6. **Pengaturan hak akses** — Memisahkan hak pengguna biasa dan administrator jika diperlukan.
7. **Peningkatan tampilan responsif** — Memastikan antarmuka nyaman digunakan pada perangkat desktop maupun ponsel.
8. **Pengujian otomatis tambahan** — Menambahkan pengujian untuk operasi CRUD, autentikasi, dan validasi.
9. **Peningkatan keamanan** — Memeriksa validasi input, pembatasan akses, dan perlindungan terhadap tindakan yang tidak diizinkan.
10. **Deployment** — Menyiapkan aplikasi untuk dijalankan pada server agar dapat diakses secara daring.

Daftar ini merupakan rencana pengembangan, bukan daftar fitur yang sudah tersedia.

## 📄 Kesimpulan

Praktikum 4 memberikan kesempatan untuk mempelajari pengembangan aplikasi web dinamis menggunakan framework Laravel. Melalui proyek LaraPress, konsep routing, controller, model, view, autentikasi, middleware, operasi CRUD, dan konfigurasi basis data dapat dipahami melalui penerapan pada sebuah website.

Pengelolaan postingan menjadi contoh penerapan operasi CRUD, sedangkan sistem autentikasi menunjukkan bagaimana akses pengguna dapat diatur. Pemisahan komponen aplikasi juga membantu membuat kode lebih terstruktur dan memudahkan pengembangan selanjutnya.

Dengan memahami konsep-konsep tersebut, diharapkan mahasiswa dapat mengembangkan aplikasi web yang lebih terorganisasi, mudah dipelihara, dan sesuai dengan kebutuhan pengguna.

---

**Dibuat oleh:** Ridwan Odi Nugroho  
**NPM:** 4524210089  
**Program Studi:** Teknik Informatika — Universitas Pancasila  
**Mata Kuliah:** Pemrograman Berbasis Web (PBW)  
**Praktikum:** Pertemuan 4

*Dibuat untuk dokumentasi pembelajaran pengembangan web menggunakan Laravel.*
