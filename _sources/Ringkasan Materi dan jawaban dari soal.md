---
title: Ringkasan Materi dan jawaban dari soal

---

# Ringkasan Materi Halaman 225–238: Transformasi Linear & Matriks

## 1. Transformasi Linear

Transformasi linear adalah fungsi $$T: \mathbb{R}^n \to \mathbb{R}^m$$ yang memetakan vektor dengan dua sifat:

- *Preservasi penjumlahan*:  
  $$T(\vec{u} + \vec{v}) = T(\vec{u}) + T(\vec{v})$$

- *Preservasi perkalian skalar*:  
  $$T(c\vec{v}) = cT(\vec{v})$$

*Contoh transformasi linear*:
- Refleksi
- Rotasi
- Skala
- Proyeksi

---

## 2. Representasi Matriks dari Transformasi

Setiap transformasi linear bisa direpresentasikan dengan matriks:

$$
T(\vec{x}) = A\vec{x}
$$

Untuk mencari matriks $A$:
- Gunakan vektor basis standar:
  - $$\vec{e}_1 = \begin{bmatrix}1 \\ 0\end{bmatrix}$$
  - $$\vec{e}_2 = \begin{bmatrix}0 \\ 1\end{bmatrix}$$
- Hitung:
  - $$T(\vec{e}_1) \Rightarrow$$ kolom pertama
  - $$T(\vec{e}_2) \Rightarrow$$ kolom kedua
- Matriks:
  $$
  A = \begin{bmatrix} T(\vec{e}_1) & T(\vec{e}_2) \end{bmatrix}
  $$

---

## 3. Interpretasi Geometris

Transformasi linear mengubah bentuk objek seperti unit square.

Jenis transformasi:
- *Rotasi*: memutar
- *Refleksi*: membalik
- *Shear*: menggeser
- *Skala*: memperbesar / memperkecil

Contoh:
$$
A = \begin{bmatrix}2 & 0 \\ 0 & 3\end{bmatrix}
$$
Mengubah ukuran 2x pada $x$ dan 3x pada $y$.

---

## 4. Contoh Penghitungan

Diketahui:
$$
A = \begin{bmatrix} 2 & -1 \\ 1 & 3 \end{bmatrix}, \quad \vec{x} = \begin{bmatrix}1 \\ 1\end{bmatrix}
$$

Maka:
$$
A\vec{x} = \begin{bmatrix}2*1 + (-1)*1 \\ 1*1 + 3*1\end{bmatrix} = \begin{bmatrix}1 \\ 4\end{bmatrix}
$$

---

## 5. Komposisi Transformasi

Transformasi linear bisa dikomposisikan:

$$
T = T_2 \circ T_1 \Rightarrow T(\vec{x}) = B(A\vec{x}) = (BA)\vec{x}
$$

Komposisi = perkalian matriks.

---

## 6. Invers Transformasi

Jika $T$ bisa dibalik, maka ada $T^{-1}$:
$$
T^{-1}(T(\vec{x})) = \vec{x}
$$

Dalam bentuk matriks:
$$
A^{-1}A = I
$$

Syarat:
- Matriks persegi
- Determinan tidak nol

---

## 7. Visualisasi Gambar ke Matriks

Contoh:
- $$T\left(\begin{bmatrix}1 \\ 0\end{bmatrix}\right) = \begin{bmatrix}1 \\ 2\end{bmatrix}$$
- $$T\left(\begin{bmatrix}0 \\ 1\end{bmatrix}\right) = \begin{bmatrix}0 \\ 3\end{bmatrix}$$

Maka:
$$
A = \begin{bmatrix}1 & 0 \\ 2 & 3\end{bmatrix}
$$

---


### *Nomor 1*

Diketahui:

$$
A = \begin{bmatrix} 2 & -1 \\ 1 & 3 \end{bmatrix}, \quad 
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad 
\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

Hitung:

$$
A\vec{x} = \begin{bmatrix} 2 & -1 \\ 1 & 3 \end{bmatrix} 
\begin{bmatrix} 1 \\ 1 \end{bmatrix} 
= \begin{bmatrix} 1 \\ 4 \end{bmatrix}
$$

$$
A\vec{y} = \begin{bmatrix} 2 & -1 \\ 1 & 3 \end{bmatrix} 
\begin{bmatrix} -1 \\ 2 \end{bmatrix} 
= \begin{bmatrix} -4 \\ 5 \end{bmatrix}
$$

---

### *Nomor 2*

Diketahui:

$$
A = \begin{bmatrix} 2 & 0 \\ 0 & 3 \end{bmatrix}, \quad 
\vec{x} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \quad 
\vec{y} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

Hitung:

$$
A\vec{x} = \begin{bmatrix} 2 \\ 3 \end{bmatrix}, \quad 
A\vec{y} = \begin{bmatrix} -2 \\ 6 \end{bmatrix}
$$

---

### *Nomor 5*

Dari gambar, diketahui:

- $$\begin{bmatrix} 1 \\ 0 \end{bmatrix} \mapsto \begin{bmatrix} 1 \\ 2 \end{bmatrix}$$
- $$\begin{bmatrix} 0 \\ 1 \end{bmatrix} \mapsto \begin{bmatrix} 0 \\ 3 \end{bmatrix}$$

Maka matriks transformasi:

$$
A = \begin{bmatrix} 1 & 0 \\ 2 & 3 \end{bmatrix}
$$

---

### *Nomor 6*

Dari gambar, diketahui:

- $$\begin{bmatrix} 1 \\ 0 \end{bmatrix} \mapsto \begin{bmatrix} 1 \\ 1 \end{bmatrix}$$
- $$\begin{bmatrix} 0 \\ 1 \end{bmatrix} \mapsto \begin{bmatrix} -1 \\ 1 \end{bmatrix}$$

Maka matriks transformasi:

$$
A = \begin{bmatrix} 1 & -1 \\ 1 & 1 \end{bmatrix}
$$
