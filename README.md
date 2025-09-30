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

Ini merupakan tampilan package terbaru saya
- Main (Post_test1) sebagai class yang menjalankan program.
- Model (Pemain) berisi model pemain, sub class pemain, abstract class, dan interface.
- Service (PemainService) berisi sistem CRUD.


<img width="453" height="175" alt="image" src="https://github.com/user-attachments/assets/39f5551d-d72f-4e92-b7de-094b58111126" />


- Interface Performa digunakan sebagai kontrak yang mewajibkan setiap class pemain memiliki metode tampilkanPerforma() dan tampilkanInfo(). Melalui interface ini program dapat memanfaatkan konsep abstraction dan polymorphism, di mana setiap class pemain memiliki implementasi berbeda walaupun metode yang dipanggil sama.


<img width="667" height="269" alt="image" src="https://github.com/user-attachments/assets/f5be1492-53b4-49fd-af15-0ae34d878f28" />


- Abstract class PemainBase berperan sebagai kerangka dasar bagi seluruh jenis pemain. Class ini menyimpan atribut umum seperti nama dan klub serta menyediakan method abstrak infoPosisi() yang harus diimplementasikan oleh setiap subclass. Dengan penerapan ini, program memanfaatkan konsep abstraction agar atribut dan perilaku dasar tersentralisasi dan lebih mudah dikelola.


<img width="1021" height="411" alt="image" src="https://github.com/user-attachments/assets/2d244983-49f5-42bd-ab09-2370e913ff48" />


- Kode ini terlihat penerapan polymorphism melalui overriding. Method tampilkanPerforma(), tampilkanInfo(), dan toString() di-override dari interface atau superclassnya untuk menyesuaikan perilaku khusus pemain senior. Hal ini memungkinkan setiap class turunan memiliki cara sendiri dalam menampilkan data, meskipun dipanggil dengan nama method yang sama.


<img width="1319" height="272" alt="image" src="https://github.com/user-attachments/assets/1deefd3c-656f-45bf-a0e9-d9b2b9ab41bc" />


- Kode ini terlihat penerapan polymorphism melalui overriding. Method tampilkanPerforma() dan toString() diimplementasikan ulang secara khusus di class pemain akademi untuk menampilkan informasi akademi dan tahun masuk. Hal ini memungkinkan setiap class turunan menampilkan data yang berbeda meskipun dipanggil dengan nama method yang sama.






























