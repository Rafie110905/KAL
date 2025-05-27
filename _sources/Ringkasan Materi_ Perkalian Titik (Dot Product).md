---
title: "\U0001F4D8 Ringkasan Materi: Perkalian Titik (Dot Product)"

---

#  Ringkasan Materi: Perkalian Titik (Dot Product)

##  Definisi
Perkalian titik (dot product) adalah operasi matematika antara dua vektor yang menghasilkan **skalar**. Digunakan dalam berbagai bidang seperti fisika, grafik komputer, dan pembelajaran mesin.

##  Rumus Umum
$$
 \mathbf{v} \cdot \mathbf{w} = 
\begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
\cdot
\begin{bmatrix}
w_1 \\
w_2
\end{bmatrix}
= v_1w_1 + v_2w_2.
$$

Sebagai Contoh :
$$
\begin{bmatrix}
2 \\
-3
\end{bmatrix}
\cdot
\begin{bmatrix}
4 \\
1
\end{bmatrix}
= 2 \cdot 4 + (-3) \cdot 1 = 5.
$$

##  Dot Product & Sudut
Dot product juga dapat dihitung menggunakan sudut di antara dua vektor:
$$
\mathbf{A} \cdot \mathbf{B} = |\mathbf{A}| |\mathbf{B}| \cos(\theta)
$$
- $|\mathbf{A}|$ = panjang vektor A  
- $|\mathbf{B}|$ = panjang vektor B  
- $\theta$ = sudut antara vektor A dan B

##  Syarat
- Kedua vektor harus memiliki **jumlah dimensi yang sama**

##  Contoh
Diberikan:
- $\mathbf{A} = [2, 3]$  
- $\mathbf{B} = [4, -1]$

Maka:
$$
\mathbf{A} \cdot \mathbf{B} = (2 \times 4) + (3 \times -1) = 8 - 3 = 5
$$

##  Interpretasi Geometris
- $\mathbf{A} \cdot \mathbf{B} > 0$: sudut $<$ 90° → vektor searah  
- $\mathbf{A} \cdot \mathbf{B} = 0$: sudut = 90° → vektor tegak lurus  
- $\mathbf{A} \cdot \mathbf{B} < 0$: sudut $>$ 90° → vektor berlawanan arah

##  Aplikasi Dot Product
- Menentukan apakah dua vektor **tegak lurus**
- Proyeksi vektor
- Fisika (kerja = gaya × perpindahan)
- Grafik komputer (shading & pencahayaan)

##  Kesimpulan
Dot product adalah alat penting dalam analisis vektor yang sederhana namun sangat berguna dalam berbagai aplikasi praktis dan teoretis.

#  Visualisasi Interaktif: Dot Product dengan GeoGebra

Perkalian Titik: Menunjukkan bagaimana dot product dihitung sebagai $v_1w_1 + v_2w_2$.

Hubungan dengan Sudut: Menunjukkan bahwa dot product juga dapat dihitung sebagai $|\mathbf{v}||\mathbf{w}|\cos(\theta)$, di mana $\theta$ adalah sudut antara vektor.

Interpretasi Geometris: Membantu memahami bagaimana dot product berkaitan dengan proyeksi satu vektor ke vektor lainnya.

<iframe src="https://www.geogebra.org/material/iframe/id/k3ch5yc4/width/700/height/500/border/888888/rc/false/ai/false/sdz/true" width="700" height="500" style="border:0px;" allowfullscreen></iframe>
