# MATEMATIKA SMA (JURUSAN IPA & PESANTREN)
## Kelas 11 - Semester Ganjil
### Pertemuan 7: Determinan dan Invers Matriks

---

### 1. Pengertian & Konsep Dasar

Dalam ilmu aljabar linear, setiap matriks persegi (matriks dengan jumlah baris dan kolom yang sama, $n \times n$) memiliki karakteristik skalar khusus yang disebut **determinan**. Determinan mencerminkan sifat geometris dari matriks tersebut, seperti faktor perubahan luas (pada dimensi 2) atau volume (pada dimensi 3).

Secara filosofis dan teologis, keberadaan determinan dan invers matriks mengajarkan kita tentang **keteraturan sunnatullah dan keseimbangan hukum sebab-akibat**. Sebagaimana setiap perbuatan manusia memiliki timbangan nilai yang presisi, setiap matriks persegi memiliki nilai determinan tunggal yang menentukan apakah matriks tersebut dapat "dibalik" (memiliki invers) atau tidak.

**Analogi Kunci dan Gembok Berpasangan:**
- Jika matriks $A$ diibaratkan sebagai proses penguncian (enkripsi pesan logistik santri), maka **invers matriks** $A^{-1}$ adalah anak kunci pembukanya.
- Mengalikan suatu matriks dengan inversnya akan mengembalikan keadaan ke elemen netral (matriks identitas $I$):

$$
A \cdot A^{-1} = A^{-1} \cdot A = I
$$

- Namun, tidak semua gembok memiliki anak kunci. Matriks yang nilai determinannya bernilai nol ($\det A = 0$) disebut **matriks singular** (rusak/kehilangan dimensi), sehingga **mustahil memiliki invers**. Matriks yang memiliki invers hanyalah matriks dengan determinan tidak sama dengan nol ($\det A \neq 0$), yang dinamakan **matriks non-singular**.
- Selain itu, determinan dapat dimanfaatkan secara langsung untuk menyelesaikan **Sistem Persamaan Linear Dua Variabel (SPLDV)** secara cepat tanpa perlu mencari invers matriks, yang dikenal dengan nama **Aturan Cramer (*Cramer's Rule*)**.

---

### 2. Bentuk Umum & Rumus Baku

#### A. Determinan dan Invers Matriks Ordo $2 \times 2$

Diberikan matriks persegi berordo $2 \times 2$:

$$
A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}
$$

1. **Determinan Matriks $2 \times 2$:**

$$
\det(A) = |A| = \begin{vmatrix} a & b \\ c & d \end{vmatrix} = ad - bc
$$

2. **Invers Matriks $2 \times 2$:**

$$
A^{-1} = \frac{1}{\det(A)} \operatorname{Adj}(A) = \frac{1}{ad - bc} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}, \quad \text{dengan syarat } ad - bc \neq 0
$$

**Keterangan Simbol:**
- $\det(A)$ atau $|A|$: Determinan dari matriks $A$ (skalar bilangan real).
- $A^{-1}$: Invers dari matriks $A$.
- $\operatorname{Adj}(A)$: Matriks adjoin dari $A$, diperoleh dengan menukar elemen diagonal utama ($a \leftrightarrow d$) dan menegasikan tanda elemen diagonal samping ($-b$ dan $-c$).
- $I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$: Matriks identitas ordo $2 \times 2$.

---

#### B. Determinan Matriks Ordo $3 \times 3$ (Metode Ekspansi Sarrus)

Diberikan matriks persegi berordo $3 \times 3$:

$$
A = \begin{pmatrix} a & b & c \\ d & e & f \\ g & h & i \end{pmatrix}
$$

Nilai determinan dihitung dengan menyalin dua kolom pertama ke sebelah kanan garis determinan:

$$
\det(A) = \begin{vmatrix} a & b & c \\ d & e & f \\ g & h & i \end{vmatrix} \begin{matrix} a & b \\ d & e \\ g & h \end{matrix}
$$

Perhitungan dilakukan dengan menjumlahkan hasil kali diagonal utama lalu mengurangkannya dengan hasil kali diagonal samping:

$$
\det(A) = (aei + bfg + cdh) - (ceg + afh + bdi)
$$

---

#### C. Invers Matriks Ordo $3 \times 3$ (Metode Matriks Adjoin)

Untuk matriks ordo $3 \times 3$, invers dirumuskan sebagai:

$$
A^{-1} = \frac{1}{\det(A)} \operatorname{Adj}(A), \quad \text{dengan syarat } \det(A) \neq 0
$$

Di mana matriks Adjoin merupakan **transpos dari matriks kofaktor**:

$$
\operatorname{Adj}(A) = (\operatorname{Kof}(A))^T = \begin{pmatrix} C_{11} & C_{21} & C_{31} \\ C_{12} & C_{22} & C_{32} \\ C_{13} & C_{23} & C_{33} \end{pmatrix}
$$

Kofaktor $C_{ij}$ didefinisikan melalui minor $M_{ij}$ (determinan submatriks setelah menghapus baris ke-$i$ dan kolom ke-$j$):

$$
C_{ij} = (-1)^{i+j} M_{ij}
$$

---

#### D. Penyelesaian SPLDV Menggunakan Determinan Saja (Aturan Cramer)

Sistem Persamaan Linear Dua Variabel (SPLDV):

$$
\begin{cases} a_1 x + b_1 y = c_1 \\ a_2 x + b_2 y = c_2 \end{cases}
$$

Dapat diselesaikan secara langsung menggunakan tiga nilai determinan:
1. **Determinan Utama ($D$)**: Determinan dari matriks koefisien variabel $x$ dan $y$:

$$
D = \begin{vmatrix} a_1 & b_1 \\ a_2 & b_2 \end{vmatrix} = a_1 b_2 - a_2 b_1
$$

2. **Determinan Variabel $x$ ($D_x$)**: Kolom koefisien $x$ diganti oleh kolom konstanta ($c_1, c_2$):

$$
D_x = \begin{vmatrix} c_1 & b_1 \\ c_2 & b_2 \end{vmatrix} = c_1 b_2 - c_2 b_1
$$

3. **Determinan Variabel $y$ ($D_y$)**: Kolom koefisien $y$ diganti oleh kolom konstanta ($c_1, c_2$):

$$
D_y = \begin{vmatrix} a_1 & c_1 \\ a_2 & c_2 \end{vmatrix} = a_1 c_2 - a_2 c_1
$$

Nilai variabel $x$ dan $y$ diperoleh secara instan tanpa perlu mencari invers matriks:

$$
x = \frac{D_x}{D} \quad \text{dan} \quad y = \frac{D_y}{D}, \quad \text{dengan syarat } D \neq 0
$$

---

### 3. Sifat-Sifat, Karakteristik, & Aturan Khusus

#### A. Syarat Keberadaan Invers
1. **Matriks Non-Singular**: Matriks persegi $A$ memiliki invers jika dan hanya jika $\det(A) \neq 0$.
2. **Matriks Singular**: Jika $\det(A) = 0$, matriks $A$ tidak memiliki invers karena pembagian dengan nol tidak terdefinisi pada bilangan real ($\frac{1}{0}$).

#### B. Analisis Solusi SPLDV pada Aturan Cramer
- **Solusi Tunggal (Unik)**: Terjadi jika $D \neq 0$. Nilai $x = \frac{D_x}{D}$ dan $y = \frac{D_y}{D}$ bernilai pasti.
- **Tak Hingga Banyak Solusi**: Terjadi jika $D = 0$ dan $D_x = D_y = 0$ (kedua persamaan merepresentasikan garis yang sama/berimpit).
- **Tidak Memiliki Solusi**: Terjadi jika $D = 0$, tetapi minimal salah satu dari $D_x \neq 0$ atau $D_y \neq 0$ (garis saling sejajar).

#### C. Sifat-Sifat Utama Determinan & Invers
Misalkan $A$ dan $B$ adalah matriks persegi berordo $n \times n$ yang memiliki invers, serta $k \in \mathbb{R}$:
1. $\det(A^T) = \det(A)$
2. $\det(A \cdot B) = \det(A) \cdot \det(B)$
3. $\det(A^{-1}) = \frac{1}{\det(A)}$
4. $\det(k \cdot A) = k^n \cdot \det(A)$ (untuk ordo $2 \times 2$, $\det(kA) = k^2 \det A$; untuk ordo $3 \times 3$, $\det(kA) = k^3 \det A$)
5. $(A^{-1})^{-1} = A$
6. $(A \cdot B)^{-1} = B^{-1} \cdot A^{-1}$ *(Urutan perkalian dibalik)*
7. $(A^T)^{-1} = (A^{-1})^T$
8. $A \cdot A^{-1} = A^{-1} \cdot A = I$

#### D. Tabel Komparasi Metode Penyelesaian SPLDV

| Aspek Perbandingan | Metode Invers Matriks | Metode Determinan (Aturan Cramer) |
| :--- | :--- | :--- |
| **Bentuk Rumus** | $X = A^{-1} \cdot B$ | $x = \frac{D_x}{D}, \quad y = \frac{D_y}{D}$ |
| **Langkah Utama** | Hitung $\det A \rightarrow$ cari adjoin $\rightarrow$ kalikan matriks | Hitung 3 determinan $2 \times 2$ ($D, D_x, D_y$) $\rightarrow$ bagi |
| **Kemudahan Hitung** | Memerlukan perkalian dua matriks di akhir | Murni operasi perkalian silang skalar |
| **Kelebihan** | Berguna untuk transformasi sistem aljabar | Lebih cepat, praktis, dan minim risiko salah tanda |

---

### 4. Contoh Soal & Pembahasan Terperinci

#### Contoh 1 (Tingkat Dasar: Determinan & Invers $2 \times 2$)
**Soal:**
Diberikan matriks $A = \begin{pmatrix} 3 & 5 \\ 1 & 2 \end{pmatrix}$.
a. Tentukan nilai determinan matriks $A$.  
b. Tentukan invers dari matriks $A$.  
c. Buktikan secara aljabar bahwa $A \cdot A^{-1} = I$.

**Penyelesaian:**
- **Diketahui:**

$$
A = \begin{pmatrix} 3 & 5 \\ 1 & 2 \end{pmatrix} \implies a = 3, \ b = 5, \ c = 1, \ d = 2
$$

- **Ditanyakan:**
  $\det(A)$, $A^{-1}$, dan pembuktian $A \cdot A^{-1} = I$.
- **Langkah Penyelesaian:**
  1. *Menghitung Determinan:*

$$
\det(A) = ad - bc = (3)(2) - (5)(1) = 6 - 5 = 1
$$

  Karena $\det(A) = 1 \neq 0$, matriks $A$ bersifat non-singular dan memiliki invers.
  2. *Menentukan Invers Matriks:*

$$
A^{-1} = \frac{1}{\det(A)} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix} = \frac{1}{1} \begin{pmatrix} 2 & -5 \\ -1 & 3 \end{pmatrix} = \begin{pmatrix} 2 & -5 \\ -1 & 3 \end{pmatrix}
$$

  3. *Pembuktian Perkalian Matriks:*

$$
\begin{aligned}
A \cdot A^{-1} &= \begin{pmatrix} 3 & 5 \\ 1 & 2 \end{pmatrix} \begin{pmatrix} 2 & -5 \\ -1 & 3 \end{pmatrix} \\
&= \begin{pmatrix} (3)(2) + (5)(-1) & (3)(-5) + (5)(3) \\ (1)(2) + (2)(-1) & (1)(-5) + (2)(3) \end{pmatrix} \\
&= \begin{pmatrix} 6 - 5 & -15 + 15 \\ 2 - 2 & -5 + 6 \end{pmatrix} \\
&= \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = I
\end{aligned}
$$

- **Kesimpulan:** 
  Nilai $\det(A) = 1$, invers $A^{-1} = \begin{pmatrix} 2 & -5 \\ -1 & 3 \end{pmatrix}$, dan terbukti $A \cdot A^{-1} = I$ ($\checkmark\ \text{Benar}$).

---

#### Contoh 2 (Pengembangan: Sarrus $3 \times 3$ & Matriks Singular)
**Soal:**
1. Hitunglah nilai determinan dari matriks $B = \begin{pmatrix} 2 & 1 & 3 \\ 0 & 4 & 2 \\ 1 & 2 & 1 \end{pmatrix}$.  
2. Tentukan nilai $k$ agar matriks $M = \begin{pmatrix} 2k & 6 \\ 3 & 9 \end{pmatrix}$ menjadi matriks singular!

**Penyelesaian:**
- **Diketahui:**

$$
B = \begin{pmatrix} 2 & 1 & 3 \\ 0 & 4 & 2 \\ 1 & 2 & 1 \end{pmatrix}, \quad M = \begin{pmatrix} 2k & 6 \\ 3 & 9 \end{pmatrix}
$$

- **Ditanyakan:**
  $\det(B)$ dan nilai $k$ saat $\det(M) = 0$.
- **Langkah Penyelesaian:**
  1. *Menghitung Determinan Matriks $B$ dengan Aturan Sarrus:*

$$
\det(B) = \begin{vmatrix} 2 & 1 & 3 \\ 0 & 4 & 2 \\ 1 & 2 & 1 \end{vmatrix} \begin{matrix} 2 & 1 \\ 0 & 4 \\ 1 & 2 \end{matrix}
$$

$$
\begin{aligned}
\det(B) &= [(2 \cdot 4 \cdot 1) + (1 \cdot 2 \cdot 1) + (3 \cdot 0 \cdot 2)] - [(3 \cdot 4 \cdot 1) + (2 \cdot 2 \cdot 2) + (1 \cdot 0 \cdot 1)] \\
&= [8 + 2 + 0] - [12 + 8 + 0] \\
&= 10 - 20 = -10
\end{aligned}
$$

  2. *Menentukan Nilai $k$ pada Matriks Singular:*
  Syarat matriks singular: $\det(M) = 0$.

$$
(2k)(9) - (6)(3) = 0 \implies 18k - 18 = 0 \implies 18k = 18 \implies k = 1
$$

- **Kesimpulan:** 
  Nilai determinan matriks $B$ adalah $-10$, dan matriks $M$ menjadi singular ketika $k = 1$ ($\checkmark\ \text{Benar}$).

---

#### Contoh 3 (Penyelesaian SPLDV Murni Menggunakan Determinan / Aturan Cramer)
**Soal:**
Tentukan himpunan penyelesaian dari sistem persamaan linear berikut menggunakan metode determinan saja:

$$
\begin{cases} 3x + 2y = 12 \\ 5x - y = 7 \end{cases}
$$

**Penyelesaian:**
- **Diketahui:**

$$
\begin{aligned}
a_1 = 3, \quad b_1 = 2, \quad c_1 = 12 \\
a_2 = 5, \quad b_2 = -1, \quad c_2 = 7
\end{aligned}
$$

- **Ditanyakan:**
  Nilai $x$ dan $y$ menggunakan Aturan Cramer.
- **Langkah Penyelesaian:**
  1. *Hitung Determinan Utama ($D$):*

$$
D = \begin{vmatrix} 3 & 2 \\ 5 & -1 \end{vmatrix} = (3)(-1) - (2)(5) = -3 - 10 = -13
$$

  2. *Hitung Determinan Variabel $x$ ($D_x$):*

$$
D_x = \begin{vmatrix} 12 & 2 \\ 7 & -1 \end{vmatrix} = (12)(-1) - (2)(7) = -12 - 14 = -26
$$

  3. *Hitung Determinan Variabel $y$ ($D_y$):*

$$
D_y = \begin{vmatrix} 3 & 12 \\ 5 & 7 \end{vmatrix} = (3)(7) - (12)(5) = 21 - 60 = -39
$$

  4. *Menentukan Nilai Variabel:*

$$
x = \frac{D_x}{D} = \frac{-26}{-13} = 2, \quad y = \frac{D_y}{D} = \frac{-39}{-13} = 3
$$

- **Kesimpulan:** 
  Himpunan penyelesaian dari sistem persamaan tersebut adalah $(x, y) = (2, 3)$ ($\checkmark\ \text{Benar}$).

---

### 5. Penerapan Kontekstual (Studi Kasus Santri & Kehidupan Nyata)

#### Kasus Pengadaan Logistik Beras dan Kurma Asrama Santri
> Pengurus logistik dapur umum asrama santri membeli bahan konsumsi untuk persiapan buka puasa sunnah santri dalam dua kali pengadaan:
> - **Pengadaan Tahap I**: Membeli $2\text{ karung}$ beras dan $3\text{ kardus}$ kurma dengan total dana $\text{Rp}420.000$.
> - **Pengadaan Tahap II**: Membeli $3\text{ karung}$ beras dan $4\text{ kardus}$ kurma dengan total dana $\text{Rp}590.000$.
>
> Berapakah harga satuan untuk $1\text{ karung}$ beras dan $1\text{ kardus}$ kurma?

**Langkah Pemecahan:**

1. **Pemodelan Sistem Persamaan:**
   Misalkan:
   - $x$ = harga $1\text{ karung}$ beras (dalam rupiah)
   - $y$ = harga $1\text{ kardus}$ kurma (dalam rupiah)

$$
\begin{cases} 2x + 3y = 420.000 \\ 3x + 4y = 590.000 \end{cases}
$$

2. **Penyelesaian dengan Metode Determinan Saja (Aturan Cramer):**
   - *Determinan Utama ($D$):*

$$
D = \begin{vmatrix} 2 & 3 \\ 3 & 4 \end{vmatrix} = (2)(4) - (3)(3) = 8 - 9 = -1
$$

   - *Determinan Variabel $x$ ($D_x$):*

$$
\begin{aligned}
D_x = \begin{vmatrix} 420.000 & 3 \\ 590.000 & 4 \end{vmatrix} &= (420.000)(4) - (3)(590.000) \\
&= 1.680.000 - 1.770.000 = -90.000
\end{aligned}
$$

   - *Determinan Variabel $y$ ($D_y$):*

$$
\begin{aligned}
D_y = \begin{vmatrix} 2 & 420.000 \\ 3 & 590.000 \end{vmatrix} &= (2)(590.000) - (420.000)(3) \\
&= 1.180.000 - 1.260.000 = -80.000
\end{aligned}
$$

   - *Menghitung Nilai Satuan:*

$$
x = \frac{D_x}{D} = \frac{-90.000}{-1} = 90.000, \quad y = \frac{D_y}{D} = \frac{-80.000}{-1} = 80.000
$$

3. **Perbandingan dengan Metode Invers Matriks ($X = A^{-1} \cdot B$):**

$$
A^{-1} = \frac{1}{-1} \begin{pmatrix} 4 & -3 \\ -3 & 2 \end{pmatrix} = \begin{pmatrix} -4 & 3 \\ 3 & -2 \end{pmatrix}
$$

$$
\begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} -4 & 3 \\ 3 & -2 \end{pmatrix} \begin{pmatrix} 420.000 \\ 590.000 \end{pmatrix} = \begin{pmatrix} 90.000 \\ 80.000 \end{pmatrix}
$$

4. **Jawaban Kontekstual:**
   Kedua metode menghasilkan nilai yang konsisten dan presisi:
   - Harga $1\text{ karung}$ beras adalah $\text{Rp}90.000$.
   - Harga $1\text{ kardus}$ kurma adalah $\text{Rp}80.000$.

---

### 6. Pola Kunci & Cara Cepat Mengingat

- **Jembatan Keledai Invers $2 \times 2$:**
  > *"Tukar posisi diagonal utama, balikkan tanda diagonal samping, lalu bagi seluruhnya dengan determinan."*

$$
\begin{pmatrix} \mathbf{a} & b \\ c & \mathbf{d} \end{pmatrix} \xrightarrow{\text{Adjoin}} \begin{pmatrix} \mathbf{d} & -b \\ -c & \mathbf{a} \end{pmatrix}
$$

- **Jembatan Keledai Aturan Cramer:**
  > *"Ganti kolom variabel yang dicari dengan kolom konstanta, lalu bagi dengan determinan utama."*

$$
x = \frac{D_x}{D}, \quad y = \frac{D_y}{D}
$$

- **Catatan Waspada (Common Pitfalls):**
  - ⚠️ **Lupa Memeriksa Nilai $D$**: Jika $D = 0$, Aturan Cramer tidak dapat membagi nilai. Jangan lanjutkan pembagian dan periksa apakah sistem memiliki tak hingga banyak solusi atau tidak memiliki solusi sama sekali.
  - ⚠️ **Tertukar Kolom Pengganti**: Saat mencari $D_x$, ganti kolom **pertama**. Saat mencari $D_y$, ganti kolom **kedua**. Jangan sampai terbalik menukar kolom.
  - ⚠️ **Kekeliruan Tanda Diagonal Samping**: Elemen diagonal samping ($b$ dan $c$) pada invers matriks **hanya berganti tanda**, bukan berpindah posisi.

---

### 7. Latihan Soal

---

#### Latihan Soal 1: Determinan, Sifat-Sifat, dan Invers Matriks Ordo $2 \times 2$ & $3 \times 3$ (20 Soal)

**A. Pemahaman Konsep & Karakteristik Matriks**
1. Diberikan matriks identitas $I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$. Tunjukkan bahwa determinan matriks identitas bernilai $1$ dan invers dari matriks identitas adalah dirinya sendiri ($I^{-1} = I$)!
2. Jika sebuah matriks persegi berordo $2 \times 2$ memiliki elemen-elemen pada baris pertama yang merupakan kelipatan dari elemen-elemen pada baris kedua, jelaskan mengapa determinan matriks tersebut selalu bernilai nol!
3. Selidikilah apakah matriks $P = \begin{pmatrix} 6 & 9 \\ 4 & 6 \end{pmatrix}$ tergolong matriks singular atau matriks non-singular!
4. Diketahui matriks $A$ berordo $2 \times 2$ dengan $\det(A) = 5$. Berdasarkan sifat-sifat determinan, tentukan nilai dari $\det(A^T)$ dan $\det(A^{-1})$!

**B. Operasi Hitung Determinan & Invers**  
*(Petunjuk: Hitunglah hasil akhir dari setiap operasi matriks berikut)*
5. $\begin{vmatrix} 7 & 4 \\ 3 & 2 \end{vmatrix}$
6. $\begin{vmatrix} -5 & 6 \\ -2 & 4 \end{vmatrix}$
7. $\begin{vmatrix} 12 & -8 \\ -3 & 2 \end{vmatrix}$
8. Invers dari matriks $A = \begin{pmatrix} 5 & 7 \\ 2 & 3 \end{pmatrix}$
9. Invers dari matriks $B = \begin{pmatrix} 4 & -2 \\ -3 & 1 \end{pmatrix}$
10. Invers dari matriks $C = \begin{pmatrix} -6 & 5 \\ -7 & 6 \end{pmatrix}$
11. $\begin{vmatrix} 1 & 2 & 3 \\ 2 & 1 & 4 \\ 1 & 0 & 2 \end{vmatrix}$ dengan aturan Sarrus.
12. $\begin{vmatrix} 3 & -1 & 2 \\ 4 & 0 & 5 \\ -2 & 1 & 3 \end{vmatrix}$ dengan aturan Sarrus.
13. Nilai $x$ yang memenuhi persamaan determinan $\begin{vmatrix} 2x & 5 \\ 4 & x \end{vmatrix} = 2$.
14. Nilai $p$ agar matriks $K = \begin{pmatrix} p+2 & 4 \\ 3 & p-2 \end{pmatrix}$ menjadi matriks singular.

**C. Sifat Aljabar Matriks Lanjutan**
15. Diberikan matriks $A = \begin{pmatrix} 2 & 1 \\ 3 & 4 \end{pmatrix}$ dan $B = \begin{pmatrix} 1 & 2 \\ 0 & 3 \end{pmatrix}$. Tentukan nilai dari $\det(A \cdot B)$ tanpa mengalikan matriks $A$ dan $B$ terlebih dahulu!
16. Diberikan matriks $M$ berordo $2 \times 2$ dengan $\det(M) = 4$. Tentukan nilai dari $\det(3M)$!
17. Diberikan matriks $P$ berordo $3 \times 3$ dengan $\det(P) = 2$. Tentukan nilai dari $\det(2P)$!
18. Diberikan persamaan matriks $A \cdot X = B$. Jika $A = \begin{pmatrix} 3 & 1 \\ 5 & 2 \end{pmatrix}$ dan $B = \begin{pmatrix} 4 \\ 7 \end{pmatrix}$, tentukan matriks kolom $X = \begin{pmatrix} x \\ y \end{pmatrix}$!
19. Selesaikan persamaan matriks $X \cdot A = B$ untuk menentukan matriks baris $X = \begin{pmatrix} x & y \end{pmatrix}$, jika diketahui $A = \begin{pmatrix} 4 & 3 \\ 1 & 1 \end{pmatrix}$ dan $B = \begin{pmatrix} 7 & 5 \end{pmatrix}$!
20. Diketahui matriks $P = \begin{pmatrix} 2 & 3 \\ 1 & 2 \end{pmatrix}$ dan $Q = \begin{pmatrix} 1 & 4 \\ 2 & 9 \end{pmatrix}$. Tentukan invers dari perkalian matriks $(P \cdot Q)^{-1}$ dengan sifat $(P \cdot Q)^{-1} = Q^{-1} \cdot P^{-1}$!

---

#### Latihan Soal 2: Penyelesaian SPLDV Menggunakan Determinan (Aturan Cramer) & Matriks Invers (20 Soal)

**A. Pemahaman Konsep Aturan Cramer**
1. Tuliskan rumus menentukan nilai $x$ dan $y$ pada SPLDV $\begin{cases} a_1 x + b_1 y = c_1 \\ a_2 x + b_2 y = c_2 \end{cases}$ menggunakan konsep determinan $D, D_x,$ dan $D_y$!
2. Jelaskan syarat mutlak nilai determinan utama ($D$) agar Aturan Cramer dapat digunakan untuk menemukan solusi tunggal!
3. Jika pada suatu sistem persamaan linear diperoleh $D = 0$, $D_x = 0$, dan $D_y = 0$, jelaskan tafsiran geometris dari kedua garis persamaan tersebut!
4. Jika pada suatu SPLDV diperoleh $D = 0$ tetapi $D_x = 14$ dan $D_y = -8$, tentukan himpunan penyelesaian dari SPLDV tersebut!

**B. Operasi Hitung SPLDV dengan Aturan Cramer**  
*(Petunjuk: Hitunglah nilai $D, D_x, D_y$ serta himpunan penyelesaian $(x, y)$ untuk setiap SPLDV berikut)*
5. $\begin{cases} 2x + y = 7 \\ 3x - 2y = 7 \end{cases}$
6. $\begin{cases} 4x + 3y = 18 \\ 2x - y = 4 \end{cases}$
7. $\begin{cases} 5x + 2y = 19 \\ 3x + 4y = 17 \end{cases}$
8. $\begin{cases} 3x - 5y = 1 \\ 2x + 3y = 7 \end{cases}$
9. $\begin{cases} 7x + 2y = -1 \\ 3x - 4y = 19 \end{cases}$
10. $\begin{cases} 6x - 5y = 9 \\ 4x + 3y = 25 \end{cases}$
11. $\begin{cases} -2x + 7y = 29 \\ 3x + 4y = 15 \end{cases}$
12. $\begin{cases} 8x + 5y = 2 \\ 3x + 2y = 1 \end{cases}$
13. $\begin{cases} 9x - 4y = 17 \\ 3x + 2y = 9 \end{cases}$
14. $\begin{cases} 5x - 6y = -22 \\ 2x + 3y = 11 \end{cases}$

**C. Penerapan Matriks Invers & Variasi SPLDV**
15. Selesaikan sistem persamaan $\begin{cases} 3x + 4y = 11 \\ 2x + 3y = 8 \end{cases}$ menggunakan metode matriks invers $X = A^{-1} \cdot B$!
16. Selesaikan sistem persamaan $\begin{cases} 5x + 7y = 3 \\ 2x + 3y = 1 \end{cases}$ menggunakan metode matriks invers $X = A^{-1} \cdot B$!
17. Diberikan sistem persamaan $\begin{cases} \frac{2}{a} + \frac{3}{b} = 13 \\ \frac{5}{a} - \frac{1}{b} = 7 \end{cases}$. Dengan memisalkan $x = \frac{1}{a}$ dan $y = \frac{1}{b}$, tentukan nilai $a$ dan $b$ menggunakan Aturan Cramer!
18. Diberikan sistem persamaan linear yang memuat pecahan: $\begin{cases} \frac{x+1}{2} - \frac{y-2}{3} = 3 \\ \frac{x-1}{3} + \frac{y+1}{2} = 4 \end{cases}$. Ubah ke dalam bentuk baku aljabar lalu selesaikan dengan metode determinan!
19. Tentukan nilai $k$ agar sistem persamaan $\begin{cases} kx + 4y = 8 \\ 3x + 6y = 12 \end{cases}$ memiliki tak hingga banyak penyelesaian!
20. Tentukan nilai $m$ agar sistem persamaan linear $\begin{cases} (m-1)x + 2y = 5 \\ 4x + my = 3 \end{cases}$ tidak memiliki solusi penyelesaian!

---

#### Latihan Soal 3: Penerapan Kontekstual Santri & Pemecahan Masalah Nyata Pesantren (20 Soal)

*(Petunjuk: Selesaikan setiap soal cerita berikut dengan menyusun model matriks dan menggunakan metode Determinan Cramer atau Matriks Invers)*

1. Santri bagian logistik dapur umum asrama membeli bahan sarapan santri:
   - Pembelian I: $4\text{ kg}$ telur ayam dan $5\text{ papan}$ tempe seharga $\text{Rp}142.000$.
   - Pembelian II: $3\text{ kg}$ telur ayam dan $2\text{ papan}$ tempe seharga $\text{Rp}85.000$.  
   Tentukan harga satuan $1\text{ kg}$ telur ayam dan $1\text{ papan}$ tempe!
2. Santri pengurus perpustakaan pondok membeli dua jenis kitab referensi:
   - Paket A: $3\text{ jilid}$ kamus bahasa Arab dan $2\text{ jilid}$ kitab fiqih seharga $\text{Rp}240.000$.
   - Paket B: $2\text{ jilid}$ kamus bahasa Arab dan $1\text{ jilid}$ kitab fiqih seharga $\text{Rp}150.000$.  
   Tentukan harga $1\text{ jilid}$ kamus bahasa Arab dan $1\text{ jilid}$ kitab fiqih!
3. Pengurus pos kesehatan pesantren membeli persediaan obat herbal santri:
   - Pembelian I: $3\text{ botol}$ minyak habbatussauda dan $2\text{ botol}$ madu murni seharga $\text{Rp}190.000$.
   - Pembelian II: $4\text{ botol}$ minyak habbatussauda dan $3\text{ botol}$ madu murni seharga $\text{Rp}265.000$.  
   Tentukan harga satuan $1\text{ botol}$ minyak habbatussauda dan $1\text{ botol}$ madu murni!
4. Santri bagian sarana asrama membeli perlengkapan kebersihan kamar mandi:
   - Pembelian I: $5\text{ buah}$ ember dan $4\text{ buah}$ gayung air dengan total biaya $\text{Rp}130.000$.
   - Pembelian II: $3\text{ buah}$ ember dan $2\text{ buah}$ gayung air dengan total biaya $\text{Rp}74.000$.  
   Tentukan harga satuan $1\text{ buah}$ ember dan $1\text{ buah}$ gayung air!
5. Pengurus asrama membagikan perlengkapan salat bagi santri baru:
   - Paket I: $3\text{ helai}$ baju koko putih dan $2\text{ helai}$ sarung tenun seharga $\text{Rp}310.000$.
   - Paket II: $2\text{ helai}$ baju koko putih dan $4\text{ helai}$ sarung tenun seharga $\text{Rp}340.000$.  
   Tentukan harga $1\text{ helai}$ baju koko putih dan $1\text{ helai}$ sarung tenun!
6. Toko Kitab Pesantren menyediakan paket kitab saku santri:
   - Paket A: $2\text{ buku}$ doa pagi-petang dan $3\text{ buku}$ zikir salat seharga $\text{Rp}34.000$.
   - Paket B: $3\text{ buku}$ doa pagi-petang dan $4\text{ buku}$ zikir salat seharga $\text{Rp}48.000$.  
   Tentukan harga $1\text{ buku}$ doa pagi-petang dan $1\text{ buku}$ zikir salat!
7. Pengurus asrama membeli lampu penerangan hemat energi untuk ruang belajar:
   - Pembelian I: $6\text{ buah}$ lampu LED $10\text{ Watt}$ dan $4\text{ buah}$ lampu LED $18\text{ Watt}$ seharga $\text{Rp}210.000$.
   - Pembelian II: $4\text{ buah}$ lampu LED $10\text{ Watt}$ dan $5\text{ buah}$ lampu LED $18\text{ Watt}$ seharga $\text{Rp}215.000$.  
   Tentukan harga satuan masing-masing lampu LED tersebut!
8. Santri marbot masjid pondok membeli perlengkapan wangi-wangian dan kebersihan:
   - Pembelian I: $4\text{ botol}$ sabun cair cuci tangan dan $3\text{ botol}$ pewangi karpet seharga $\text{Rp}145.000$.
   - Pembelian II: $2\text{ botol}$ sabun cair cuci tangan dan $5\text{ botol}$ pewangi karpet seharga $\text{Rp}165.000$.  
   Tentukan harga $1\text{ botol}$ sabun cuci tangan dan $1\text{ botol}$ pewangi karpet!
9. Panitia takjil puasa sunnah santri menyiapkan buah segar hidangan berbuka:
   - Pembelian I: $5\text{ butir}$ semangka dan $4\text{ butir}$ melon seharga $\text{Rp}155.000$.
   - Pembelian II: $3\text{ butir}$ semangka dan $6\text{ butir}$ melon seharga $\text{Rp}165.000$.  
   Tentukan harga $1\text{ butir}$ semangka dan $1\text{ butir}$ melon!
10. Pengurus kamar santri membeli perlengkapan tidur dan salat:
    - Pembelian I: $2\text{ lembar}$ sajadah busa dan $3\text{ buah}$ bantal tidur seharga $\text{Rp}230.000$.
    - Pembelian II: $4\text{ lembar}$ sajadah busa dan $1\text{ buah}$ bantal tidur seharga $\text{Rp}310.000$.  
    - Tentukan harga $1\text{ lembar}$ sajadah busa dan $1\text{ buah}$ bantal tidur!
11. Bagian pengajaran kelas tahfiz membeli alat tulis guru:
    - Pembelian I: $5\text{ kotak}$ spidol papan tulis dan $3\text{ buah}$ penghapus magnet seharga $\text{Rp}135.000$.
    - Pembelian II: $3\text{ kotak}$ spidol papan tulis dan $4\text{ buah}$ penghapus magnet seharga $\text{Rp}103.000$.  
    - Tentukan harga $1\text{ kotak}$ spidol dan $1\text{ buah}$ penghapus!
12. Toko Kitab Pesantren menjual mushaf Al-Qur'an dan buku tajwid:
    - Paket Barokah: $4\text{ mushaf}$ Al-Qur'an dan $5\text{ buku}$ kaidah tajwid praktis seharga $\text{Rp}325.000$.
    - Paket Hidayah: $2\text{ mushaf}$ Al-Qur'an dan $3\text{ buku}$ kaidah tajwid praktis seharga $\text{Rp}175.000$.  
    - Tentukan harga $1\text{ mushaf}$ Al-Qur'an dan $1\text{ buku}$ kaidah tajwid!
13. Santri bagian rumah tangga asrama membeli perlengkapan minum santri:
    - Pembelian I: $2\text{ unit}$ dispenser air galon dan $3\text{ buah}$ teko air stainless seharga $\text{Rp}380.000$.
    - Pembelian II: $1\text{ unit}$ dispenser air galon dan $4\text{ buah}$ teko air stainless seharga $\text{Rp}290.000$.  
    - Tentukan harga $1\text{ unit}$ dispenser air galon dan $1\text{ buah}$ teko air stainless!
14. Unit wirausaha santri budidaya ikan lele membeli bibit dan pakan:
    - Tahap I: $1.000\text{ ekor}$ benih lele dan $2\text{ sak}$ pakan pelet seharga $\text{Rp}340.000$.
    - Tahap II: $2.000\text{ ekor}$ benih lele dan $3\text{ sak}$ pakan pelet seharga $\text{Rp}560.000$.  
    - Tentukan harga $1.000\text{ ekor}$ benih lele dan $1\text{ sak}$ pakan pelet!
15. Pengurus kebun pondok membeli bibit pohon buah berkah:
    - Pembelian I: $3\text{ bibit}$ pohon tin dan $2\text{ bibit}$ pohon kurma seharga $\text{Rp}270.000$.
    - Pembelian II: $2\text{ bibit}$ pohon tin dan $4\text{ bibit}$ pohon kurma seharga $\text{Rp}420.000$.  
    - Tentukan harga $1\text{ bibit}$ pohon tin dan $1\text{ bibit}$ pohon kurma!
16. Dapur umum pondok membeli bahan rempah-rempah bumbu masak:
    - Pembelian I: $4\text{ kg}$ bawang merah dan $3\text{ kg}$ bawang putih seharga $\text{Rp}220.000$.
    - Pembelian II: $2\text{ kg}$ bawang merah dan $5\text{ kg}$ bawang putih seharga $\text{Rp}220.000$.  
    - Tentukan harga $1\text{ kg}$ bawang merah dan $1\text{ kg}$ bawang putih!
17. Pengurus asrama memesan mebel perlengkapan belajar santri:
    - Pesanan I: $3\text{ unit}$ meja belajar lipat dan $2\text{ unit}$ rak buku gantung seharga $\text{Rp}260.000$.
    - Pesanan II: $4\text{ unit}$ meja belajar lipat dan $3\text{ unit}$ rak buku gantung seharga $\text{Rp}365.000$.  
    - Tentukan harga $1\text{ unit}$ meja belajar lipat dan $1\text{ unit}$ rak buku gantung!
18. Santri piket pengingat waktu salat membeli jam dinding dan jadwal salat:
    - Pembelian I: $2\text{ unit}$ jam dinding digital azan dan $3\text{ buah}$ kalender hijriah dinding seharga $\text{Rp}460.000$.
    - Pembelian II: $1\text{ unit}$ jam dinding digital azan dan $4\text{ buah}$ kalender hijriah dinding seharga $\text{Rp}280.000$.  
    - Tentukan harga satuan $1\text{ unit}$ jam digital azan dan $1\text{ buah}$ kalender hijriah dinding!
19. Panitia manasik haji santri membeli perlengkapan peragaan:
    - Pembelian I: $5\text{ set}$ kain ihram santri dan $4\text{ buah}$ sabuk haji seharga $\text{Rp}460.000$.
    - Pembelian II: $3\text{ set}$ kain ihram santri dan $2\text{ buah}$ sabuk haji seharga $\text{Rp}260.000$.  
    - Tentukan harga $1\text{ set}$ kain ihram dan $1\text{ buah}$ sabuk haji!
20. Santri panitia kajian majelis taklim membeli mikrofon nirkabel dan kabel cadangan:
    - Pembelian I: $2\text{ set}$ mikrofon nirkabel dan $3\text{ gulung}$ kabel audio seharga $\text{Rp}540.000$.
    - Pembelian II: $1\text{ set}$ mikrofon nirkabel dan $4\text{ gulung}$ kabel audio seharga $\text{Rp}370.000$.  
    - Tentukan harga $1\text{ set}$ mikrofon nirkabel dan $1\text{ gulung}$ kabel audio!

---

### 8. Pekerjaan Rumah (PR Pondok / Mandiri)

**Petunjuk Pengerjaan:**
- Kerjakan di buku catatan tugas matematika secara mandiri, runtut, dan rapi.
- Tuliskan apa yang diketahui, rumus matriks yang digunakan, serta langkah penyelesaian baris demi baris.

1. Tentukan determinan dan invers dari matriks $A = \begin{pmatrix} 6 & 8 \\ 2 & 3 \end{pmatrix}$, kemudian buktikan bahwa $A \cdot A^{-1} = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$!
2. Selesaikan sistem persamaan linear berikut murni menggunakan Aturan Determinan Cramer:

$$
\begin{cases} 4x - 3y = 17 \\ 2x + 5y = 2 \end{cases}
$$

3. **Soal Kontekstual Aktivitas Pondok Pesantren:**  
   Pengurus pos kesehatan pesantren membeli dua jenis obat herbal untuk persediaan santri:
   - Pembelian I: $3\text{ botol}$ minyak habbatussauda dan $2\text{ botol}$ madu murni seharga $\text{Rp}190.000$.
   - Pembelian II: $4\text{ botol}$ minyak habbatussauda dan $3\text{ botol}$ madu murni seharga $\text{Rp}265.000$.  
   - Susunlah pemodelan matematika masalah di atas ke dalam SPLDV!  
   - Tentukan nilai $D, D_x,$ dan $D_y$!  
   - Hitunglah harga satuan untuk $1\text{ botol}$ minyak habbatussauda dan $1\text{ botol}$ madu murni dengan Aturan Cramer!
4. **Pertanyaan Pemahaman Konsep:**  
   *Jelaskan dengan kata-katamu sendiri: Mengapa metode determinan (Aturan Cramer) sering kali dianggap lebih praktis dan cepat dibandingkan metode matriks invers dalam menyelesaikan sistem persamaan linear dua variabel? Berikan satu contoh analisis langkah perhitungannya!*

---

### 9. Ringkasan Materi

- **Determinan Matriks Persegi**: Determinan ordo $2 \times 2$ dirumuskan dengan selisih kali silang diagonal $\det(A) = ad - bc$. Untuk ordo $3 \times 3$, determinan dihitung menggunakan aturan perkalian diagonal Sarrus.
- **Invers Matriks Ordo $2 \times 2$**: Dirumuskan sebagai $A^{-1} = \frac{1}{\det(A)} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}$, yang hanya terdefinisi jika matriks bersifat non-singular ($\det(A) \neq 0$).
- **Matriks Singular**: Matriks persegi dengan determinan nol ($\det(A) = 0$). Matriks singular tidak memiliki invers karena pembagian dengan nol tidak terdefinisi.
- **Penyelesaian SPLDV dengan Determinan (Aturan Cramer)**: Sistem $\begin{cases} a_1 x + b_1 y = c_1 \\ a_2 x + b_2 y = c_2 \end{cases}$ dapat diselesaikan secara instan melalui perbandingan nilai determinan: $x = \frac{D_x}{D}$ dan $y = \frac{D_y}{D}$ (dengan syarat $D \neq 0$), di mana $D_x$ dan $D_y$ dibentuk dengan menukar kolom variabel terkait menggunakan kolom konstanta.
