# Web responsive
Tugas m3 dan m4

# Informasi Mahasiswa
Nama  : Akbar Zulfikar R
Nim   : 5190411163
Kelas : D

# Implementasi

# Route


# Authetication 
Login, verification, dan logout diatur oleh controller 

# Template Inheritance
Membuat master layout yang berisi komponen-komponen yang digunakan berulang-ulang dan komponen yang bisa di inject. Adapun komponen yang bisa digunakan berulang-ulang yaitu:

Header
Sidebar
Sedangkan komponen yang bisa di inject yaitu:

Title
Content

Penggunaan Layout Pada Halaman Home :

Penggunaan master layout pada halaman mahasiswa :


# Dosen

Membuat Model Dosen beserta dengan Controller, Migration, dan Factory.
php artisan make:model Dosen -mcf
Migration pada model Dosen. Menentukan schema database termasuk nama kolom dan tipe data.

Model Dosen. Menentukan field yang boleh di isi.

DosenFactory. Mendefinisikan nilai-nilai yang harus diterapkan pada saat memasukkan data ke dalam model Dosen. Pengisian data dilakukan dengan menggunakan libary Faker. Faker digunakan untuk menciptakan data bohongan. Dalam konteks ini, data yang di ciptakan Faker adalah:

NIK
Nama
Jenis kelamin (Male / Female)
Dan Jabatan Strukturan

Seeding Dosen. Mengisikan 100 data Dosen ke dalam database.

DosenController. mengembalikan view beserta data dosen yang telah di Paginate sebanyak 10.

View Dosen:


# Pengujian

# Uji Authetication

# Uji Halaman

# Hasil Pengujian







