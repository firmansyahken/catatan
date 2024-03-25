# Algoritma dan Pemrograman Dasar Python

## Pengenalan Python
- Python adalah bahasa pemrograman tingkat tinggi yang mudah dipelajari dan kuat.
- Dikembangkan oleh Guido van Rossum pada tahun 1991.
- Cocok untuk pemula dan digunakan dalam berbagai bidang, termasuk pengembangan web, analisis data, dan kecerdasan buatan.

## Instalasi Python
- Buka [python.org](https://www.python.org/), unduh installer sesuai dengan sistem operasi yang digunakan, dan ikuti petunjuk instalasinya.
- Pastikan untuk menambahkan Python ke PATH saat instalasi.

## Hello World
```python
print("Hello, World!")
```

## Variabel dan Tipe Data
- Variabel digunakan untuk menyimpan data.
- Tipe data dasar Python meliputi:
  - Integer: `10`
  - Float: `3.14`
  - String: `"Hello"`
  - Boolean: `True` atau `False`

```python
# Contoh penggunaan variabel
umur = 20
nama = "John"
tinggi = 175.5
sudah_menikah = False
```

## Operasi Dasar
- Python mendukung berbagai operasi matematika dan logika.

```python
# Operasi Matematika
x = 10
y = 5
penjumlahan = x + y
pengurangan = x - y
perkalian = x * y
pembagian = x / y
modulus = x % y

# Operasi Logika
a = True
b = False
logika_and = a and b
logika_or = a or b
logika_not = not a
```

## Struktur Kontrol
### Pengkondisian
```python
umur = 18
if umur >= 18:
    print("Anda sudah dewasa")
else:
    print("Anda masih anak-anak")
```

### Perulangan
```python
# Perulangan dengan for
for i in range(5):
    print(i)

# Perulangan dengan while
counter = 0
while counter < 5:
    print(counter)
    counter += 1
```

## Fungsi
- Fungsi adalah blok kode yang dapat dipanggil dengan parameter tertentu.

```python
def tambah(x, y):
    return x + y

hasil = tambah(3, 5)  # Output: 8
```

## Modul
- Modul adalah file yang berisi definisi fungsi, variabel, dan pernyataan Python.
- Dapat diimpor ke dalam program Python lainnya.

```python
# Contoh penggunaan modul
import math

print(math.sqrt(16))  # Output: 4.0
```

## Penanganan Kesalahan
- Menggunakan blok `try` dan `except` untuk menangani pengecualian.

```python
try:
    nilai = int(input("Masukkan angka: "))
    print("Pangkat dua dari", nilai, "adalah", nilai**2)
except ValueError:
    print("Masukan bukan merupakan angka")
```

## Tips dan Trik
- Gunakan komentar untuk menjelaskan kode.
- Ikuti gaya penulisan kode Python (PEP 8).
- Gunakan nama variabel yang deskriptif.
- Rajinlah berlatih dan eksperimen dengan kode.

---

Ini hanya beberapa konsep dasar dalam pemrograman Python. Pastikan untuk terus belajar dan berlatih untuk menguasai lebih banyak konsep dan teknik dalam pengembangan perangkat lunak menggunakan Python.
