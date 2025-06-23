---
title: ' Transformasi Matriks'

---

# 📐 Transformasi Matriks

## 📌 Pengertian
Transformasi matriks adalah proses memetakan titik-titik pada bidang (2D) atau ruang (3D) ke titik-titik baru menggunakan operasi matriks. Transformasi ini digunakan dalam berbagai bidang seperti grafika komputer, geometri, dan aljabar linear.

---

## 🧮 Representasi Umum

Misalkan vektor posisi:
$${\vec{v}} = \begin{bmatrix} x \\ y \end{bmatrix}$$

Maka transformasi linier:
$${\vec{v}}' = A \cdot {\vec{v}}$$

Dengan matriks transformasi:
$$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$$

---

## ✨ Jenis-jenis Transformasi Matriks

### 1. **Translasi**
Tidak bisa direpresentasikan langsung dengan matriks 2x2, melainkan menggunakan **matriks homogen**:

\begin{bmatrix}
x' \\
y' \\
1
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 & t_x \\
0 & 1 & t_y \\
0 & 0 & 1
\end{bmatrix}
\cdot
\begin{bmatrix}
x \\
y \\
1
\end{bmatrix}


### 2. **Rotasi**
Rotasi sebesar sudut θ terhadap titik asal:
$$
R(\theta) = 
\begin{bmatrix}
\cos \theta & -\sin \theta \\
\sin \theta & \cos \theta
\end{bmatrix}
$$

Contoh: Rotasi 90° searah jarum jam:
$$
\begin{bmatrix}
0 & 1 \\
-1 & 0
\end{bmatrix}
$$

### 3. **Refleksi (Pencerminan)**
- Terhadap sumbu X:
  $$
  \begin{bmatrix}
  1 & 0 \\
  0 & -1
  \end{bmatrix}
  $$
- Terhadap sumbu Y:
  $$
  \begin{bmatrix}
  -1 & 0 \\
  0 & 1
  \end{bmatrix}
  $$

### 4. **Dilatasi (Skalasi)**
- Skalasi umum:
  $$
  \begin{bmatrix}
  s_x & 0 \\
  0 & s_y
  \end{bmatrix}
  $$
- Jika $s_x = s_y = k$, maka hasilnya adalah pembesaran/pengecilan isotropik.

### 5. **Shear (Penggeseran)**
- Shear terhadap sumbu X:
  $$
  \begin{bmatrix}
  1 & k \\
  0 & 1
  \end{bmatrix}
  $$
- Shear terhadap sumbu Y:
  $$
  \begin{bmatrix}
  1 & 0 \\
  k & 1
  \end{bmatrix}
  $$

---

## 🔁 Komposisi Transformasi
Beberapa transformasi dapat digabung dengan mengalikan matriks transformasi secara berurutan:
$$
T = A_n \cdot A_{n-1} \cdots A_1
$$

---

## 💡 Contoh Kasus

Misalkan titik awal $\vec{v} = \begin{bmatrix} 2 \\ 3 \end{bmatrix}$, dan dilakukan rotasi 90° berlawanan arah jarum jam.

Gunakan matriks rotasi:
$$
R = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}
$$

Hitung:
$$
\vec{v}' = R \cdot \vec{v} = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix} \cdot \begin{bmatrix} 2 \\ 3 \end{bmatrix} = \begin{bmatrix} -3 \\ 2 \end{bmatrix}
$$

---

## 📚 Kesimpulan
Transformasi matriks adalah cara sistematis untuk memanipulasi bentuk dan posisi objek dalam ruang menggunakan aljabar linear. Setiap jenis transformasi memiliki matriks khusus yang dapat dikombinasikan untuk membentuk transformasi kompleks.

---
