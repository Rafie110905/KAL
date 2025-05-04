---
title: 'Ringkasan tentang Transformasi Linear'

---

# Transformasi Linier

## Pengantar Transformasi Linier

### Definisi
Fungsi $T$ yang memetakan ruang vektor $V$ ke ruang vektor $W$:
- $V$: domain $T$
- $W$: kodomain $T$

### Contoh Soal
Untuk transformasi $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$:
1. Cari bayangan $\mathbf{v}=(-1,2)$
2. Cari prabayangan $\mathbf{w}=(-1,11)$

**Solusi**:
Prabayangan $\mathbf{w}=(-1,11)$ adalah $\{(3,4)\}$

##  Matriks untuk Transformasi Linier

### Catatan Penting
1. Transformasi linier mempertahankan operasi aljabar linier
2. Transformasi linier dari $V$ ke $V$ disebut operator linier

### Transformasi Khusus
- **Transformasi nol**: $T(\mathbf{v}) = \mathbf{0}$
- **Transformasi identitas**: $T(\mathbf{v}) = \mathbf{v}$

### Representasi Matriks
Untuk matriks $A$ berukuran $m \times n$, fungsi $T(\mathbf{v}) = A\mathbf{v}$ adalah transformasi linier dari $\mathbb{R}^n$ ke $\mathbb{R}^m$

#### Contoh Matriks
1. **Rotasi** di $\mathbb{R}^2$ dengan sudut $\theta$:
$$
A = \begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
$$

2. **Proyeksi** di $\mathbb{R}^3$:
$$
A = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$

##  Kemiripan

### Matriks Standar
Matriks $A$ yang memenuhi:
$$
T(\mathbf{v}) = A\mathbf{v} \quad \forall \mathbf{v} \in \mathbb{R}^n
$$

### Mencari Matriks Standar
1. Transformasi nol: matriks nol $m \times n$
2. Transformasi identitas: matriks identitas $n \times n$

### Komposisi Transformasi
Untuk $T_1: \mathbb{R}^n \rightarrow \mathbb{R}^m$ dan $T_2: \mathbb{R}^m \rightarrow \mathbb{R}^p$:
$$
[T_2 \circ T_1] = [T_2][T_1]
$$

## Transformasi Invers

### Definisi
Jika $T$ invertible, invers $T^{-1}$ bersifat unik dan memenuhi:
$$
T^{-1}(T(\mathbf{v})) = \mathbf{v}
$$

### Representasi Matriks
$$
[T^{-1}] = [T]^{-1}
$$

## Basis Non-Standar

### Matriks Relatif terhadap Basis $B$
Untuk basis $B = \{\mathbf{b}_1, ..., \mathbf{b}_n\}$:
$$
[T]_B = P^{-1}[T]_{\text{standar}}P
$$
dengan $P$ matriks perubahan basis.

## Matriks Diagonal

### Sifat-Sifat
1. Nilai eigen adalah elemen diagonal
2. Perhitungan pangkat matriks diagonal lebih mudah

---

## Contoh Soal dan Penyelesaian

### Latihan 1
Buktikan $T(v_1,v_2) = (v_1 + v_2, v_1)$ adalah transformasi linier.

**Penyelesaian**:
1. Penjumlahan vektor:
$$
T(\mathbf{u}+\mathbf{v}) = T(u_1+v_1, u_2+v_2) = \cdots = T(\mathbf{u}) + T(\mathbf{v})
$$
2. Perkalian skalar:
$$
T(c\mathbf{v}) = \cdots = cT(\mathbf{v})
$$

### Latihan 2
Cari matriks standar untuk $T(x,y,z) = (x+y, y-z, x+z)$

**Penyelesaian**:
$$
A = \begin{bmatrix}
1 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{bmatrix}
$$

### Latihan 3
Tunjukkan matriks rotasi mempertahankan panjang vektor.

**Penyelesaian**:
Untuk $\mathbf{v} \in \mathbb{R}^2$:
$$
\|T(\mathbf{v})\| = \|A\mathbf{v}\| = \|\mathbf{v}\|
$$

---

## Teorema Penting
1. **Teorema Rank-Nullity**:
$$
\dim(\text{Ker}(T)) + \dim(\text{Range}(T)) = \dim(V)
$$
2. **Kemiripan Matriks**:
Dua matriks merepresentasikan transformasi linier yang sama jika dan hanya jika similar