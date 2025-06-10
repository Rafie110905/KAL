---
title: "\U0001F4D8 Perkalian Silang (Cross Product)"

---

# 📘 Perkalian Silang (Cross Product)

## 📌 Pendahuluan
Perkalian silang adalah operasi antara dua vektor dalam ruang tiga dimensi ($\mathbb{R}^3$) yang menghasilkan vektor baru yang tegak lurus terhadap kedua vektor asal. Operasi ini digunakan untuk menghitung **luas jajar genjang**, **luas segitiga**, serta **volume bangun ruang** seperti paralelepiped.

---

## 🧮 Definisi dan Rumus
Jika terdapat dua vektor:
- $\vec{u} = (a_1, a_2, a_3)$
- $\vec{v} = (b_1, b_2, b_3)$

Maka:
$$
\vec{u} \times \vec{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3
\end{vmatrix}
$$

Hasilnya adalah:
$$
\vec{u} \times \vec{v} = 
\left( a_2b_3 - a_3b_2, \ 
a_3b_1 - a_1b_3, \ 
a_1b_2 - a_2b_1 \right)
$$

---

## 📐 Luas Jajar Genjang & Segitiga

### Luas Jajar Genjang
Dua vektor $\vec{u}$ dan $\vec{v}$ membentuk sebuah jajar genjang. Luasnya dihitung dari panjang vektor hasil perkalian silang:
$$
\text{Luas} = |\vec{u} \times \vec{v}|
$$

### Luas Segitiga
Jika tiga titik A, B, dan C membentuk segitiga, maka:
- $\vec{AB} = \vec{B} - \vec{A}$
- $\vec{AC} = \vec{C} - \vec{A}$

Luas segitiga:
$$
\text{Luas} = \frac{1}{2} |\vec{AB} \times \vec{AC}|
$$

---

## ✅ Penyelesaian Soal

### 🧮 Soal 1:
Diketahui:
- $\vec{u} = [1, 2]$, $\vec{v} = [2, 1]$  
- Diasumsikan $\vec{u} = (1, 2, 0)$, $\vec{v} = (2, 1, 0)$

$$
\vec{u} \times \vec{v} = 
(2 \cdot 0 - 0 \cdot 1, \ 
0 \cdot 2 - 1 \cdot 0, \ 
1 \cdot 1 - 2 \cdot 2) = (0, 0, -3)
$$

$$
|\vec{u} \times \vec{v}| = \sqrt{0^2 + 0^2 + (-3)^2} = 3
$$

✅ **Jawaban: 3 satuan luas**

---

### 🧮 Soal 2:
$\vec{u} = (2, 0, 0)$, $\vec{v} = (0, 3, 0)$

$$
\vec{u} \times \vec{v} = 
(0 \cdot 0 - 0 \cdot 3, \ 
0 \cdot 0 - 2 \cdot 0, \ 
2 \cdot 3 - 0 \cdot 0) = (0, 0, 6)
$$

$$
|\vec{u} \times \vec{v}| = 6
$$

✅ **Jawaban: 6 satuan luas**

---

### 🧮 Soal 3:
Titik-titik sudut: $A = (0,0,0)$, $B = (1,3,-1)$, $C = (2,1,1)$  
Vektor:
- $\vec{AB} = (1,3,-1)$
- $\vec{AC} = (2,1,1)$

$$
\vec{AB} \times \vec{AC} = 
\left| \begin{array}{ccc}
i & j & k \\
1 & 3 & -1 \\
2 & 1 & 1
\end{array} \right| = (3 \cdot 1 - (-1) \cdot 1, - (1 \cdot 1 - (-1) \cdot 2), 1 \cdot 1 - 3 \cdot 2) = (4, -3, -5)
$$

$$
|\vec{AB} \times \vec{AC}| = \sqrt{4^2 + (-3)^2 + (-5)^2} = \sqrt{50}
$$

$$
\text{Luas} = \frac{1}{2} \sqrt{50} \approx 3.54
$$

✅ **Jawaban: sekitar 3.54 satuan luas**

---

### 🧮 Soal 4:
Titik-titik: $A = (5,2,-1)$, $B = (3,6,2)$, $C = (1,0,4)$  
Vektor:
- $\vec{AB} = (-2, 4, 3)$
- $\vec{AC} = (-4, -2, 5)$

$$
\vec{AB} \times \vec{AC} = 
\left( 4 \cdot 5 - 3 \cdot (-2), \
3 \cdot (-4) - (-2) \cdot 5, \
(-2) \cdot (-2) - 4 \cdot (-4) \right) = (26, -2, 20)
$$

$$
|\vec{AB} \times \vec{AC}| = \sqrt{26^2 + (-2)^2 + 20^2} = \sqrt{1080} \approx 32.86
$$

$$
\text{Luas} = \frac{1}{2} \times 32.86 \approx 16.43
$$

✅ **Jawaban: sekitar 16.43 satuan luas**

---

## 📓 Kesimpulan

- Perkalian silang menghasilkan vektor tegak lurus dari dua vektor dalam $\mathbb{R}^3$.
- Panjang hasil cross product menunjukkan luas jajar genjang.
- Luas segitiga adalah setengah dari luas jajar genjang.
- Digunakan dalam banyak bidang sains dan teknik, termasuk fisika dan komputer grafis.