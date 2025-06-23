---
title: "\U0001F4D8 Eigenvalue dan Eigenvector"

---

# 📘 Eigenvalue dan Eigenvector

## 🔷 Pengantar

Dalam aljabar linear, **eigenvalue** dan **eigenvector** adalah konsep penting yang digunakan untuk memahami bagaimana transformasi linear bekerja terhadap vektor. Mereka sangat penting dalam berbagai bidang seperti machine learning, fisika, teknik, statistik, dan lainnya.

---

## 📌 Definisi Formal

Diberikan:
- Matriks persegi $A$ berukuran $n \times n$
- Vektor bukan nol $\mathbf{v}$
- Skalar $\lambda$

Jika:

$$
A \cdot \mathbf{v} = \lambda \cdot \mathbf{v}
$$

maka:
- $\mathbf{v}$ adalah **eigenvector**
- $\lambda$ adalah **eigenvalue**

---

## 📐 Intuisi Geometris

- Ketika vektor dikalikan dengan matriks $A$, arah vektor biasanya berubah.
- Tetapi jika vektor tersebut **tidak berubah arah**, hanya panjangnya saja yang berubah, maka vektor itu adalah **eigenvector**, dan skala perubahannya adalah **eigenvalue**.

---

## 🧮 Cara Mencari Eigenvalue dan Eigenvector

### Langkah 1: Persamaan Karakteristik

$$
\det(A - \lambda I) = 0
$$

Hasilnya adalah polinomial dengan akar-akar berupa nilai eigen (**eigenvalue**).

### Langkah 2: Substitusi untuk Mencari Eigenvector

Untuk setiap $\lambda$, substitusi ke:

$$
(A - \lambda I)\mathbf{v} = 0
$$

dan selesaikan untuk mendapatkan $\mathbf{v}$.

---

## 🔢 Contoh

Diberikan:

$$
A = \begin{bmatrix} 2 & 1 \\ 1 & 2 \end{bmatrix}
$$

### Langkah 1: Cari Eigenvalue

$$
\det(A - \lambda I) = \det \begin{bmatrix} 2 - \lambda & 1 \\ 1 & 2 - \lambda \end{bmatrix}
= (2 - \lambda)^2 - 1 = 0
$$

$$
(2 - \lambda)^2 = 1 \Rightarrow \lambda = 1, 3
$$

### Langkah 2: Cari Eigenvector

#### Untuk $\lambda = 3$:

$$
A - 3I = \begin{bmatrix} -1 & 1 \\ 1 & -1 \end{bmatrix}
$$

$$
x = y \Rightarrow \mathbf{v}_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

#### Untuk $\lambda = 1$:

$$
A - I = \begin{bmatrix} 1 & 1 \\ 1 & 1 \end{bmatrix}
$$

$$
x = -y \Rightarrow \mathbf{v}_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}
$$

---

## 🧠 Sifat-Sifat Penting

- Jumlah eigenvalue = $n$ (termasuk multiplikitas)
- $\det(A)$ adalah hasil kali seluruh eigenvalue
- $\operatorname{Tr}(A)$ (trace) adalah jumlah seluruh eigenvalue
- Jika $A$ simetris:
  - Semua $\lambda$ adalah bilangan real
  - Eigenvector dari eigenvalue yang berbeda **saling ortogonal**

### ✳️ Ortonormal vs Ortogonal

- **Ortogonal**: Dua vektor $\mathbf{u}$ dan $\mathbf{v}$ dikatakan ortogonal jika  
  $$
  \mathbf{u} \cdot \mathbf{v} = 0
  $$
  Artinya, sudut antara keduanya adalah 90°.

- **Ortonormal**: Dua (atau lebih) vektor dikatakan ortonormal jika mereka:
  - Saling **ortogonal**
  - Masing-masing **memiliki panjang (norma) 1**

Contoh ortonormal:

$$
\mathbf{u} = \begin{bmatrix} \frac{1}{\sqrt{2}} \\ \frac{1}{\sqrt{2}} \end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} \frac{1}{\sqrt{2}} \\ -\frac{1}{\sqrt{2}} \end{bmatrix}
$$

---

## 🧪 Aplikasi Dunia Nyata

| Bidang | Kegunaan |
|--------|----------|
| 📊 Machine Learning | PCA, reduksi dimensi |
| 🧬 Bioinformatika | Analisis ekspresi gen |
| 🌍 Fisika | Dinamika sistem dan getaran |
| 🖥️ Komputasi | PageRank oleh Google |
| 🎧 Sinyal & Gambar | Kompresi, filter, transformasi |

---

## ⚠️ Catatan

- Tidak semua matriks memiliki eigenvalue real.
- Jika tidak bisa didiagonalisasi, gunakan **Jordan Canonical Form**.
- Eigenvalue bisa kompleks (contoh: matriks rotasi).

---

## 📚 Kesimpulan

| Konsep | Penjelasan |
|--------|------------|
| **Eigenvalue** | Skalar $\lambda$ yang mengukur skala perubahan vektor |
| **Eigenvector** | Vektor $\mathbf{v}$ yang tidak berubah arah setelah transformasi |
| **Persamaan utama** | $A\mathbf{v} = \lambda\mathbf{v}$ |
| **Tujuan** | Memahami perilaku transformasi linear |

---

## ✅ Bonus: Kode Python (NumPy)

```python
import numpy as np

A = np.array([[2, 1], [1, 2]])
eigenvalues, eigenvectors = np.linalg.eig(A)

print("Eigenvalues:", eigenvalues)
print("Eigenvectors:\n", eigenvectors)
