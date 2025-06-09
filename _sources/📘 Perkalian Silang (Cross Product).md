---
title: "\U0001F4D8 Perkalian Silang (Cross Product)"

---

# 📘 Perkalian Silang (Cross Product)

## 📌 Pendahuluan
Dalam ruang tiga dimensi (R³), terdapat dua jenis operasi pada vektor: **perkalian titik (dot product)** dan **perkalian silang (cross product)**. Perkalian silang menghasilkan sebuah **vektor baru yang tegak lurus** terhadap kedua vektor asal. Operasi ini sangat berguna dalam berbagai bidang seperti fisika, teknik, dan komputer grafis.

---

## 🧮 Definisi Matematis
Diberikan dua vektor **A** dan **B** di R³:
- **A** = (a₁, a₂, a₃)
- **B** = (b₁, b₂, b₃)

Perkalian silang A × B didefinisikan sebagai:
```
A × B = |  i    j    k  |
        | a₁  a₂  a₃ |
        | b₁  b₂  b₃ |
```

Hasil determinan matriks di atas adalah:
```
A × B = (a₂b₃ - a₃b₂)i - (a₁b₃ - a₃b₁)j + (a₁b₂ - a₂b₁)k
```

---

## 🧠 Intuisi Geometris
- Arah dari **A × B** ditentukan oleh **aturan tangan kanan**.
- Panjangnya setara dengan **luas jajar genjang** yang dibentuk oleh A dan B:
```
|A × B| = |A| × |B| × sin(θ)
```
dimana θ adalah sudut antara vektor A dan B.

---

## 📘 Contoh Perhitungan

### Contoh 1:
Diberikan vektor:
- A = (1, 2, 3)
- B = (4, 5, 6)

Hitung A × B:
```
= |i  j  k |
  |1  2  3|
  |4  5  6|

= i(2×6 - 3×5) - j(1×6 - 3×4) + k(1×5 - 2×4)
= i(12 - 15) - j(6 - 12) + k(5 - 8)
= -3i + 6j - 3k
```

Hasil: **A × B = (-3, 6, -3)**

---

## ✅ Sifat-Sifat Perkalian Silang

| No | Sifat | Keterangan |
|----|-------|------------|
| 1 | **A × B = - (B × A)** | Anti-komutatif |
| 2 | **A × A = 0** | Karena sin(0) = 0 |
| 3 | **(kA) × B = k (A × B)** | k adalah skalar |
| 4 | **A × (B + C) = A × B + A × C** | Distribusi |
| 5 | **A · (A × B) = 0** | Tegak lurus terhadap A dan B |

---

## 🛠️ Implementasi dalam Dunia Nyata

1. **Fisika**: Menghitung momen gaya (τ = r × F)
2. **Grafika Komputer**: Menentukan normal permukaan (digunakan dalam pencahayaan dan shading)
3. **Robotika**: Menentukan arah gerakan atau rotasi
4. **Teknik Mesin**: Perhitungan torsi

---

## 📦 Volume Paralelepiped

Sebuah **paralelepiped** adalah bangun tiga dimensi yang dibentuk oleh tiga vektor: A, B, dan C. Volume bangun ini dihitung dengan:

```
Volume = |A · (B × C)|
```

### Contoh:
- A = (1, 0, 0)
- B = (0, 1, 0)
- C = (0, 0, 1)

Langkah-langkah:
1. B × C = (1, 0, 0)
2. A · (B × C) = 1
3. Volume = |1| = **1 satuan kubik**

---

## 🎯 Latihan Soal

### Soal 1
Hitung hasil dari A × B jika:
- A = (3, -3, 1)
- B = (4, 9, 2)

### Soal 2
Tentukan hasil perkalian silang untuk:
- A = (2, -1, 3)
- B = (1, 4, -2)

### Soal 3 (Volume)
Diberikan:
- A = (1, 2, 3)
- B = (4, 5, 6)
- C = (7, 8, 9)

Hitunglah volume paralelepiped yang dibentuk oleh ketiga vektor tersebut.

---

## 📓 Kesimpulan

Perkalian silang adalah alat penting dalam vektor tiga dimensi:
- Menghasilkan vektor ortogonal terhadap dua vektor asal
- Digunakan untuk menghitung luas jajar genjang dan volume bangun ruang
- Memiliki sifat anti-komutatif dan hasil selalu tegak lurus terhadap dua vektor asal


