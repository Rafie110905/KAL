---
title: 'Bukti bahwa $T(v_1, v_2) = (v_1 + v_2, v_1)$ adalah Transformasi Linier'

---

# Pembuktian Transformasi Linier

Diberikan transformasi $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$ sebagai berikut:

$$
T(v_1, v_2) = (v_1 + v_2, v_1)
$$

Kita akan membuktikan bahwa $T$ adalah **transformasi linier**, yaitu memenuhi dua sifat:

1. **Preservasi Penjumlahan**:
   $$
   T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})
   $$

2. **Preservasi Perkalian Skalar**:
   $$
   T(c \cdot \mathbf{v}) = c \cdot T(\mathbf{v})
   $$

---

## 1. Uji Penjumlahan

Misalkan:

$$
\mathbf{u} = (u_1, u_2), \quad \mathbf{v} = (v_1, v_2)
$$

Hitung:

$$
\mathbf{u} + \mathbf{v} = (u_1 + v_1, u_2 + v_2)
$$

$$
T(\mathbf{u} + \mathbf{v}) = T(u_1 + v_1, u_2 + v_2) = ((u_1 + v_1) + (u_2 + v_2), u_1 + v_1)
$$

$$
= (u_1 + v_1 + u_2 + v_2, u_1 + v_1)
$$

Sementara:

$$
T(\mathbf{u}) = (u_1 + u_2, u_1), \quad T(\mathbf{v}) = (v_1 + v_2, v_1)
$$

$$
T(\mathbf{u}) + T(\mathbf{v}) = (u_1 + u_2 + v_1 + v_2, u_1 + v_1)
$$

Karena:

$$
T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})
$$

✅ Sifat penjumlahan **terpenuhi**.

---

## 2. Uji Perkalian Skalar

Misalkan:

$$
\mathbf{v} = (v_1, v_2), \quad c \in \mathbb{R}
$$

Hitung:

$$
c \cdot \mathbf{v} = (cv_1, cv_2)
$$

$$
T(c \cdot \mathbf{v}) = T(cv_1, cv_2) = (cv_1 + cv_2, cv_1) = c(v_1 + v_2, v_1)
$$

$$
c \cdot T(\mathbf{v}) = c(v_1 + v_2, v_1) = (cv_1 + cv_2, cv_1)
$$

Karena:

$$
T(c \cdot \mathbf{v}) = c \cdot T(\mathbf{v})
$$

✅ Sifat perkalian skalar **terpenuhi**.

---

## ✅ Kesimpulan

Karena transformasi $T(v_1, v_2) = (v_1 + v_2, v_1)$ memenuhi dua sifat transformasi linier, maka:

$$
T \text{ adalah transformasi linier.}
$$
