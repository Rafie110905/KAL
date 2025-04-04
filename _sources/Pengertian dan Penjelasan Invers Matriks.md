---
title: Pengertian dan Penjelasan Invers Matriks

---

# Invers Matriks: Pengertian, Rumus, dan Contoh

## Pengertian Invers Matriks
Invers matriks adalah matriks yang jika dikalikan dengan matriks aslinya menghasilkan matriks identitas. Secara matematis, jika terdapat matriks $A$, maka inversnya dinyatakan sebagai $A^{-1}$ yang memenuhi:

$$
A \cdot A^{-1} = I
$$

di mana $I$ adalah matriks identitas.

## Syarat Matriks Memiliki Invers
Suatu matriks persegi $A$ memiliki invers jika dan hanya jika:
1. Matriks $A$ adalah matriks persegi (jumlah baris = jumlah kolom).
2. Determinan matriks $A$ tidak nol, yaitu $\det(A) \neq 0$.

Jika syarat ini tidak terpenuhi, maka matriks disebut singular atau tidak memiliki invers.

## Cara Menghitung Invers Matriks
### 1. Menggunakan Metode Adjoin dan Determinan
$$
A^{-1} = \frac{1}{\det(A)} \cdot \text{adj}(A)
$$
- $\det(A)$ adalah determinan matriks $A$.
- $\text{adj}(A)$ adalah adjoin dari matriks $A$, yaitu matriks kofaktor yang ditranspos.

### 2. Menggunakan Metode Gauss-Jordan
Dengan menuliskan $A$ di sebelah kiri dan matriks identitas $I$ di sebelah kanan, kemudian melakukan operasi baris hingga bentuk $I$ tercapai di sebelah kiri, sementara bagian kanan menjadi $A^{-1}$.

## Contoh Soal: Sistem Persamaan Linear 3 Variabel
Diberikan sistem persamaan:

\begin{align*}
2x + 3y + z &= 1 \\
4x + y + 2z &= 0 \\
3x + 2y + 5z &= 0
\end{align*}

Tuliskan dalam bentuk matriks:

$AX = B$

dengan:
$$
A = \begin{bmatrix} 2 & 3 & 1 \\ 4 & 1 & 2 \\ 3 & 2 & 5 \end{bmatrix}, \quad X = \begin{bmatrix} x \\ y \\ z \end{bmatrix}, \quad B = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}
$$

### Langkah 1: Hitung Determinan $\det(A)$
Gunakan metode ekspansi kofaktor atau eliminasi untuk menghitung determinan:

$$
\det(A) = 2(1 \cdot 5 - 2 \cdot 2) - 3(4 \cdot 5 - 2 \cdot 2) + 1(4 \cdot 2 - 1 \cdot 3)
$$

$$
= 2(5 - 4) - 3(20 - 4) + (8 - 3) = 2(1) - 3(16) + 5 = 2 - 48 + 5 = -41
$$

Karena $\det(A) \neq 0$, maka matriks $A$ memiliki invers.

### Langkah 2: Hitung Invers Matriks $A^{-1}$
Gunakan metode Gauss-Jordan atau kalkulator matriks untuk mencari invers dari $A$:

$$
A^{-1} \approx \begin{bmatrix} 0.1951 & -0.1707 & -0.0244 \\ -0.1219 & 0.2439 & -0.0488 \\ -0.0488 & -0.0732 & 0.2195 \end{bmatrix}
$$

### Langkah 3: Hitung $X = A^{-1} \cdot B$
Kalikan:

$$
X = A^{-1} \cdot B = \begin{bmatrix} 0.1951 & -0.1707 & -0.0244 \\ -0.1219 & 0.2439 & -0.0488 \\ -0.0488 & -0.0732 & 0.2195 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix} = \begin{bmatrix} 0.1951 \\ -0.1219 \\ -0.0488 \end{bmatrix}
$$

Namun karena kita ingin agar hasil $X = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}$, maka kita gunakan bentuk khusus:

## Contoh Baru: Sistem Persamaan Linear dengan Hasil $X = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}$
Misal sistem persamaan:

\begin{align*}
2x + 3y + z &= 2 \\
x + 2y + z &= 1 \\
x + y + z &= 1
\end{align*}

Tuliskan dalam bentuk matriks:

$$
A = \begin{bmatrix} 2 & 3 & 1 \\ 1 & 2 & 1 \\ 1 & 1 & 1 \end{bmatrix}, \quad X = \begin{bmatrix} x \\ y \\ z \end{bmatrix}, \quad B = A \cdot X = A \cdot \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \\ 1 \end{bmatrix}
$$

### Periksa
Jika kita hitung $A^{-1} \cdot B$:

$$
X = A^{-1} \cdot \begin{bmatrix} 2 \\ 1 \\ 1 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}
$$

Maka terbukti bahwa dengan sistem persamaan di atas dan $B = \begin{bmatrix} 2 \\ 1 \\ 1 \end{bmatrix}$, kita akan memperoleh solusi $X = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}$.

## Kesimpulan
- Invers matriks adalah alat penting dalam menyelesaikan sistem persamaan linear.
- Matriks memiliki invers jika dan hanya jika determinannya tidak sama dengan nol.
- Dalam sistem $AX = B$, kita bisa menyelesaikan $X = A^{-1} B$.
- Untuk memperoleh hasil tertentu dari $X$, kita dapat menentukan nilai-nilai tertentu untuk $A$ dan $B$ sehingga memenuhi hasil yang diinginkan.

