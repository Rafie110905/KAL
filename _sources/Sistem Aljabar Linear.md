# Sistem Persamaan Linear

## 1. Pengertian
Sistem Persamaan Linear adalah kumpulan dua atau lebih persamaan linear yang memiliki satu atau lebih variabel. Penyelesaian dari sistem ini adalah nilai variabel yang memenuhi semua persamaan dalam sistem.

## 2. Bentuk Umum
- **Dua variabel:**
  ```math
  \begin{cases} 
  ax + by = c \\ 
  dx + ey = f 
  \end{cases}
  ```
- **Tiga variabel:**
  ```math
  \begin{cases} 
  ax + by + cz = d \\ 
  ex + fy + gz = h \\ 
  ix + jy + kz = l 
  \end{cases}
  ```

## 3. Metode Penyelesaian

### a. Metode Substitusi
1. Nyatakan salah satu variabel dalam bentuk variabel lainnya.
2. Substitusikan ke persamaan lain.
3. Selesaikan hingga mendapatkan nilai variabel.

#### Contoh:
```math
\begin{cases} 
2x + y = 8 \\ 
x - y = 2 
\end{cases}
```
- Dari persamaan kedua: `x = y + 2`
- Substitusi ke persamaan pertama:
  ```math
  2(y+2) + y = 8
  ```
  ```math
  3y + 4 = 8 \Rightarrow y = 4
  ```
- Substitusi `y = 4` ke `x = y + 2`: `x = 6`
- **Solusi**: `(6,4)`

### b. Metode Eliminasi
1. Samakan koefisien salah satu variabel.
2. Kurangi atau jumlahkan persamaan untuk menghilangkan satu variabel.
3. Selesaikan persamaan yang tersisa.

#### Contoh:
```math
\begin{cases} 
3x + 2y = 12 \\ 
5x - 2y = 8 
\end{cases}
```
- **Eliminasi `y`** dengan menjumlahkan kedua persamaan:
  ```math
  (3x + 2y) + (5x - 2y) = 12 + 8
  ```
  ```math
  8x = 20 \Rightarrow x = 2.5
  ```
- Substitusi `x = 2.5` ke persamaan pertama:
  ```math
  3(2.5) + 2y = 12
  ```
  ```math
  7.5 + 2y = 12 \Rightarrow y = 2.25
  ```
- **Solusi**: `(2.5, 2.25)`

### c. Metode Matriks (Metode Gauss-Jordan)
Persamaan dapat ditulis dalam bentuk matriks:
```math
\begin{bmatrix} a & b & | & c \\ d & e & | & f \end{bmatrix}
```
Gunakan operasi baris untuk mendapatkan bentuk matriks eselon tereduksi.

#### Contoh:
Dari sistem
```math
\begin{cases} 
2x + y = 5 \\ 
x - y = 1 
\end{cases}
```
Dapat ditulis sebagai:
```math
\begin{bmatrix} 2 & 1 & | 5 \\ 1 & -1 & | 1 \end{bmatrix}
```
Gunakan operasi baris hingga diperoleh solusi `x` dan `y`.

## 4. Jenis Solusi
1. **Satu solusi unik** → Jika persamaan memiliki satu titik potong.
2. **Tak terhingga banyak solusi** → Jika dua persamaan identik atau sejajar.
3. **Tidak ada solusi** → Jika persamaan tidak memiliki titik potong (garis sejajar).

## 5. Contoh Soal dan Latihan
**Soal 1:**
Selesaikan sistem persamaan berikut dengan metode eliminasi:
```math
\begin{cases} 
4x + 3y = 20 \\ 
2x - y = 4 
\end{cases}
```

**Jawaban:**
1. Kalikan persamaan kedua dengan `3` agar koefisien `y` sama:
   ```math
   \begin{cases} 
   4x + 3y = 20 \\ 
   6x - 3y = 12 
   \end{cases}
   ```
2. Eliminasi `y` dengan menjumlahkan kedua persamaan:
   ```math
   10x = 32 \Rightarrow x = 3.2
   ```
3. Substitusi `x = 3.2` ke `2x - y = 4`:
   ```math
   6.4 - y = 4 \Rightarrow y = 2.4
   ```
4. **Solusi**: `(3.2, 2.4)`

**Soal 2:**
Selesaikan sistem berikut dengan metode substitusi:
```math
\begin{cases} 
5x + 2y = 14 \\ 
3x - y = 1 
\end{cases}
```

**Jawaban:**
1. Nyatakan `y` dari persamaan kedua:
   ```math
   y = 3x - 1
   ```
2. Substitusi ke persamaan pertama:
   ```math
   5x + 2(3x - 1) = 14
   ```
   ```math
   5x + 6x - 2 = 14
   ```
   ```math
   11x = 16 \Rightarrow x = \frac{16}{11}
   ```
3. Substitusi `x = \frac{16}{11}` ke `y = 3x - 1`:
   ```math
   y = 3 \times \frac{16}{11} - 1 = \frac{48}{11} - \frac{11}{11} = \frac{37}{11}
   ```
4. **Solusi**: `(\frac{16}{11}, \frac{37}{11})`

## 6. Kesimpulan
- Sistem Persamaan Linear terdiri dari dua atau lebih persamaan linear.
- Dapat diselesaikan dengan metode **Substitusi, Eliminasi, atau Matriks**.
- Solusinya bisa berupa **satu solusi, banyak solusi, atau tidak ada solusi**.
