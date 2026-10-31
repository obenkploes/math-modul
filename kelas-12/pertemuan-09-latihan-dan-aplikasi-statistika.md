# MATEMATIKA SMA (JURUSAN IPA & PESANTREN)
## Kelas 12 - Semester Ganjil
### Pertemuan 9: Statistika Deskriptif Terpadu — Latihan & Aplikasi Analisis Data Riil Santri

---

### 1. Pengertian & Konsep Dasar

Statistika deskriptif adalah cabang statistika yang bertujuan untuk menghimpun, menyusun, menyajikan, dan menganalisis data numerik sehingga mampu memberikan gambaran ringkas, objektif, dan bermakna mengenai karakteristik suatu populasi atau sampel.

Dalam pembelajaran sebelumnya, kita telah mempelajari komponen-komponen statistika secara parsial:
1. **Penyajian Data**: Tabel distribusi frekuensi, histogram, poligon frekuensi, dan kurva ogive.
2. **Ukuran Pemusatan Data**: Nilai rata-rata hitung (*Mean* $\bar{x}$), nilai tengah (*Median* $Me$), dan nilai yang paling sering muncul (*Modus* $Mo$).
3. **Ukuran Letak Data**: Nilai pembagi posisi sekumpulan data terurut, meliputi Kuartil ($Q_1, Q_2, Q_3$), Desil ($D_1, \dots, D_9$), dan Persentil ($P_1, \dots, P_{99}$).
4. **Ukuran Penyebaran Data**: Tingkat variabilitas atau derajat keragaman data di sekitar nilai pusatnya, meliputi Jangkauan ($R$), Jangkauan Antarkuartil ($H$), Simpangan Kuartil ($Q_d$), Simpangan Rata-rata ($SR$), Ragam ($S^2$), dan Simpangan Baku ($S$).

Pada **Pertemuan 9** ini, seluruh kompetensi tersebut disatukan dalam **satu kesatuan analisis terpadu (*Integrated Data Analysis*)**. Mengetahui nilai rata-rata (*mean*) saja tidak pernah cukup untuk menilai performa suatu kelompok. Dua kelas tahfiz bisa saja memiliki rata-rata hafalan yang sama, namun kelas yang satu memiliki sebaran hafalan yang sangat homogen (seluruh santri rata hafalannya), sedangkan kelas lainnya sangat timpang (ada yang sudah khatam, namun ada yang tertinggal jauh). Oleh karena itu, analisis data yang shahih menuntut integrasi antara **pusat, letak, dan sebaran data**.

Secara filosofis dan teologis Islam, statistika terpadu mengajarkan kita tentang **kejujuran hisab, objektivitas data, dan keadilan evaluasi**. Allah SWT berfirman:

> *"Dan diletakkanlah kitab (catatan amal), lalu engkau akan melihat orang yang bersalah merasa ketakutan terhadap apa yang (tertulis) di dalamnya, dan mereka berkata: 'Aduhai celaka kami, kitab apakah ini yang tidak meninggalkan yang kecil dan tidak (pula) yang besar, melainkan mencatat semuanya secara teliti' ..."*  
> **(QS. Al-Kahfi: 49)**

Setiap data mewakili ikhtiar nyata santri yang harus dihisab secara akurat tanpa manipulasi, sehingga kebijakan pembinaan di pondok pesantren dapat diambil secara adil dan tepat sasaran.

---

### 2. Bentuk Umum & Rumus Baku Terpadu

#### A. Peta Formula Statistika Deskriptif Data Berkelompok

Untuk data berkelompok yang disajikan dalam tabel distribusi frekuensi dengan $k$ kelas interval dan total frekuensi $n = \sum_{i=1}^k f_i$:

1. **Aturan Pembentukan Kelas (Sturges):**

$$
k = 1 + 3{,}3 \log n \quad \text{dan} \quad p = \frac{R}{k} = \frac{X_{\max} - X_{\min}}{k}
$$

2. **Ukuran Pemusatan:**
   - **Rata-rata Hitung (*Mean*):**

$$
\bar{x} = \frac{\sum_{i=1}^k f_i x_i}{\sum_{i=1}^k f_i} \quad (x_i = \text{titik tengah kelas ke-}i)
$$

   - **Median ($Me$):**

$$
Me = L_{me} + \left( \frac{\frac{1}{2}n - \sum f_{k,me}}{f_{me}} \right) p
$$

   - **Modus ($Mo$):**

$$
Mo = L_{mo} + \left( \frac{d_1}{d_1 + d_2} \right) p
$$

3. **Ukuran Letak (Fraktil Data Berkelompok):**
   - **Kuartil ke-$i$ ($Q_i$ untuk $i = 1, 2, 3$):**

$$
Q_i = L_{Q_i} + \left( \frac{\frac{i}{4}n - \sum f_{k,Q_i}}{f_{Q_i}} \right) p
$$

   - **Desil ke-$i$ ($D_i$ untuk $i = 1, 2, \dots, 9$):**

$$
D_i = L_{D_i} + \left( \frac{\frac{i}{10}n - \sum f_{k,D_i}}{f_{D_i}} \right) p
$$

   - **Persentil ke-$i$ ($P_i$ untuk $i = 1, 2, \dots, 99$):**

$$
P_i = L_{P_i} + \left( \frac{\frac{i}{100}n - \sum f_{k,P_i}}{f_{P_i}} \right) p
$$

4. **Ukuran Penyebaran:**
   - **Simpangan Rata-rata ($SR$):**

$$
SR = \frac{\sum_{i=1}^k f_i \lvert x_i - \bar{x} \rvert}{\sum_{i=1}^k f_i}
$$

   - **Ragam / Varians ($S^2$) dan Simpangan Baku ($S$):**

$$
S^2 = \frac{\sum_{i=1}^k f_i (x_i - \bar{x})^2}{\sum_{i=1}^k f_i} \implies S = \sqrt{S^2}
$$

---

#### B. Parameter Komparasi Relatif

Ketika membandingkan dua kelompok data yang memiliki satuan berbeda (misalnya: membandingkan berat badan santri dalam kg dengan tinggi badan dalam cm) atau kelompok dengan nilai rata-rata yang terpaut jauh, perbandingan simpangan baku absolut ($S$) tidak lagi adil. Oleh karena itu, digunakan parameter relatif:

1. **Angka Baku (*Standardized Score / Z-Score*):**  
   Mengukur seberapa jauh deviasi suatu data individu ($x$) dari rata-rata kelompoknya dalam satuan simpangan baku:

$$
Z = \frac{x - \bar{x}}{S}
$$

   - Jika $Z \gt 0$, santri berada di atas rata-rata kelompok.
   - Jika $Z = 0$, santri tepat berada pada rata-rata kelompok.
   - Jika $Z \lt 0$, santri berada di bawah rata-rata kelompok.

2. **Koefisien Variasi ($KV$):**  
   Persentase perbandingan antara simpangan baku dengan nilai rata-rata hitungnya, digunakan untuk mengukur tingkat homogenitas relatif:

$$
KV = \frac{S}{\bar{x}} \times 100\%
$$

   - **Semakin kecil nilai $KV$**, semakin homogen (konsisten/merata) data kelompok tersebut.
   - **Semakin besar nilai $KV$**, semakin heterogen (bervariasi/timpang) data kelompok tersebut.

---

### 3. Sifat-Sifat, Karakteristik, & Aturan Khusus

#### A. Identifikasi Bentuk Kemiringan Kurva (*Skewness*)

Hubungan antara posisi Mean ($\bar{x}$), Median ($Me$), dan Modus ($Mo$) menentukan bentuk kurva distribusi frekuensi:

| Bentuk Distribusi | Hubungan Nilai | Karakteristik Persebaran Data Santri |
| :--- | :---: | :--- |
| **Simetris (Normal)** | $\bar{x} = Me = Mo$ | Data tersebar seimbang di kanan dan kiri nilai rata-rata. Prestasi santri terdistribusi ideal. |
| **Miring ke Kanan (*Positively Skewed*)** | $Mo \lt Me \lt \bar{x}$ | Ekor kurva menjulur ke kanan. Sebagian besar santri memperoleh skor rendah/sedang, hanya sedikit santri yang meraih skor sangat tinggi. |
| **Miring ke Kiri (*Negatively Skewed*)** | $\bar{x} \lt Me \lt Mo$ | Ekor kurva menjulur ke kiri. Sebagian besar santri memperoleh skor tinggi, hanya sedikit santri yang tertinggal di skor rendah. |

#### B. Matriks Pemilihan Ukuran Statistik Sesuai Kondisi Data

| Kondisi Data Riil | Ukuran Pemusatan Terbaik | Ukuran Penyebaran Terbaik | Alasan Metodologis |
| :--- | :---: | :---: | :--- |
| **Data Normal / Simetris (Tanpa Pencilan)** | Mean ($\bar{x}$) | Simpangan Baku ($S$) | Memperhitungkan seluruh nilai data secara matematis. |
| **Data Miring / Terdapat Pencilan (*Outlier*)** | Median ($Me$) | Simpangan Kuartil ($Q_d$) | Resisten terhadap nilai ekstrem yang dapat mendistorsi rata-rata. |
| **Data Kategori / Nominal (Moda Dominan)** | Modus ($Mo$) | Jangkauan ($R$) | Mengetahui kelompok mayoritas atau preferensi dominan. |
| **Komparasi 2 Kelompok Beda Rata-rata/Satuan** | Relative Mean | Koefisien Variasi ($KV$) | Membandingkan dispersi relatif secara proporsional. |

---

### 4. Contoh Soal & Pembahasan Terperinci

#### Contoh 1 (Tingkat Dasar: Analisis Komprehensif Data Tunggal Santri)
**Soal:**
Berikut adalah data perolehan nilai tes kelancaran membaca kitab kuning (*Fathul Qorib*) dari $10$ orang santri kelas mutawassithah:

$$
68, \ 72, \ 75, \ 75, \ 78, \ 80, \ 82, \ 85, \ 85, \ 90
$$

Tentukan:
a. Ukuran Pemusatan: Mean ($\bar{x}$), Median ($Me$), dan Modus ($Mo$).  
b. Ukuran Letak: Kuartil Bawah ($Q_1$), Kuartil Atas ($Q_3$), dan Jangkauan Antarkuartil ($H$).  
c. Ukuran Penyebaran: Simpangan Rata-rata ($SR$), Varians ($S^2$), dan Simpangan Baku ($S$).  
d. Angka Baku ($Z$-score) dari seorang santri bernama Ahmad yang memperoleh nilai $85$.

**Penyelesaian:**
- **Diketahui:**
  Data terurut: $n = 10$.
  Nilai: $68, 72, 75, 75, 78, 80, 82, 85, 85, 90$.

- **Ditanyakan:**
  a. $\bar{x}, Me, Mo$  
  b. $Q_1, Q_3, H$  
  c. $SR, S^2, S$  
  d. $Z$-score Ahmad ($x = 85$)

- **Langkah Penyelesaian:**

**1. Ukuran Pemusatan:**
- **Mean ($\bar{x}$):**

$$
\bar{x} = \frac{68 + 72 + 75 + 75 + 78 + 80 + 82 + 85 + 85 + 90}{10} = \frac{790}{10} = 79
$$

- **Median ($Me$):**  
  Letak median berada di antara data ke-$5$ ($78$) dan data ke-$6$ ($80$):

$$
Me = \frac{x_5 + x_6}{2} = \frac{78 + 80}{2} = 79
$$

- **Modus ($Mo$):**  
  Nilai yang memiliki frekuensi terbanyak (muncul $2$ kali) adalah $75$ dan $85$ (**Bimodal**).

**2. Ukuran Letak:**
- Paruh bawah ($5$ data): $68, 72, 75, 75, 78 \implies Q_1 = 75$.
- Paruh atas ($5$ data): $80, 82, 85, 85, 90 \implies Q_3 = 85$.
- **Hamparan ($H$):**

$$
H = Q_3 - Q_1 = 85 - 75 = 10
$$

**3. Ukuran Penyebaran:**
- Nilai selisih mutlak $\lvert x_i - \bar{x} \rvert$ terhadap $\bar{x} = 79$:  
  $\lvert 68 - 79 \rvert = 11$, $\lvert 72 - 79 \rvert = 7$, $\lvert 75 - 79 \rvert = 4$, $\lvert 75 - 79 \rvert = 4$, $\lvert 78 - 79 \rvert = 1$, $\lvert 80 - 79 \rvert = 1$, $\lvert 82 - 79 \rvert = 3$, $\lvert 85 - 79 \rvert = 6$, $\lvert 85 - 79 \rvert = 6$, $\lvert 90 - 79 \rvert = 11$.

$$
\begin{aligned}
\sum_{i=1}^{10} \lvert x_i - \bar{x} \rvert &= 11 + 7 + 4 + 4 + 1 + 1 + 3 + 6 + 6 + 11 = 54 \\
SR &= \frac{54}{10} = 5{,}4
\end{aligned}
$$

- Kuadrat deviasi $(x_i - \bar{x})^2$:  
  $121, 49, 16, 16, 1, 1, 9, 36, 36, 121$.

$$
\begin{aligned}
\sum_{i=1}^{10} (x_i - \bar{x})^2 &= 121 + 49 + 16 + 16 + 1 + 1 + 9 + 36 + 36 + 121 = 406 \\
S^2 &= \frac{406}{10} = 40{,}6 \\
S &= \sqrt{40{,}6} \approx 6{,}37
\end{aligned}
$$

**4. Angka Baku ($Z$-score) Ahmad ($x = 85$):**

$$
Z = \frac{x - \bar{x}}{S} = \frac{85 - 79}{6{,}37} = \frac{6}{6{,}37} \approx +0{,}94
$$

- **Kesimpulan:**
  Rata-rata kelas adalah $79$ dengan simpangan baku $6{,}37$. Ahmad memperoleh $Z = +0{,}94$, artinya kemampuan membaca kitab Ahmad berada $0{,}94$ simpangan baku **di atas rata-rata** seluruh santri di kelasnya ($\checkmark\ \text{Benar}$).

---

#### Contoh 2 (Pengembangan: Analisis Terpadu Data Berkelompok & Evaluasi Homogenitas)
**Soal:**
Tabel berikut menyajikan data durasi waktu muthala'ah (belajar mandiri malam) dari $40$ orang santri di asrama pondok pesantren:

| Waktu Muthala'ah (Menit) | Frekuensi ($f_i$) |
| :---: | :---: |
| $31 - 40$ | $4$ |
| $41 - 50$ | $8$ |
| $51 - 60$ | $14$ |
| $61 - 70$ | $10$ |
| $71 - 80$ | $4$ |

Tentukan:
a. Nilai rata-rata hitung ($\bar{x}$).  
b. Nilai Median ($Me$) dan Modus ($Mo$).  
c. Nilai Persentil ke-$75$ ($P_{75}$).  
d. Nilai Simpangan Baku ($S$) dan Koefisien Variasi ($KV$).

**Penyelesaian:**
- **Langkah 1: Susun Tabel Komputasi Penolong:**

| Kelas | $f_i$ | Titik Tengah ($x_i$) | $f_i x_i$ | $f_k$ | $(x_i - \bar{x})$ | $(x_i - \bar{x})^2$ | $f_i (x_i - \bar{x})^2$ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| $31 - 40$ | $4$ | $35{,}5$ | $142$ | $4$ | $-20$ | $400$ | $1.600$ |
| $41 - 50$ | $8$ | $45{,}5$ | $364$ | $12$ | $-10$ | $100$ | $800$ |
| $51 - 60$ | $14$ | $55{,}5$ | $777$ | $26$ | $0$ | $0$ | $0$ |
| $61 - 70$ | $10$ | $65{,}5$ | $655$ | $36$ | $+10$ | $100$ | $1.000$ |
| $71 - 80$ | $4$ | $75{,}5$ | $302$ | $40$ | $+20$ | $400$ | $1.600$ |
| **Total** | $\sum f_i = 40$ | $-$ | $\sum f_i x_i = 2.220$ | $-$ | $-$ | $-$ | $\sum = 5.000$ |

- **Langkah 2: Menghitung Nilai Rata-rata ($\bar{x}$):**

$$
\bar{x} = \frac{\sum f_i x_i}{\sum f_i} = \frac{2.220}{40} = 55{,}5\text{ menit}
$$

- **Langkah 3: Menghitung Median ($Me$):**
  - Letak Median = data ke-$\frac{40}{2} = 20$, berada pada kelas ke-$3$ ($51 - 60$).
  - $L_{me} = 50{,}5$, $\sum f_{k,me} = 12$, $f_{me} = 14$, $p = 10$.

$$
Me = 50{,}5 + \left( \frac{20 - 12}{14} \right) \cdot 10 = 50{,}5 + \frac{80}{14} \approx 50{,}5 + 5{,}71 = 56{,}21\text{ menit}
$$

- **Langkah 4: Menghitung Modus ($Mo$):**
  - Kelas modus memiliki frekuensi terbesar ($14$), yaitu kelas $51 - 60$.
  - $L_{mo} = 50{,}5$, $d_1 = 14 - 8 = 6$, $d_2 = 14 - 10 = 4$, $p = 10$.

$$
Mo = 50{,}5 + \left( \frac{6}{6 + 4} \right) \cdot 10 = 50{,}5 + \frac{6}{10} \cdot 10 = 50{,}5 + 6 = 56{,}5\text{ menit}
$$

- **Langkah 5: Menghitung Persentil ke-$75$ ($P_{75}$):**
  - Letak $P_{75} = \frac{75}{100} \cdot 40 = 30$, berada pada kelas ke-$4$ ($61 - 70$).
  - $L_{P} = 60{,}5$, $\sum f_k = 26$, $f_P = 10$, $p = 10$.

$$
P_{75} = 60{,}5 + \left( \frac{30 - 26}{10} \right) \cdot 10 = 60{,}5 + \frac{4}{10} \cdot 10 = 64{,}5\text{ menit}
$$

- **Langkah 6: Menghitung Simpangan Baku ($S$) & Koefisien Variasi ($KV$):**

$$
\begin{aligned}
S^2 &= \frac{\sum f_i (x_i - \bar{x})^2}{\sum f_i} = \frac{5.000}{40} = 125 \\
S &= \sqrt{125} = 5\sqrt{5} \approx 11{,}18\text{ menit} \\
KV &= \frac{S}{\bar{x}} \times 100\% = \frac{11{,}18}{55{,}5} \times 100\% \approx 20{,}14\%
\end{aligned}
$$

- **Kesimpulan:**
  Rata-rata waktu muthala'ah santri adalah $55{,}5\text{ menit}$ dengan simpangan baku $11{,}18\text{ menit}$. Sebanyak $75\%$ santri belajar mandiri selama $\le 64{,}5\text{ menit}$, dan nilai $KV = 20{,}14\%$ menunjukkan variabilitas waktu belajar santri tergolong cukup homogen ($\checkmark\ \text{Benar}$).

---

### 5. Penerapan Kontekstual (Studi Kasus Santri & Kehidupan Nyata)

#### Audit Kesiapan Wisuda Tahfiz: Analisis Dua Asrama Santri
> Pengurus Lembaga Tahfizul Qur'an Pesantren mengevaluasi capaian hafalan Al-Qur'an (dalam satuan juz) santri tingkat akhir di dua asrama menjelang wisuda tasmi'. Masing-masing asrama membina $30$ orang santri.
> 
> Dari hasil pengolahan data riil diperoleh ringkasan statistik berikut:
> - **Asrama Salman Al-Farisi**:
>   - Rata-rata hafalan: $\bar{x}_1 = 24\text{ juz}$
>   - Median: $Me_1 = 25\text{ juz}$
>   - Simpangan Baku: $S_1 = 2{,}1\text{ juz}$
> - **Asrama Bilal bin Rabah**:
>   - Rata-rata hafalan: $\bar{x}_2 = 24\text{ juz}$
>   - Median: $Me_2 = 21\text{ juz}$
>   - Simpangan Baku: $S_2 = 5{,}6\text{ juz}$

**Analisis Komprehensif Berbasis Data:**

1. **Analisis Nilai Rata-rata vs Median (Bentuk Kurva Kemiringan):**
   - Pada **Asrama Salman Al-Farisi**, nilai $\bar{x}_1 = 24$ dan $Me_1 = 25$ relatif berdekatan ($\bar{x} \approx Me$). Hal ini mengindikasikan bahwa distribusi hafalan santri mendekati **simetris normal**. Sebagian besar santri berada di sekitar $22 - 26\text{ juz}$.
   - Pada **Asrama Bilal bin Rabah**, nilai $Me_2 = 21$ jauh lebih rendah daripada rata-ratanya $\bar{x}_2 = 24$ ($Me \lt \bar{x}$). Hal ini menunjukkan distribusi **miring ke kanan (*positively skewed*)**. Artinya, mayoritas santri sebenarnya baru hafal sekitar $21\text{ juz}$, namun nilai rata-rata asrama terangkat tinggi karena adanya segelintir santri luar biasa yang sudah khatam $30\text{ juz}$ (*pencilan atas / high outliers*).

2. **Evaluasi Homogenitas & Konsistensi (Simpangan Baku & Koefisien Variasi):**

$$
\begin{aligned}
KV_{\text{Salman}} &= \frac{2{,}1}{24} \times 100\% = 8{,}75\% \\
KV_{\text{Bilal}} &= \frac{5{,}6}{24} \times 100\% = 23{,}33\%
\end{aligned}
$$

   - Asrama Salman Al-Farisi memiliki $KV$ yang sangat rendah ($8{,}75\%$), membuktikan bahwa proses belajar dan setoran santri berlangsung sangat **merata, disiplin, dan konsisten**.
   - Asrama Bilal bin Rabah memiliki $KV$ yang tinggi ($23{,}33\%$), menandakan adanya **kesenjangan hafalan yang sangat tajam (*gap*)** di antara sesama santri sekamar.

3. **Rekomendasi Kebijakan Pondok Pesantren:**
   - **Untuk Asrama Bilal**: Pengasuh wajib menerapkan sistem tutor sebaya (*peer-mentoring*), di mana santri yang sudah hafal $30\text{ juz}$ ditugaskan menyimak dan membantu santri yang masih berada di bawah $20\text{ juz}$.
   - **Untuk Asrama Salman**: Metode halaqah dapat dipertahankan sebagai percontohan (*role model*) manajemen kurikulum tahfiz yang berhasil menjaga pemerataan capaian santri.

---

### 6. Pola Kunci & Cara Cepat Mengingat

- **Bagan Alur Lengkap Investigasi Statistika Deskriptif:**

> 1. **Data Mentah** $\longrightarrow$ Urutkan data dan susun ke dalam **Tabel Distribusi & Kurva Ogive**.  
> 2. **Kalkulasi Parameter Statistik**:
>    - **Ukuran Pemusatan**: Mean ($\bar{x}$), Median ($Me$), Modus ($Mo$)
>    - **Ukuran Letak**: Kuartil ($Q_i$), Desil ($D_i$), Persentil ($P_i$)
>    - **Ukuran Penyebaran**: Jangkauan ($R$), Simpangan Rata-rata ($SR$), Ragam ($S^2$), Simpangan Baku ($S$)  
> 3. **Analisis Komparasi Relatif**: Angka Baku ($Z$-Score) dan Koefisien Variasi ($KV$).  
> 4. **Pengambilan Kebijakan Pesantren**: Rekomendasi pembinaan santri berbasis data objektif.

- **Jembatan Keledai Bentuk Kurva Kemiringan (*Skewness*):**
  > *"Rata-rata selalu ditarik ke arah ekor panjang: Kalau ekor ke kanan, Mean paling besar ($Mo < Me < \bar{x}$). Kalau ekor ke kiri, Mean paling kecil ($\bar{x} < Me < Mo$)."*

- **Catatan Waspada Kesalahan Umum (*Common Pitfalls*):**
  - ⚠️ **Tertipu Nilai Rata-rata**: Jangan pernah menyimpulkan dua kelompok sama prestasinya hanya karena nilai rata-ratanya sama. Selalu periksa nilai **Simpangan Baku ($S$)** atau **Koefisien Variasi ($KV$)**.
  - ⚠️ **Salah Frekuensi Kumulatif pada Fraktil**: Pada rumus $Me, Q_i, D_i,$ atau $P_i$, simbol $\sum f_k$ adalah **jumlah frekuensi seluruh kelas SEBELUM kelas target**, bukan frekuensi pada kelas target itu sendiri.
  - ⚠️ **Ketelitian Panjang Kelas ($p$)**: Untuk kelas bertipe bulat seperti $51 - 60$, panjang kelasnya adalah $60 - 51 + 1 = 10$, bukan $60 - 51 = 9$.

---

### 7. Latihan Soal Mandiri

---

#### Latihan Soal 1: Analisis Terpadu Data Tunggal & Transformasi Statistik (20 Soal)

**Petunjuk Pengerjaan:**
- Untuk soal nomor 1–4, jawablah pertanyaan pemahaman konsep dan interpretasi statistik secara ringkas dan tepat.
- Untuk soal nomor 5–14, hitunglah seluruh parameter statistik yang diminta (Mean, Median, Modus, $Q_1, Q_3, H, SR, S^2,$ dan $S$) dari kumpulan data yang diberikan.
- Untuk soal nomor 15–20, selesaikan permasalahan sifat aljabar, transformasi data, dan penalaran statistika.

1. Jelaskan mengapa nilai median lebih andal digunakan dibandingkan nilai rata-rata hitung pada data yang memiliki pencilan (*outlier*) ekstrem!
2. Seorang santri memperoleh nilai ujian nahwu $82$ pada kelas dengan rata-rata $76$ dan simpangan baku $4$. Di kelas shorof, ia memperoleh nilai $85$ pada kelas dengan rata-rata $75$ dan simpangan baku $8$. Pada mata pelajaran manakah posisi santri tersebut relatif lebih unggul? Jelaskan menggunakan konsep $Z$-score!
3. Dua kelompok santri mengikuti uji petik hafalan mufradat. Kelompok A memiliki rata-rata $50$ kata dengan $S = 5$, sedangkan Kelompok B memiliki rata-rata $80$ kata dengan $S = 8$. Kelompok manakah yang memiliki variabilitas relatif lebih konsisten?
4. Suatu kumpulan data memiliki nilai rata-rata $60$, median $58$, dan modus $55$. Buatlah sketsa kasar bentuk kurva distribusi data tersebut dan tentukan jenis kemiringannya (*skewness*)!
5. Diberikan data nilai tasmi' Al-Qur'an: $70, 72, 75, 75, 80, 84, 88$. Tentukan nilai Mean, Median, Modus, Jangkauan, dan Simpangan Bakunya!
6. Diberikan data waktu (dalam menit) santri mengkhatamkan wirid ba'da maghrib: $12, 14, 15, 15, 16, 18, 20, 26$. Hitunglah Kuartil Bawah ($Q_1$), Kuartil Atas ($Q_3$), Hamparan ($H$), dan Simpangan Kuartil ($Q_d$)!
7. Diberikan data berat buah tin (dalam gram) hasil kebun pesantren: $40, 42, 45, 48, 50, 55$. Tentukan Simpangan Rata-rata ($SR$) dan Varians ($S^2$) dari data tersebut!
8. Diberikan data: $4, 6, 7, 7, 8, 9, 10, 13$. Tentukan nilai ragam ($S^2$) dan simpangan baku ($S$)!
9. Data skor ujian tajwid: $65, 70, 75, 80, 80, 85, 90, 95$. Hitunglah persentil ke-$25$ dan persentil ke-$75$, lalu tentukan simpangan kuartilnya!
10. Data setoran hafalan barzanji: $8, 8, 9, 10, 10, 11, 12, 12, 14$. Tentukan nilai mean, simpangan rata-rata, dan simpangan bakunya!
11. Data usia santri penghuni kamar Abu Ubaidah: $14, 15, 15, 16, 16, 16, 17, 18, 19$. Tentukan modus, median, dan jangkauan antarkuartil data tersebut!
12. Diberikan data pengamatan durasi muthala'ah (dalam jam per pekan): $10, 12, 14, 16, 18, 20$. Tentukan nilai koefisien variasinya ($KV$)!
13. Diberikan data: $5, 8, 9, 10, 12, 15, 18, 19$. Hitunglah nilai simpangan rata-rata ($SR$) data tersebut!
14. Data skor adab santri: $78, 80, 82, 84, 85, 86, 88, 93$. Tentukan nilai varians ($S^2$) dan simpangan bakunya ($S$)!
15. Sekumpulan data berukuran $n = 8$ memiliki nilai rata-rata $50$ dan simpangan baku $6$. Jika setiap nilai data dikalikan $3$ kemudian dikurangi $15$, tentukan nilai rata-rata dan simpangan baku data yang baru!
16. Suatu data memiliki varians $S^2 = 9$. Jika seluruh data diubah melalui rumus $y_i = -4x_i + 25$, tentukan nilai simpangan baku dan varians data yang baru!
17. Diketahui kumpulan data $x_1, x_2, \dots, x_{10}$ memiliki $\sum x_i = 150$ dan $\sum x_i^2 = 2.450$. Tentukan nilai varians ($S^2$) dan simpangan baku ($S$) data tersebut!
18. Dari lima bilangan bulat positif diketahui mediannya adalah $7$, modusnya adalah $6$, dan rata-ratanya adalah $8$. Jika jangkauannya adalah $6$, tentukan kelima bilangan tersebut!
19. Santri teladan memiliki nilai ujian tauhid $92$. Jika nilai rata-rata kelas adalah $80$ dengan varians $25$, berapakah nilai angka baku ($Z$-score) santri tersebut?
20. Tiga puluh santri memiliki rata-rata nilai matematika $72$ dengan simpangan baku $8$. Dua orang santri baru dengan nilai $72$ dan $72$ bergabung ke dalam kelompok tersebut. Selidikilah secara aljabar apakah simpangan baku kelompok yang baru membesar, mengecil, atau tetap!

---

#### Latihan Soal 2: Analisis Terpadu Data Berkelompok & Kurva Frekuensi (20 Soal)

**Petunjuk Pengerjaan:**
- Untuk soal nomor 1–4, jawablah pertanyaan analisis kurva distribusi dan sifat data berkelompok.
- Untuk soal nomor 5–14, selesaikan perhitungan ukuran pemusatan, letak, dan penyebaran dari tabel distribusi frekuensi yang disajikan.
- Untuk soal nomor 15–20, selesaikan analisis komparasi dan rekonstruksi data distribusi frekuensi.

1. Jelaskan perbedaan pokok antara ogive positif (ogive naik) dan ogive negatif (ogive turun) serta bagaimana keduanya dapat digunakan untuk menentukan letak nilai median!
2. Jika suatu tabel distribusi frekuensi memiliki batas kelas pertama $20 - 29$, tentukan batas bawah, batas atas, tepi bawah, tepi atas, dan panjang kelas interval tersebut!
3. Tuliskan hubungan matematis antara Kuartil ke-$2$ ($Q_2$), Desil ke-$5$ ($D_5$), dan Persentil ke-$50$ ($P_{50}$) pada data berkelompok!
4. Jelaskan dampak penambahan kelas interval baru dengan frekuensi sangat kecil pada ekor kanan terhadap nilai rata-rata dan nilai median!

*(Gunakan tabel distribusi frekuensi berikut untuk mengerjakan soal nomor 5–8)*  
Tabel nilai ujian hafalan matan jazariyah $40$ santri:

| Nilai Ujian | Frekuensi ($f_i$) |
| :---: | :---: |
| $51 - 60$ | $6$ |
| $61 - 70$ | $10$ |
| $71 - 80$ | $14$ |
| $81 - 90$ | $7$ |
| $91 - 100$ | $3$ |

5. Tentukan nilai titik tengah ($x_i$) untuk setiap kelas interval dan hitunglah nilai rata-rata hitung ($\bar{x}$) nilai ujian santri!
6. Tentukan nilai Median ($Me$) dan Modus ($Mo$) dari tabel ujian tersebut!
7. Tentukan nilai Kuartil Bawah ($Q_1$) dan Kuartil Atas ($Q_3$) dari data berkelompok tersebut!
8. Lengkapi tabel penolong kuadrat deviasi dan hitunglah nilai simpangan baku ($S$) dari nilai ujian santri tersebut!

*(Gunakan tabel distribusi frekuensi berikut untuk mengerjakan soal nomor 9–12)*  
Tabel durasi zikir pagi (dalam menit) dari $50$ santri:

| Waktu (Menit) | Frekuensi ($f_i$) |
| :---: | :---: |
| $11 - 15$ | $5$ |
| $16 - 20$ | $12$ |
| $21 - 25$ | $18$ |
| $26 - 30$ | $10$ |
| $31 - 35$ | $5$ |

9. Hitunglah nilai rata-rata hitung ($\bar{x}$) durasi zikir pagi santri!
10. Tentukan nilai Desil ke-$4$ ($D_4$) dan Desil ke-$8$ ($D_8$) dari data durasi zikir tersebut!
11. Tentukan nilai Persentil ke-$90$ ($P_{90}$) yang membatasi $10\%$ santri dengan durasi zikir terlama!
12. Hitunglah nilai Simpangan Rata-rata ($SR$) dari data berkelompok tersebut!

*(Gunakan tabel distribusi frekuensi berikut untuk mengerjakan soal nomor 13–14)*  
Tabel skor tes kosakata bahasa Arab santri baru:

| Skor | Frekuensi |
| :---: | :---: |
| $41 - 50$ | $4$ |
| $51 - 60$ | $8$ |
| $61 - 70$ | $12$ |
| $71 - 80$ | $10$ |
| $81 - 90$ | $6$ |

13. Hitunglah nilai ragam ($S^2$) dan simpangan baku ($S$) skor tes kosakata bahasa Arab tersebut!
14. Hitunglah nilai Koefisien Variasi ($KV$) dari data skor kosakata bahasa Arab tersebut!
15. Suatu tabel distribusi frekuensi memiliki kelas median pada interval $60 - 69$ dengan panjang kelas $10$, frekuensi kelas median $16$, dan frekuensi kumulatif sebelum kelas median $14$. Jika total frekuensi adalah $40$, tentukan nilai mediannya!
16. Sebuah data berkelompok memiliki nilai $\sum f_i = 60$, $\sum f_i x_i = 4.200$, dan $\sum f_i x_i^2 = 301.500$. Tentukan nilai mean dan simpangan baku data tersebut!
17. Diberikan histogram dengan nilai tengah kelas $15, 20, 25, 30$ dan frekuensi masing-masing $4, 6, 8, 2$. Tentukan nilai rata-rata dan modusnya!
18. Dari tabel distribusi frekuensi simetris diketahui nilai $\bar{x} = 75$ dan simpangan baku $S = 6$. Jika seluruh data di setiap kelas interval dikurangi $5$, tentukan nilai mean, median, dan simpangan baku yang baru!
19. Diketahui frekuensi kumulatif kurang dari untuk kelas-kelas interval berturut-turut adalah $3, 9, 21, 32, 40$. Tentukan frekuensi mutlak ($f_i$) pada setiap kelas interval!
20. Pada tabel distribusi frekuensi durasi tidur malam santri, diketahui modus berada pada interval $41 - 50$ dengan frekuensi $15$. Selisih frekuensi kelas modus dengan kelas sebelumnya adalah $5$ dan dengan kelas sesudahnya adalah $3$. Tentukan nilai modusnya!

---

#### Latihan Soal 3: Studi Kasus Kontekstual Santri & Pemecahan Masalah Nyata Pesantren (20 Soal)

**Petunjuk Pengerjaan:**
- Analisislah setiap permasalahan kontekstual di lingkungan pondok pesantren berikut dengan menerapkan konsep statistika deskriptif secara utuh, jujur, dan bertanggung jawab.

1. Pengasuh halaqah tahfiz mencatat capaian setoran tasmi' hafalan Al-Qur'an (dalam lembar per pekan) dari $9$ santri teladan: $14, 16, 18, 18, 20, 22, 24, 25, 32$. Hitunglah jangkauan, rata-rata, dan simpangan kuartilnya!
2. Catatan nilai ujian lisan nahwu jurumiyah dari $8$ santri asrama adalah: $74, 76, 78, 80, 80, 84, 88, 96$. Tentukan nilai simpangan rata-rata dan simpangan bakunya!
3. Dua kamar santri dievaluasi kedisiplinan jam bangun tahajud (dalam menit sebelum subuh) selama sepekan:
   - Kamar Ibnu Abbas: $30, 35, 40, 40, 45, 50, 50$
   - Kamar Ibnu Umar: $20, 30, 40, 45, 50, 60, 65$  
   Hitunglah rata-rata dan simpangan baku kedua kamar, lalu analisislah kamar manakah yang paling konsisten bangun malam!
4. Pengurus dapur umum pesantren menimbang kebutuhan konsumsi telur ayam harian (dalam kg) selama $7$ hari: $25, 28, 30, 30, 32, 35, 36\text{ kg}$. Hitung varians dan simpangan bakunya!
5. Santri piket kebersihan mencatat volume penggunaan air wudu di masjid pesantren (dalam ratusan liter) pada $8$ waktu salat: $15, 16, 18, 18, 20, 22, 25, 30$. Tentukan kuartil bawah ($Q_1$), median ($Me$), dan kuartil atas ($Q_3$) pemakaian air tersebut!
6. Poskestren memeriksa kadar hemoglobin (Hb dalam g/dL) dari $7$ orang santriwati: $11{,}8; 12{,}0; 12{,}2; 12{,}4; 12{,}6; 13{,}0; 13{,}4$. Tentukan nilai rata-rata dan simpangan baku kadar Hb santriwati!
7. Toko Kitab Pesantren mendata jumlah penjualan kitab fiqih per hari selama $10$ hari: $8, 10, 12, 12, 14, 15, 16, 18, 20, 25\text{ eksemplar}$. Hitunglah koefisien variasinya ($KV$)!
8. Unit kebun buah tin pesantren mencatat berat panen harian (dalam kg) selama $6$ hari: $12, 14, 15, 16, 18, 21\text{ kg}$. Tentukan simpangan rata-rata hasil panen tersebut!
9. Sebanyak $40$ santri mengikuti ujian seleksi beasiswa kuliah ke Timur Tengah dengan sebaran nilai sebagai berikut:

| Nilai Seleksi | Frekuensi |
| :---: | :---: |
| $61 - 70$ | $4$ |
| $71 - 80$ | $12$ |
| $81 - 90$ | $16$ |
| $91 - 100$ | $8$ |

Panitia menetapkan bahwa santri yang berhak lolos ke tahap wawancara adalah mereka yang berada pada kelompok $25\%$ teratas ($P_{75}$). Tentukan nilai ambang batas minimal kelolosan santri!
10. Berdasarkan data tabel soal nomor 9, hitunglah nilai simpangan baku dari skor seleksi beasiswa tersebut!
11. Dua halaqah tahfiz putri memiliki rata-rata waktu muraja'ah mandiri yang sama yaitu $90\text{ menit}$. Halaqah Maryam memiliki simpangan baku $S = 6\text{ menit}$, sedangkan Halaqah Asiyah memiliki simpangan baku $S = 18\text{ menit}$. Analisislah kondisi riil kedua halaqah tersebut dan jelaskan halaqah manakah yang lebih membutuhkan pembimbingan intensif!
12. Santri bagian perpustakaan mendata jumlah kunjungan santri per hari selama dua pekan berturut-turut (dalam satuan orang): $35, 40, 42, 45, 45, 48, 50, 52, 55, 58, 60, 65$. Tentukan nilai persentil ke-$40$ ($P_{40}$) dari kunjungan perpustakaan!
13. Catatan infak sukarela harian santri untuk renovasi asrama yatim tercatat dalam tabel berikut:

| Infak (Ribu Rupiah) | Frekuensi Hari |
| :---: | :---: |
| $21 - 30$ | $5$ |
| $31 - 40$ | $8$ |
| $41 - 50$ | $12$ |
| $51 - 60$ | $10$ |
| $61 - 70$ | $5$ |

Tentukan rata-rata dan median perolehan infak harian tersebut!
14. Berdasarkan data tabel infak soal nomor 13, hitunglah nilai simpangan baku dan koefisien variasinya!
15. Santri bagian multimedia mendata kecepatan akses internet laboratorium komputer (dalam Mbps) pada $8$ titik ruangan: $16, 20, 22, 24, 25, 28, 30, 37\text{ Mbps}$. Hitung angka baku ($Z$-score) dari ruangan yang memiliki kecepatan $37\text{ Mbps}$!
16. Dalam musabaqah tilawatil Qur'an antar-pesantren, Zaid memperoleh nilai lagu $88$ pada kategori yang memiliki rata-rata $80$ dan simpangan baku $5$. Pada kategori tajwid, ia memperoleh nilai $92$ pada kategori dengan rata-rata $84$ dan simpangan baku $8$. Pada kategori manakah prestasi Zaid relatif lebih gemilang?
17. Dapur umum pesantren mencatat berat sisa makanan santri (dalam kg per hari) selama sepekan: $3, 4, 4, 5, 6, 7, 9\text{ kg}$. Tentukan jangkauan antarkuartil dan simpangan rata-rata sisa makanan untuk evaluasi efisiensi porsi makan!
18. Santri peternakan mendata hasil perahan susu kambing etawa (dalam liter per hari) selama $8$ hari: $14, 15, 16, 16, 17, 18, 20, 24\text{ liter}$. Tentukan varians dan simpangan baku produksi susu kambing!
19. Waktu yang dibutuhkan santri untuk menyelesaikan lari pagi mengelilingi kompleks pesantren sejauh $3\text{ km}$ tercatat: $14, 15, 16, 17, 17, 18, 20, 23\text{ menit}$. Hitunglah simpangan kuartil waktu tempuh santri!
20. Pembina asrama mendata poin pelanggaran kedisiplinan santri di dua lorong kamar: Lorong Al-Quds (rata-rata poin $= 12$ dengan $S = 2$) dan Lorong Al-Andalus (rata-rata poin $= 12$ dengan $S = 7$). Lorong manakah yang memiliki kedisiplinan santri lebih merata? Berikan rekomendasi tindakan pembinaan untuk pengurus santri!

---

### 8. Pekerjaan Rumah (PR Pondok / Mandiri)

**Petunjuk Pengerjaan:**
- Kerjakan di buku catatan tugas matematika secara mandiri, rapi, dan sistematis.
- Tuliskan dengan runtut apa yang diketahui, rumus statistika yang digunakan, perhitungan langkah per langkah, serta kesimpulan akhirnya.

1. **Analisis Terpadu Data Tunggal:**  
   Diberikan data nilai tasmi' $5\text{ juz}$ sekali duduk dari $10$ santri teladan:

$$
80, \ 82, \ 84, \ 85, \ 85, \ 88, \ 90, \ 92, \ 94, \ 98
$$

   Tentukan nilai Mean ($\bar{x}$), Median ($Me$), Modus ($Mo$), Kuartil Bawah ($Q_1$), Kuartil Atas ($Q_3$), Simpangan Rata-rata ($SR$), Varians ($S^2$), dan Simpangan Baku ($S$)!

2. **Analisis Terpadu Data Berkelompok:**  
   Diberikan tabel distribusi frekuensi waktu muthala'ah kitab kuning harian santri:

| Durasi (Menit) | Frekuensi ($f_i$) |
| :---: | :---: |
| $41 - 50$ | $4$ |
| $51 - 60$ | $10$ |
| $61 - 70$ | $16$ |
| $71 - 80$ | $14$ |
| $81 - 90$ | $6$ |

   Lengkapilah tabel penolong dan hitunglah:
   a. Rata-rata hitung ($\bar{x}$) dan Modus ($Mo$).  
   b. Persentil ke-$70$ ($P_{70}$).  
   c. Simpangan Baku ($S$) dan Koefisien Variasi ($KV$).

3. **Studi Kasus Komparasi Kehidupan Pondok Pesantren:**  
   Pengurus asrama membandingkan kedisiplinan kehadiran salat berjamaah subuh tepat waktu di masjid antara Kamar An-Nur dan Kamar Al-Falah selama $10$ hari pengamatan:
   - Kamar An-Nur memiliki rata-rata kehadiran $8$ santri per hari dengan simpangan baku $S = 0{,}8$.
   - Kamar Al-Falah memiliki rata-rata kehadiran $8$ santri per hari dengan simpangan baku $S = 2{,}9$.  
   Analisislah kamar manakah yang memiliki komitmen berjamaah lebih konsisten dan homogen, serta jelaskan makna perbedaan simpangan baku tersebut terhadap stabilitas suasana ibadah kamar!

4. **Pertanyaan Pemahaman Konsep & Refleksi Analitis:**  
   *Jelaskan mengapa dalam pengambilan kebijakan di pondok pesantren (seperti penentuan kelulusan beasiswa atau pendampingan belajar santri), pengasuh tidak boleh hanya melihat nilai rata-rata (mean) semata! Jelaskan bagaimana perpaduan antara Mean, Median, Simpangan Baku, dan Z-Score mampu menghasilkan keputusan yang lebih adil dan berakar pada nilai-nilai kebenaran!*

---

### 9. Ringkasan Materi

- **Statistika Deskriptif Terpadu**: Analisis data yang shahih mengintegrasikan ukuran penyajian (tabel dan ogive), ukuran pemusatan (Mean, Median, Modus), ukuran letak (Kuartil, Desil, Persentil), dan ukuran penyebaran (Simpangan Baku, Varians, Simpangan Kuartil) secara simultan.
- **Deteksi Kemiringan Sebaran (*Skewness*)**: Posisi relatif antara Mean, Median, dan Modus menentukan bentuk distribusi data. Jika $\bar{x} \approx Me \approx Mo$, data simetris normal; jika $Mo \lt Me \lt \bar{x}$, data miring ke kanan (*positively skewed*); jika $\bar{x} \lt Me \lt Mo$, data miring ke kiri (*negatively skewed*).
- **Alat Ukur Komparatif ($Z$-score dan $KV$)**: Angka baku ($Z = \frac{x - \bar{x}}{S}$) mengukur posisi relatif individu santri terhadap kelompoknya, sedangkan Koefisien Variasi ($KV = \frac{S}{\bar{x}} \times 100\%$) mengukur tingkat keragaman relatif dua kelompok data yang berbeda skala atau rata-ratanya.
- **Keadilan Hisab Berbasis Data**: Dalam Islam, statistika deskriptif menjadi sarana menegakkan objektivitas dan keadilan perlakuan, di mana setiap santri dievaluasi secara presisi sehingga kebijakan pendampingan belajar di pondok pesantren tepat sasaran dan berkeadilan.

