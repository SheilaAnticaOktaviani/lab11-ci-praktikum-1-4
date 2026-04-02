# lab11-ci-praktikum-1-4
## Nama : SHEILA ANTICA OKTAVIANI
## Kelas : I241A
## NIM : 312410002
## Dosen MK : Agung Nugroho, S.Kom., M.Kom., S.Kom., M. Kom


## Halaman Login (/user/login)
Halaman ini digunakan untuk autentikasi pengguna sebelum masuk ke halaman admin.
1. Fitur:
2. Input:
3. Email address
4. Password
5. Tombol:
6. Login
7. Validasi login:
8. Mengecek email dan password yang dimasukkan
Tujuan: Mengamankan akses ke halaman admin agar hanya user tertentu yang bisa menambah artikel.
## Halaman Home / Artikel (/artikel)
Halaman ini merupakan halaman utama yang menampilkan daftar artikel yang tersedia.
Fitur:
1. Menampilkan list artikel (contoh: Artikel pertama, Artikel kedua)
#### Setiap artikel memiliki:
- Judul
- Gambar (thumbnail)
- Cuplikan isi artikel
### Navigasi menu:
- Home
- Artikel
- About
- Kontak
- Sidebar (Widget):
- Widget Link
- Widget Text
Tujuan: Memberikan tampilan kepada user untuk membaca daftar artikel yang telah dibuat.
## Halaman Tambah Artikel (/admin/artikel/add)
Halaman ini digunakan oleh admin untuk menambahkan artikel baru ke dalam sistem.
### Fitur:
Form input:
1. Judul → untuk memasukkan judul artikel
2. Isi artikel → untuk memasukkan konten artikel
#### Tombol:
1. Kirim → untuk menyimpan artikel ke database
### Navigasi admin:
1. Dashboard
2. Artikel
3. Tambah Artikel
Tujuan: Memudahkan admin dalam mengelola dan menambahkan konten artikel.
## Struktur Umum Aplikasi
### Aplikasi ini terdiri dari:
- Frontend: Tampilan halaman menggunakan HTML & CSS
- Backend: Mengelola data artikel dan autentikasi user
### Routing:
/artikel → halaman publik
/admin/artikel/add → halaman admin tambah artikel
/user/login → halaman login

## Halaman User Login
<img width="959" height="473" alt="user login" src="https://github.com/user-attachments/assets/9ac3f602-793d-4d8e-a042-b570e7f3d909" />

### Email address : admin@gmail.com
### password      : admin123

## Halaman Tambah Artikel
<img width="958" height="473" alt="Tambahkan artikel" src="https://github.com/user-attachments/assets/6c89053e-ff09-4351-980a-c11aa2b447b9" />

## Halaman Home ( Layanan sederhana)
<img width="955" height="476" alt="Home" src="https://github.com/user-attachments/assets/d630e5b9-59b9-4594-a225-8d3d230b2547" />

## 1. Halaman Admin – Daftar Artikel
<img width="956" height="472" alt="artikel" src="https://github.com/user-attachments/assets/ba5e0f5d-a731-4932-80ed-e5332f06cff8" />

Halaman ini merupakan dashboard admin untuk mengelola artikel pada sistem.
### Fitur utama:
Navigasi Menu
### Dashboard: menuju halaman utama admin
### Artikel: menampilkan daftar artikel
### Tambah Artikel: untuk menambahkan artikel baru
## Tabel Daftar Artikel
ID: nomor unik artikel
Judul: judul dan ringkasan isi artikel
Status: status publikasi (misalnya 0 = belum publish)
## Aksi:
Ubah: mengedit artikel
Hapus: menghapus artikel
### Halaman ini berfungsi sebagai pusat kontrol CRUD (Create, Read, Update, Delete) artikel.

## Halaman Error 404 (Admin)
(Gambar: Error 404)
<img width="959" height="476" alt="dashboard" src="https://github.com/user-attachments/assets/0b1a4b95-a164-4db3-8a52-6ee90a3060ac" />

Halaman ini menampilkan error ketika sistem tidak menemukan controller atau method yang dipanggil.
## Penjelasan:
### Error:
Controller or its method is not found: \App\Controllers\Home::getAdmin
### Artinya:
Route menuju /admin tidak terhubung dengan method yang benar
Method getAdmin belum dibuat atau salah penulisan
### Hal ini biasanya terjadi karena:
1. Salah routing
2. Method controller belum dibuat
3. Penamaan function tidak sesuai

## 3. Halaman About (User)
(Gambar: Halaman About)
<img width="949" height="473" alt="Halaman about" src="https://github.com/user-attachments/assets/46948426-a19f-4459-bdf8-8e8b991fd952" />

Halaman ini merupakan bagian dari frontend website yang menampilkan informasi tentang website.
### Struktur halaman:
- Navbar
- Home
- Artikel
- About
- Kontak
- Konten Utama
Judul: Halaman About
Deskripsi: penjelasan singkat isi website
Sidebar (Widget)
Widget Link (navigasi tambahan)
Widget Text (informasi tambahan)
### Digunakan untuk memberikan informasi kepada pengguna tentang tujuan website.

## 4. Halaman Contact
(Gambar: Halaman Contact)
<img width="955" height="472" alt="Halaman Kontak" src="https://github.com/user-attachments/assets/3cd86495-94ae-4d12-aaef-a26ca6aced2a" />

Halaman ini merupakan halaman sederhana yang menampilkan informasi kontak.
Isi:
Teks: "Ini halaman Contact"
### Fungsi:
Sebagai halaman informasi kontak
### Bisa dikembangkan menjadi:
Form kontak
Email form
Integrasi WhatsApp
## Kesimpulan
Project ini terdiri dari dua bagian utama:
Frontend (User) → halaman Home, Artikel, About, Contact
Backend (Admin) → pengelolaan artikel (CRUD)
Selain itu, terdapat:
Sistem routing yang menghubungkan halaman
Penanganan error (404) untuk debugging
