# Materi Kuliah Basis Data1

## Pengenalan Basis Data

### Definisi Basis Data
Basis data adalah kumpulan informasi yang terorganisir dengan baik yang dapat diakses, dimanipulasi, dan dikelola dengan menggunakan perangkat lunak tertentu.

### Komponen Utama Basis Data
1. **Data:** Fakta-fakta yang direkam dan disimpan dalam basis data.
2. **Perangkat Lunak Manajemen Basis Data (DBMS):** Program yang digunakan untuk mengelola dan mengakses basis data.
3. **Pengguna:** Orang-orang atau aplikasi yang berinteraksi dengan basis data.

## Model Data Relasional

### Pengertian
Model data relasional adalah pendekatan untuk mengorganisir data dalam basis data dengan menggunakan tabel yang terdiri dari baris dan kolom.

### Konsep Penting
1. **Tabel:** Kumpulan entitas yang terdiri dari baris dan kolom.
2. **Kunci Primer (Primary Key):** Kolom atau kombinasi kolom yang secara unik mengidentifikasi setiap baris dalam sebuah tabel.
3. **Kunci Asing (Foreign Key):** Kolom yang menghubungkan dua tabel dengan merujuk pada kunci primer dari tabel lain.
4. **Hubungan (Relationships):** Keterkaitan antara data dalam tabel-tabel yang berbeda.

## Bahasa Permintaan Struktur (SQL)

### Pengertian
SQL (Structured Query Language) adalah bahasa standar yang digunakan untuk mengakses dan mengelola basis data relasional.

### Perintah Dasar SQL
1. **SELECT:** Digunakan untuk menampilkan data dari satu atau lebih tabel.
   ```sql
   SELECT kolom1, kolom2 FROM tabel;
