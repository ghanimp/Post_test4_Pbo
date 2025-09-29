## Ghani Mandala Putra
## 2409116042
----
## Deskripsi Program

Program ini adalah aplikasi berbasis Java Console yang dirancang untuk mengelola data pemain sepak bola yang berlaga di Liga Inggris. Program ini dibangun menggunakan konsep OOP (Object-Oriented Programming) dengan struktur yang rapi, sehingga mampu memisahkan pemain senior dan pemain akademi.

## Struktur Program

1. Class Post_test1 (Main)

Menyediakan menu utama berbasis teks:
- Tambah Pemain
- Lihat Daftar Pemain
- Update Pemain
- Hapus Pemain
- Cari Pemain
- Keluar

2. Package model

- Pemain (Super Class)

Berisi data dasar pemain Liga Inggris: nama, klub, posisi, nomor punggung, usia.

- PemainAkademi (Subclass)

Berisi tambahan data akademi & tahun masuk bagi pemain muda yang terdaftar di akademi klub Liga Inggris.

- PemainSenior (Subclass)

Berisi tambahan data pengalaman atau penghargaan yang dimiliki pemain senior di Liga Inggris.

- PemainBase (Abstract class)

PemainBase ini menyimpan properti dasar nama dan klub yang dipakai oleh semua turunan, supaya kamu tidak copy-paste field itu ke setiap class.

- Performa (Interface)

Performa berfungsi sebagai kontrak yang mewajibkan setiap class yang mengimplementasikannya punya method tampilkanPerforma().

3. Package service

PemainService Menangani semua proses CRUD:

- Tambah Pemain Senior atau Pemain Akademi
- Lihat Daftar Pemain berdasarkan tipe (Semua, Senior saja, Akademi saja)
- Update Data Pemain
- Hapus Pemain
- Cari Pemain berdasarkan nama
----
## Penjelasan kode yang saya tambahkan

<img width="391" height="328" alt="image" src="https://github.com/user-attachments/assets/2a031fc0-c5ba-44cb-a209-ab203f75ee13" />

