# Database Join

Dalam basis data relasional, operasi join digunakan untuk menggabungkan data dari dua atau lebih tabel berdasarkan kriteria tertentu. Operasi join memungkinkan pengguna untuk menggabungkan data yang terkait dari tabel yang berbeda untuk menghasilkan satu set data yang lebih lengkap.

## Jenis-Jenis Join

### 1. Inner Join
Inner join mengembalikan baris yang memiliki nilai kunci yang sesuai dalam kedua tabel yang terhubung. Hanya baris yang memiliki pasangan nilai dalam kedua tabel yang dimasukkan dalam hasil.

```sql
SELECT orders.OrderID, customers.CustomerName
FROM orders
INNER JOIN customers ON orders.CustomerID = customers.CustomerID;
```

### 2. Left Join (Outer Join)
Left join mengembalikan semua baris dari tabel kiri (tabel pertama yang disebutkan dalam pernyataan join), dan baris yang sesuai dari tabel kanan (tabel kedua yang disebutkan dalam pernyataan join). Jika tidak ada nilai yang cocok, nilai-nilai di kolom kanan akan NULL.

```sql
SELECT customers.CustomerName, orders.OrderID
FROM customers
LEFT JOIN orders ON customers.CustomerID = orders.CustomerID;
```

### 3. Right Join (Outer Join)
Right join adalah kebalikan dari left join. Ini mengembalikan semua baris dari tabel kanan (tabel kedua yang disebutkan dalam pernyataan join), dan baris yang sesuai dari tabel kiri (tabel pertama yang disebutkan dalam pernyataan join). Jika tidak ada nilai yang cocok, nilai-nilai di kolom kiri akan NULL.

```sql
SELECT orders.OrderID, customers.CustomerName
FROM orders
RIGHT JOIN customers ON orders.CustomerID = customers.CustomerID;
```

### 4. Full Outer Join
Full outer join mengembalikan baris saat ada kecocokan dalam salah satu dari tabel yang terhubung. Ini akan mengembalikan semua baris dari kedua tabel dan mengisi NULL pada kolom yang tidak memiliki nilai yang cocok.

```sql
SELECT customers.CustomerName, orders.OrderID
FROM customers
FULL OUTER JOIN orders ON customers.CustomerID = orders.CustomerID;
```

### 5. Cross Join
Cross join menghasilkan hasil kartesian dari kedua tabel yang terhubung. Ini menggabungkan setiap baris dari tabel pertama dengan setiap baris dari tabel kedua.

```sql
SELECT * FROM customers
CROSS JOIN orders;
```
