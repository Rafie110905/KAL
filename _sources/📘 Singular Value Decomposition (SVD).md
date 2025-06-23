---
title: "\U0001F4D8 Singular Value Decomposition (SVD)"

---

# 📘 SVD (Singular Value Decomposition) — Ringkasan Lengkap

---

## 🔷 1. Apa itu SVD?

**Singular Value Decomposition (SVD)** adalah suatu teknik dalam aljabar linear yang memfaktorkan sebuah matriks real $A$ berukuran $m \times n$ menjadi tiga matriks:

$$
A = U \cdot \Sigma \cdot V^T
$$

dengan:
- $U$: matriks ortonormal berukuran $m \times m$ (kolom-kolomnya adalah **left singular vectors**)
- $\Sigma$: matriks diagonal berukuran $m \times n$ (berisi **singular values** — nilai non-negatif yang diurut menurun)
- $V^T$: transpose dari matriks ortonormal $V$ berukuran $n \times n$ (baris-barisnya adalah **right singular vectors**)

---

## 💡 2. Kegunaan SVD

SVD memiliki banyak aplikasi penting di berbagai bidang:

- 🧠 **Machine Learning**: reduksi dimensi (PCA), klasifikasi
- 📊 **Data Compression**: kompresi gambar, teks, suara
- 🧹 **Noise Removal**: menyaring noise dari sinyal atau data
- 📈 **Sistem Rekomendasi**: seperti YouTube, Netflix
- 📷 **Image Reconstruction**: rekonstruksi gambar dari fitur utama
- 🧮 **Solusi sistem persamaan** menggunakan pseudo-inverse

---

## 🧼 3. Noise Removal dengan SVD

Caranya:
1. Hitung $A = U \Sigma V^T$
2. Ambil hanya beberapa singular values terbesar (misalnya top-$k$ nilai dalam $\Sigma$)
3. Buat kembali matriks aproksimasi $A_k = U_k \Sigma_k V_k^T$
4. Hasilnya adalah versi **denoised** dari $A$

---

## 📦 4. Topik Pemodelan Menggunakan SVD

Beberapa topik dalam pemodelan yang bisa menggunakan SVD:
- **Model reduksi dimensi** (PCA)
- **Model pembobotan fitur penting**
- **Model penghapusan noise / dekomposisi sinyal**
- **Model sistem rekomendasi berbasis matrix factorization**
- **Latent Semantic Indexing (LSI)** untuk pemodelan teks

---

## 🧮 5. Cara Mencari Matriks $U$, $\Sigma$, dan $V^T$

1. Hitung $A^T A$
2. Hitung **eigenvalue dan eigenvector** dari $A^T A$
3. Ambil akar dari eigenvalue sebagai **singular values**
4. Eigenvector $v_i$ menjadi kolom-kolom dari $V$
5. Hitung:
   $$
   u_i = \frac{1}{\sigma_i} A v_i
   $$
   untuk mendapatkan kolom-kolom $U$
6. Susun $\Sigma$ dari $\sigma_i$

---

## 🧠 6. Rumus Mencari $V$ dari $A^T A$

Dapatkan eigenvector dan eigenvalue dari matriks:

$$
A^T A v = \lambda v
$$

Vektor $v$ adalah kolom dari $V$ dan $\lambda$ adalah nilai kuadrat dari singular values $\sigma$.

---

## ✅ 7. Contoh SVD Matriks 2x2

Diberikan:

$$
A = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}
$$

Langkah-langkah:
- Hitung $A^T A = \begin{bmatrix} 10 & 6 \\ 6 & 10 \end{bmatrix}$
- Eigenvalue: $\lambda_1 = 16$, $\lambda_2 = 4$
- Singular values: $\sigma_1 = 4$, $\sigma_2 = 2$
- Eigenvector $v_1 = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}$, $v_2 = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix}$
- Matriks $V^T$:
  $$
  \begin{bmatrix}
  \frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
  \frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
  \end{bmatrix}
  $$

Hitung $U$ dari:
$$
u_i = \frac{1}{\sigma_i} A v_i
$$

Hasil:
$$
U = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}
$$

Dan $\Sigma = \begin{bmatrix} 4 & 0 \\ 0 & 2 \end{bmatrix}$

---

## 🔁 8. Apakah $U \Sigma V^T = A$?

✅ **Ya**, jika kita hitung:

$$
A = U \cdot \Sigma \cdot V^T
$$

dengan hasil $U$, $\Sigma$, dan $V^T$ dari proses SVD yang tepat, maka kita akan mendapatkan kembali matriks $A$ yang asli.

---

## 🧮 9. Contoh SVD Matriks 3x2

Diberikan:

$$
A = \begin{bmatrix}
4 & 2 \\
2 & 7 \\
1 & 4
\end{bmatrix}
$$

Langkah-langkah:

- Hitung $A^T A = \begin{bmatrix} 21 & 28 \\ 28 & 69 \end{bmatrix}$

- Eigenvalue: $\lambda_1 \approx 81.84$, $\lambda_2 \approx 8.16$

- Singular values: $\sigma_1 \approx 9.04$, $\sigma_2 \approx 2.86$

- Matriks $\Sigma = \begin{bmatrix} 9.04 & 0 \\ 0 & 2.86 \\ 0 & 0 \end{bmatrix}$

- Matriks $V^T \approx \begin{bmatrix} 0.37 & 0.93 \\ -0.93 & 0.37 \end{bmatrix}$

- Hitung $U$ dari $u_i = \frac{1}{\sigma_i} A v_i$

Hasil:
$$
U \approx \begin{bmatrix}
0.35 & -0.63 & \cdots \\
0.71 & 0.07 & \cdots \\
0.61 & 0.77 & \cdots
\end{bmatrix}
$$

---

> 🧠 Dengan SVD, kita bisa memecah matriks menjadi bagian-bagian fundamentalnya, mengisolasi komponen penting, dan membuang gangguan atau data tak relevan.
