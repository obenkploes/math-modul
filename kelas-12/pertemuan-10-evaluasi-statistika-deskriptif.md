# MATEMATIKA SMA (JURUSAN IPA & PESANTREN)
## Kelas 12 - Semester Ganjil
### Pertemuan 10: Evaluasi Mandiri — Ulangan Harian Statistika Deskriptif

---

### 1. Pengertian & Konsep Dasar

Evaluasi mandiri (*self-assessment*) adalah proses pengujian yang dilakukan secara sadar, jujur, dan bertanggung jawab untuk mengukur sejauh mana seluruh konsep, formula, dan keterampilan analitis statistika deskriptif telah dikuasai dengan benar. 

Dalam tradisi keilmuan Islam dan kehidupan pondok pesantren, evaluasi merupakan perwujudan dari konsep **muhasabah** (introspeksi diri secara objektif). Allah SWT berfirman:

> *"Wahai orang-orang yang beriman! Bertakwalah kepada Allah dan hendaklah setiap diri memperhatikan apa yang telah diperbuatnya untuk hari esok (akhirat), dan bertakwalah kepada Allah. Sungguh, Allah Mahateliti terhadap apa yang kamu kerjakan."*  
> **(QS. Al-Hasyr: 18)**

Sebagaimana hisab di akhirat didasarkan pada catatan amal yang teliti tanpa ada yang terlewat sedikit pun (*QS. Al-Kahfi: 49*), penguasaan statistika deskriptif menguji kemampuan santri dalam membaca, menyajikan, dan menghitung data riil secara presisi. Mengetahui nilai rata-rata (*mean*) saja tidak mencukupi; seorang penuntut ilmu harus mampu melihat bagaimana data tersebut memusat, di mana letak posisinya, dan seberapa besar penyebaran (*dispersi*) nilai di sekitar pusatnya.

Modul Pertemuan 10 ini dirancang sebagai sarana **uji kompetensi komprehensif** yang menyatukan lima pilar statistika deskriptif:
1. **Penyajian Data**: Tabel distribusi frekuensi, histogram, poligon, dan kurva ogive.
2. **Ukuran Pemusatan**: Rata-rata hitung (*Mean* $\bar{x}$), nilai tengah (*Median* $Me$), dan nilai dominan (*Modus* $Mo$).
3. **Ukuran Letak**: Kuartil ($Q_1, Q_2, Q_3$), Desil ($D_i$), dan Persentil ($P_i$).
4. **Ukuran Penyebaran**: Jangkauan ($R$), Simpangan Kuartil ($Q_d$), Simpangan Rata-rata ($SR$), Varians ($S^2$), dan Simpangan Baku ($S$).
5. **Analisis Relatif & Sebaran**: Angka Baku ($Z$-score), Koefisien Variasi ($KV$), dan identifikasi kemiringan kurva (*skewness*).

---

### 2. Bentuk Umum & Rumus Baku

Berikut adalah lembar kompilasi formula resmi (*Master Formula Sheet*) yang digunakan dalam evaluasi mandiri ini:

#### A. Pembentukan Distribusi Frekuensi Data Berkelompok (Aturan Sturges)

Untuk data mentah berukuran $n$ dengan jangkauan $R = X_{\max} - X_{\min}$:

$$
k = 1 + 3{,}3 \log n \quad \text{dan} \quad p = \frac{R}{k}
$$

**Keterangan:**
- $k$: Banyak kelas interval (dibulatkan ke bilangan bulat terdekat atau ke atas).
- $p$: Panjang / lebar kelas interval.
- $R$: Jangkauan (*range*) data.

---

#### B. Ukuran Pemusatan Data

1. **Rata-rata Hitung (*Mean* $\bar{x}$):**
   - Data Tunggal:

$$
\bar{x} = \frac{\sum_{i=1}^n x_i}{n}
$$

   - Data Berkelompok:

$$
\bar{x} = \frac{\sum_{i=1}^k f_i x_i}{\sum_{i=1}^k f_i} \quad (x_i = \text{titik tengah kelas ke-}i)
$$

2. **Median ($Me$):**
   - Data Tunggal: Nilai data ke-$\frac{n+1}{2}$ (untuk $n$ ganjil) atau rata-rata data ke-$\frac{n}{2}$ dan ke-$\left(\frac{n}{2}+1\right)$ (untuk $n$ genap).
   - Data Berkelompok:

$$
Me = L_{me} + \left( \frac{\frac{1}{2}n - \sum f_{k,me}}{f_{me}} \right) p
$$

3. **Modus ($Mo$):**
   - Data Tunggal: Nilai yang frekuensinya paling banyak muncul.
   - Data Berkelompok:

$$
Mo = L_{mo} + \left( \frac{d_1}{d_1 + d_2} \right) p
$$

**Keterangan:**
- $L_{me}, L_{mo}$: Tepi bawah kelas median dan kelas modus ($L = \text{Batas Bawah} - 0{,}5$).
- $\sum f_{k,me}$: Jumlah frekuensi kumulatif sebelum kelas median.
- $f_{me}$: Frekuensi kelas median.
- $d_1 = f_{mo} - f_{mo-1}$: Selisih frekuensi kelas modus dengan kelas sebelumnya.
- $d_2 = f_{mo} - f_{mo+1}$: Selisih frekuensi kelas modus dengan kelas sesudahnya.

---

#### C. Ukuran Letak Data (Fraktil)

1. **Kuartil ($Q_i$ untuk $i = 1, 2, 3$):**

$$
Q_i = L_{Q_i} + \left( \frac{\frac{i}{4}n - \sum f_{k,Q_i}}{f_{Q_i}} \right) p
$$

2. **Desil ($D_i$ untuk $i = 1, 2, \dots, 9$):**

$$
D_i = L_{D_i} + \left( \frac{\frac{i}{10}n - \sum f_{k,D_i}}{f_{D_i}} \right) p
$$

3. **Persentil ($P_i$ untuk $i = 1, 2, \dots, 99$):**

$$
P_i = L_{P_i} + \left( \frac{\frac{i}{100}n - \sum f_{k,P_i}}{f_{P_i}} \right) p
$$

4. **Jangkauan Antarkuartil ($H$) dan Simpangan Kuartil ($Q_d$):**

$$
H = Q_3 - Q_1 \quad \text{dan} \quad Q_d = \frac{1}{2} H = \frac{1}{2}(Q_3 - Q_1)
$$

---

#### D. Ukuran Penyebaran Data

1. **Simpangan Rata-rata ($SR$):**
   - Data Tunggal:

$$
SR = \frac{\sum_{i=1}^n \lvert x_i - \bar{x} \rvert}{n}
$$

   - Data Berkelompok:

$$
SR = \frac{\sum_{i=1}^k f_i \lvert x_i - \bar{x} \rvert}{\sum_{i=1}^k f_i}
$$

2. **Ragam / Varians ($S^2$) dan Simpangan Baku ($S$):**
   - Data Tunggal:

$$
S^2 = \frac{\sum_{i=1}^n (x_i - \bar{x})^2}{n} \implies S = \sqrt{S^2}
$$

   - Data Berkelompok:

$$
S^2 = \frac{\sum_{i=1}^k f_i (x_i - \bar{x})^2}{\sum_{i=1}^k f_i} \implies S = \sqrt{S^2}
$$

---

#### E. Parameter Komparasi Relatif

1. **Angka Baku (*Z-Score*):**

$$
Z = \frac{x - \bar{x}}{S}
$$

2. **Koefisien Variasi ($KV$):**

$$
KV = \frac{S}{\bar{x}} \times 100\%
$$

---

### 3. Sifat-Sifat, Karakteristik, & Panduan Diagnostik Mandiri

#### A. Efek Transformasi Data terhadap Ukuran Statistik

Misalkan sekumpulan data awal memiliki rata-rata $\bar{x}$, median $Me$, modus $Mo$, jangkauan $R$, simpangan kuartil $Q_d$, simpangan rata-rata $SR$, dan simpangan baku $S$:

| Operasi Transformasi pada Setiap Data | Ukuran Pemusatan & Letak ($\bar{x}, Me, Mo, Q_i, P_i$) | Ukuran Penyebaran ($R, H, Q_d, SR, S$) | Varians ($S^2$) |
| :--- | :---: | :---: | :---: |
| **Ditambah konstanta $c$ ($x_i + c$)** | Bertambah sebesar $c$ ($\bar{x} + c$) | **Tetap** (tidak berubah) | **Tetap** |
| **Dikurang konstanta $c$ ($x_i - c$)** | Berkurang sebesar $c$ ($\bar{x} - c$) | **Tetap** (tidak berubah) | **Tetap** |
| **Dikalikan konstanta $k$ ($k \cdot x_i$)** | Dikalikan $k$ ($k \cdot \bar{x}$) | Dikalikan $|k|$ ($|k| \cdot S$) | Dikalikan $k^2$ ($k^2 \cdot S^2$) |
| **Dibagi konstanta $k$ ($\frac{x_i}{k}$)** | Dibagi $k$ ($\frac{\bar{x}}{k}$) | Dibagi $|k|$ ($\frac{S}{|k|}$) | Dibagi $k^2$ ($\frac{S^2}{k^2}$) |

---

#### B. Deteksi Kemiringan Kurva (*Skewness*)

Hubungan antara posisi tiga nilai pusat menentukan bentuk kurva distribusi frekuensi:

| Pola Hubungan Nilai Pusat | Bentuk Kurva Distribusi | Interpretasi Karakteristik Nilai Santri |
| :--- | :---: | :--- |
| **$\bar{x} = Me = Mo$** | Simetris (Distribusi Normal) | Nilai santri menyebar seimbang di kanan dan kiri rata-rata. |
| **$Mo \lt Me \lt \bar{x}$** | Miring ke Kanan (*Positively Skewed*) | Mayoritas santri memperoleh nilai di bawah rata-rata (soal dirasa sulit). |
| **$\bar{x} \lt Me \lt Mo$** | Miring ke Kiri (*Negatively Skewed*) | Mayoritas santri memperoleh nilai di atas rata-rata (prestasi sangat baik). |

---

#### C. Matriks Diagnostik Kesalahan Umum (*Common Traps Checklist*)

Sebelum menyelesaikan soal ulangan, perhatikan jebakan-jebakan umum berikut:
1. ⚠️ **Salah Mengambil Tepi Bawah ($L$)**: Tepi bawah adalah batas bawah kelas dikurangi $0{,}5$ (untuk data ketelitian satuan). Jangan memasukkan batas bawah langsung ke dalam rumus interpolasi.
2. ⚠️ **Tertukar Frekuensi Kumulatif ($\sum f_k$)**: Nilai $\sum f_k$ pada rumus Median, Kuartil, dan Persentil adalah jumlah frekuensi **sebelum** kelas yang bersangkutan, bukan frekuensi kelas itu sendiri.
3. ⚠️ **Lupa Mengurutkan Data**: Menentukan median, kuartil, dan desil data tunggal wajib mengurutkan data dari nilai terkecil ke terbesar terlebih dahulu.
4. ⚠️ **Mengabaikan Pengaruh Nilai Ekstrem (*Outlier*)**: Mean sangat rentan terdistorsi oleh nilai pencilan, sedangkan Median dan Simpangan Kuartil bersifat resisten (*robust*).
5. ⚠️ **Simpangan Baku Bernilai Negatif**: Nilai varians ($S^2$) dan simpangan baku ($S$) **selalu $\ge 0$**. Jika hasil hitungmu negatif, dipastikan terjadi kesalahan penjumlahan kuartal deviasi.

---

### 4. Contoh Soal Evaluasi & Pembahasan Terperinci

#### Contoh 1 (Tingkat Standar: Evaluasi Komprehensif Data Tunggal Santri)
**Soal:**
Tercatat skor penilaian kelancaran membaca kitab kuning (*Fathul Qorib*) dari $10$ orang santri teladan:

$$
74, \ 82, \ 68, \ 90, \ 74, \ 86, \ 78, \ 70, \ 84, \ 74
$$

Tentukan:
a. Mean ($\bar{x}$), Median ($Me$), dan Modus ($Mo$).  
b. Kuartil Bawah ($Q_1$), Kuartil Atas ($Q_3$), dan Simpangan Kuartil ($Q_d$).  
c. Simpangan Rata-rata ($SR$) dan Simpangan Baku ($S$).  
d. Angka baku ($Z$-score) santri bernama Zaid yang memperoleh skor $90$.

**Penyelesaian:**
- **Langkah 1: Mengurutkan Data ($n = 10$):**

$$
68, \ 70, \ 74, \ 74, \ 74, \ 78, \ 82, \ 84, \ 86, \ 90
$$

- **Langkah 2: Menghitung Ukuran Pemusatan:**
  - **Mean ($\bar{x}$):**

$$
\bar{x} = \frac{68 + 70 + 74 + 74 + 74 + 78 + 82 + 84 + 86 + 90}{10} = \frac{780}{10} = 78
$$

  - **Median ($Me$):** Letak median berada di antara data ke-$5$ ($74$) dan data ke-$6$ ($78$):

$$
Me = \frac{x_5 + x_6}{2} = \frac{74 + 78}{2} = 76
$$

  - **Modus ($Mo$):** Nilai yang paling sering muncul adalah $74$ (muncul sebanyak $3$ kali).

- **Langkah 3: Menghitung Ukuran Letak:**
  - Paruh bawah ($5$ data pertama: $68, 70, \mathbf{74}, 74, 74$) $\implies Q_1 = 74$.
  - Paruh atas ($5$ data terakhir: $78, 82, \mathbf{84}, 86, 90$) $\implies Q_3 = 84$.
  - **Simpangan Kuartil ($Q_d$):**

$$
Q_d = \frac{1}{2}(Q_3 - Q_1) = \frac{1}{2}(84 - 74) = \frac{1}{2}(10) = 5
$$

- **Langkah 4: Menghitung Ukuran Penyebaran:**
  - Selisih mutlak $\lvert x_i - \bar{x} \rvert$ terhadap $\bar{x} = 78$: $10, 8, 4, 4, 4, 0, 4, 6, 8, 12$.

$$
\sum_{i=1}^{10} \lvert x_i - 78 \rvert = 10 + 8 + 4 + 4 + 4 + 0 + 4 + 6 + 8 + 12 = 60
$$

$$
SR = \frac{60}{10} = 6
$$

  - Kuadrat selisih $(x_i - \bar{x})^2$: $100, 64, 16, 16, 16, 0, 16, 36, 64, 144$.

$$
\sum_{i=1}^{10} (x_i - 78)^2 = 100 + 64 + 16 + 16 + 16 + 0 + 16 + 36 + 64 + 144 = 472
$$

$$
S^2 = \frac{472}{10} = 47{,}2 \implies S = \sqrt{47{,}2} \approx 6{,}87
$$

- **Langkah 5: Menghitung Angka Baku ($Z$-score) Zaid ($x = 90$):**

$$
Z = \frac{90 - 78}{6{,}87} = \frac{12}{6{,}87} \approx +1{,}75
$$

- **Kesimpulan:**  
  Rata-rata skor adalah $78$, median $76$, modus $74$, dengan $S = 6{,}87$. Nilai $Z = +1{,}75$ menunjukkan Zaid berada $1{,}75$ simpangan baku di atas rata-rata kelompok ($\checkmark\ \text{Benar}$).

---

#### Contoh 2 (Tingkat Pengembangan: Evaluasi Data Berkelompok & Koefisien Variasi)
**Soal:**
Tabel berikut menyajikan data durasi belajar mandiri malam (*muthala'ah*) dari $50$ orang santri asrama:

| Durasi (Menit) | Frekuensi ($f_i$) |
| :---: | :---: |
| $41 - 50$ | $6$ |
| $51 - 60$ | $12$ |
| $61 - 70$ | $18$ |
| $71 - 80$ | $10$ |
| $81 - 90$ | $4$ |

Tentukan:
a. Nilai rata-rata hitung ($\bar{x}$).  
b. Nilai Median ($Me$) dan Modus ($Mo$).  
c. Kuartil Atas ($Q_3$).  
d. Simpangan Baku ($S$) dan Koefisien Variasi ($KV$).

**Penyelesaian:**
- **Langkah 1: Susun Tabel Komputasi Penolong ($n = 50$):**

| Interval | $f_i$ | $x_i$ | $f_i x_i$ | $f_k$ | $(x_i - \bar{x})$ | $(x_i - \bar{x})^2$ | $f_i (x_i - \bar{x})^2$ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| $41 - 50$ | $6$ | $45{,}5$ | $273$ | $6$ | $-19$ | $361$ | $2.166$ |
| $51 - 60$ | $12$ | $55{,}5$ | $666$ | $18$ | $-9$ | $81$ | $972$ |
| $61 - 70$ | $18$ | $65{,}5$ | $1.179$ | $36$ | $+1$ | $1$ | $18$ |
| $71 - 80$ | $10$ | $75{,}5$ | $755$ | $46$ | $+11$ | $121$ | $1.210$ |
| $81 - 90$ | $4$ | $85{,}5$ | $342$ | $50$ | $+21$ | $441$ | $1.764$ |
| **Total** | $\sum f_i = 50$ | $-$ | $\sum f_i x_i = 3.215$ | $-$ | $-$ | $-$ | $\sum = 6.130$ |

- **Langkah 2: Menghitung Rata-rata ($\bar{x}$):**

$$
\bar{x} = \frac{3.215}{50} = 64{,}3\text{ menit} \approx 64{,}5\text{ menit} \quad (\text{dibulatkan ke } 64{,}5 \text{ untuk komputasi deviasi baku})
$$

Jika menggunakan nilai presisi $\bar{x} = 64{,}3$:
- **Langkah 3: Menghitung Median ($Me$):**
  - Letak Median = data ke-$\frac{50}{2} = 25$, berada pada kelas $61 - 70$.
  - $L_{me} = 60{,}5$, $\sum f_{k,me} = 18$, $f_{me} = 18$, $p = 10$.

$$
Me = 60{,}5 + \left( \frac{25 - 18}{18} \right) \cdot 10 = 60{,}5 + \frac{70}{18} \approx 60{,}5 + 3{,}89 = 64{,}39\text{ menit}
$$

- **Langkah 4: Menghitung Modus ($Mo$):**
  - Kelas modus memiliki $f$ terbesar ($18$), yaitu kelas $61 - 70$.
  - $L_{mo} = 60{,}5$, $d_1 = 18 - 12 = 6$, $d_2 = 18 - 10 = 8$, $p = 10$.

$$
Mo = 60{,}5 + \left( \frac{6}{6 + 8} \right) \cdot 10 = 60{,}5 + \frac{60}{14} \approx 60{,}5 + 4{,}29 = 64{,}79\text{ menit}
$$

- **Langkah 5: Menghitung Kuartil Atas ($Q_3$):**
  - Letak $Q_3 = \frac{3}{4} \times 50 = 37{,}5$, berada pada kelas $71 - 80$.
  - $L_{Q_3} = 70{,}5$, $\sum f_{k,Q_3} = 36$, $f_{Q_3} = 10$, $p = 10$.

$$
Q_3 = 70{,}5 + \left( \frac{37{,}5 - 36}{10} \right) \cdot 10 = 70{,}5 + 1{,}5 = 72{,}0\text{ menit}
$$

- **Langkah 6: Menghitung Simpangan Baku ($S$) dan Koefisien Variasi ($KV$):**

$$
S^2 = \frac{6.130}{50} = 122{,}6 \implies S = \sqrt{122{,}6} \approx 11{,}07\text{ menit}
$$

$$
KV = \frac{S}{\bar{x}} \times 100\% = \frac{11{,}07}{64{,}3} \times 100\% \approx 17{,}22\%
$$

- **Kesimpulan:**  
  Rata-rata durasi muthala'ah adalah $64{,}3\text{ menit}$, median $64{,}39\text{ menit}$, modus $64{,}79\text{ menit}$, dan simpangan baku $11{,}07\text{ menit}$. Nilai $KV = 17{,}22\%$ menunjukkan durasi belajar santri tergolong cukup homogen ($\checkmark\ \text{Benar}$).

---

### 5. Penerapan Kontekstual (Studi Kasus Santri & Kehidupan Nyata)

#### Evaluasi Komparatif Capaian Tasmi' Al-Qur'an Antar-Halaqah Santri
> Lembaga Pengembangan Tahfizul Qur'an Pesantren mengaudit capaian hafalan (dalam satuan juz) dari santri tingkat akhir di dua halaqah pembinaan, yaitu **Halaqah Utsman** ($30$ santri) dan **Halaqah Ali** ($30$ santri).
> 
> Ringkasan parameter statistik yang diperoleh dari pengolahan data riil adalah sebagai berikut:
> - **Halaqah Utsman**:
>   - Rata-rata ($\bar{x}_1$) = $23\text{ juz}$
>   - Median ($Me_1$) = $23\text{ juz}$
>   - Modus ($Mo_1$) = $23\text{ juz}$
>   - Simpangan Baku ($S_1$) = $2{,}3\text{ juz}$
> - **Halaqah Ali**:
>   - Rata-rata ($\bar{x}_2$) = $23\text{ juz}$
>   - Median ($Me_2$) = $20\text{ juz}$
>   - Modus ($Mo_2$) = $18\text{ juz}$
>   - Simpangan Baku ($S_2$) = $5{,}8\text{ juz}$

**Analisis Evaluasi Berbasis Data:**

1. **Analisis Bentuk Sebaran (*Skewness*):**
   - Pada **Halaqah Utsman**, nilai $\bar{x}_1 = Me_1 = Mo_1 = 23\text{ juz}$. Hal ini menunjukkan sebaran data berbentuk **simetris ideal (distribusi normal)**. Prestasi hafalan santri terkonsentrasi merata di sekitar $21 - 25\text{ juz}$.
   - Pada **Halaqah Ali**, berlaku hubungan $Mo_2 \lt Me_2 \lt \bar{x}_2$ ($18 \lt 20 \lt 23$). Hal ini menunjukkan sebaran data **miring ke kanan (*positively skewed*)**. Mayoritas santri di halaqah ini sebenarnya baru menyelesaikan $18 - 20\text{ juz}$, namun rata-rata halaqah terangkat naik oleh segelintir santri istimewa yang telah mengkhatamkan $30\text{ juz}$.

2. **Evaluasi Dispersi & Homogenitas:**

$$
KV_{\text{Utsman}} = \frac{2{,}3}{23} \times 100\% = 10{,}0\%
$$

$$
KV_{\text{Ali}} = \frac{5{,}8}{23} \times 100\% \approx 25{,}22\%
$$

3. **Keputusan Manajerial Pesantren yang Berkeadilan:**
   - Menghindari kesalahan persepsi: Meskipun kedua halaqah memiliki rata-rata hafalan yang sama ($23\text{ juz}$), kondisi nyata santri di dalamnya sangat berbeda.
   - **Rekomendasi Halaqah Utsman**: Program pembinaan reguler dapat dilanjutkan dengan fokus pada muraja'ah mutqin terpadu.
   - **Rekomendasi Halaqah Ali**: Diperlukan program pendampingan khusus (*tahsin wa ziyadah intensif*) bagi mayoritas santri yang berada di bawah $20\text{ juz}$, serta mengikutsertakan santri yang sudah $30\text{ juz}$ sebagai tutor sebaya (*peer-tutor*).

---

### 6. Pola Kunci & Cara Cepat Mengingat

- **Prinsip "Tepi dan Selisih" pada Modus:**
  > *"Tepi bawah ditambah perbandingan selisih frekuensi atas terhadap total selisih, kali panjang kelas."*

$$
Mo = L + \left( \frac{d_1}{d_1 + d_2} \right) p
$$

- **Prinsip "Kurang dari Frekuensi Kumulatif" pada Fraktil:**
  > *"Letak dikurangi frekuensi kumulatif sebelumnya, dibagi frekuensi kelasnya, dikalikan panjang kelas."*

$$
\text{Fraktil} = L + \left( \frac{\text{Posisi} - \sum f_k}{f} \right) p
$$

- **Invariansi Ukuran Sebaran Terhadap Pergeseran:**
  > *"Jika seluruh data ditambah atau dikurang angka yang sama, lebar sebaran data tidak berubah sedikit pun ($S_{\text{baru}} = S_{\text{lama}}$). Namun jika dikali atau dibagi, ukuran sebaran ikut membesar atau mengecil secara proporsional."*

- **Checklist Verifikasi Mandiri Sebelum Mengakhiri Ujian (Sanity Check):**
  1. Apakah nilai Median dan Modus berada di dalam rentang kelas interval yang dipilih? (Jika kelas $61 - 70$, nilai hasil hitung wajib berada di antara $60{,}5$ dan $70{,}5$).
  2. Apakah nilai Simpangan Kuartil $Q_d \le \text{Jangkauan } R$?
  3. Apakah tanda $Z$-score konsisten dengan posisinya terhadap rata-rata? (Positif jika $x \gt \bar{x}$, nol jika $x = \bar{x}$, negatif jika $x \lt \bar{x}$).

---

### 7. Latihan Soal

---

#### Latihan Soal 1: Pemahaman Konsep, Karakteristik Distribusi, & Data Tunggal (20 Soal)

**A. Pemahaman Konsep & Sifat Statistik**
1. Jelaskan perbedaan mendasar antara kurva ogive positif dan kurva ogive negatif ditinjau dari jenis frekuensi kumulatif yang digunakan!
2. Suatu kumpulan data memiliki nilai rata-rata $72$, median $75$, dan modus $80$. Tentukan bentuk kemiringan kurva distribusi frekuensi dari data tersebut beserta artinya!
3. Jika setiap data pada suatu kelompok dikalikan $3$ kemudian dikurangi $15$, bagaimanakah perubahan yang terjadi pada nilai rata-rata dan simpangan bakunya?
4. Mengapa simpangan kuartil ($Q_d$) dianggap sebagai ukuran penyebaran yang lebih tepat daripada simpangan baku ($S$) ketika data memuat nilai ekstrem (*pencilan*)?

**B. Operasi Hitung Data Tunggal**  
*(Petunjuk: Diberikan data skor tes nahwu santri: $7, \ 5, \ 8, \ 9, \ 7, \ 6, \ 10, \ 7, \ 8, \ 6$. Hitunglah butir nomor 5–14)*
5. Nilai rata-rata hitung ($\bar{x}$) dari data tersebut.
6. Nilai median ($Me$) dari data tersebut.
7. Nilai modus ($Mo$) dari data tersebut.
8. Jangkauan ($R$) dari data tersebut.
9. Kuartil pertama / kuartil bawah ($Q_1$).
10. Kuartil ketiga / kuartil atas ($Q_3$).
11. Jangkauan antarkuartil / hamparan ($H$) dan simpangan kuartil ($Q_d$).
12. Nilai Desil ke-$6$ ($D_6$).
13. Simpangan rata-rata ($SR$).
14. Varians ($S^2$) dan simpangan baku ($S$).

**C. Variasi Aljabar & Komparasi Relatif**
15. Diberikan sekumpulan data: $4, \ 6, \ 8, \ x, \ 10$. Jika rata-rata dari data tersebut adalah $7$, tentukan nilai $x$ dan nilai simpangan bakunya!
16. Sekumpulan data berukuran $n = 8$ memiliki rata-rata $15$ dan simpangan baku $3$. Jika setiap nilai data dikalikan $2$ lalu ditambah $5$, tentukan rata-rata dan simpangan baku yang baru!
17. Diketahui seorang santri bernama Umar memperoleh skor tes fiqih $85$. Jika rata-rata kelas adalah $75$ dengan simpangan baku $8$, hitunglah angka baku ($Z$-score) Umar!
18. Santri bernama Khalid memperoleh nilai $80$ pada ujian tafsir (rata-rata kelas $70, S = 5$) dan nilai $88$ pada ujian hadis (rata-rata kelas $80, S = 8$). Pada mata pelajaran manakah prestasi Khalid relatif lebih unggul terhadap teman sekelasnya?
19. Kelas A memiliki rata-rata nilai hafalan $80$ dengan $S = 4$, sedangkan Kelas B memiliki rata-rata $70$ dengan $S = 7$. Hitunglah Koefisien Variasi ($KV$) masing-masing kelas dan simpulkan kelas manakah yang lebih homogen!
20. Lima orang santri memiliki berat badan: $48, \ 52, \ 56, \ 60, \ 64\text{ kg}$. Tentukan nilai ragam ($S^2$) dari data berat badan tersebut!

---

#### Latihan Soal 2: Pengolahan Tabel Frekuensi, Ogive, & Data Berkelompok (20 Soal)

**A. Aturan Sturges & Interpretasi Tabel**
1. Sebanyak $100$ data mentah waktu muthala'ah santri akan disajikan dalam tabel distribusi frekuensi kelompok. Berdasarkan Aturan Sturges ($\log 100 = 2$), tentukan banyak kelas interval ideal yang harus dibuat!
2. Jika suatu tabel distribusi frekuensi memiliki kelas interval $55 - 63$, tentukan:
   - Batas bawah dan batas atas kelas.
   - Tepi bawah dan tepi atas kelas.
   - Titik tengah kelas ($x_i$).
   - Panjang kelas ($p$).
3. Suatu kurva ogive positif menunjukkan bahwa frekuensi kumulatif kurang dari nilai tepi atas $70{,}5$ adalah $32$ dari total $40$ santri. Tentukan persentase santri yang memperoleh nilai lebih dari $70{,}5$!
4. Jelaskan langkah menentukan titik potong antara kurva ogive positif dan ogive negatif, serta parameter pemusatan apa yang diperoleh dari absis titik potong tersebut!

**B. Komputasi Data Berkelompok**  
*(Petunjuk: Perhatikan tabel distribusi frekuensi skor tes tajwid santri berikut untuk menjawab soal nomor 5–14)*

| Skor Ujian | Frekuensi ($f_i$) |
| :---: | :---: |
| $51 - 60$ | $5$ |
| $61 - 70$ | $8$ |
| $71 - 80$ | $15$ |
| $81 - 90$ | $12$ |
| $91 - 100$ | $10$ |

5. Tentukan total frekuensi ($n$) dan susunlah kolom frekuensi kumulatif kurang dari ($\le$)!
6. Hitunglah nilai rata-rata hitung ($\bar{x}$) menggunakan metode titik tengah!
7. Tentukan kelas median dan hitunglah nilai Median ($Me$) data tersebut!
8. Tentukan kelas modus dan hitunglah nilai Modus ($Mo$) data tersebut!
9. Hitunglah nilai Kuartil Bawah ($Q_1$)!
10. Hitunglah nilai Kuartil Atas ($Q_3$)!
11. Tentukan nilai Simpangan Kuartil ($Q_d$) dari tabel tersebut!
12. Hitunglah nilai Desil ke-$4$ ($D_4$)!
13. Hitunglah nilai Persentil ke-$80$ ($P_{80}$)!
14. Hitunglah nilai Varians ($S^2$) dan Simpangan Baku ($S$) dari tabel tersebut!

**C. Analisis Lanjutan & Kurva Distribusi**
15. Berdasarkan hasil perhitungan nilai $\bar{x}, Me,$ dan $Mo$ pada tabel di atas, simpulkan bentuk kemiringan kurva distribusinya (*skewness*)!
16. Jika batas nilai kelulusan minimal (KKM) tes tajwid ditetapkan sebesar $75{,}5$, tentukan estimasi banyak santri yang dinyatakan lulus KKM menggunakan rumus interpolasi!
17. Pengurus pesantren memberikan beasiswa kitab gratis kepada $15\%$ santri dengan nilai tertinggi. Tentukan batas nilai terendah untuk mendapatkan beasiswa tersebut (gunakan Persentil ke-$85$)!
18. Diberikan histogram dengan nilai tepi-tepi kelas: $29{,}5; \ 39{,}5; \ 49{,}5; \ 59{,}5; \ 69{,}5$ dengan frekuensi berturut-turut $4, \ 11, \ 15, \ 10$. Tentukan nilai Modus dari data histogram tersebut!
19. Tentukan Koefisien Variasi ($KV$) dari data berkelompok pada tabel soal nomor 5–14 di atas!
20. Jika seluruh frekuensi pada tabel di atas dikalikan $2$ (proporsi frekuensi tetap sama), apakah nilai Mean, Median, dan Simpangan Bakunya akan berubah? Jelaskan secara analitis!

---

#### Latihan Soal 3: Studi Kasus Kontekstual Santri & Pemecahan Masalah Nyata Pesantren (20 Soal)

1. Santri bagian logistik menimbang karung beras kiriman wali santri (dalam kg): $48, 50, 50, 52, 53, 54, 55, 58$. Tentukan rata-rata dan jangkauan antarkuartil berat karung beras tersebut!
2. Pengurus kamar mendata waktu tidur malam santri (dalam menit setelah pukul 22.00): $10, 15, 15, 20, 25, 30, 45$. Tentukan nilai median dan simpangan rata-rata waktu tidur santri!
3. Dapur umum pesantren mencatat volume konsumsi minyak goreng (dalam liter per hari) selama $8$ hari: $12, 14, 15, 15, 16, 17, 18, 21$. Hitunglah varians dan simpangan baku konsumsi minyak goreng!
4. Pengurus poskestren mengukur suhu tubuh santri yang mengalami flu: $36{,}8; \ 37{,}2; \ 37{,}5; \ 37{,}5; \ 38{,}0; \ 38{,}4^\circ\text{C}$. Tentukan modus dan simpangan kuartil data suhu tersebut!
5. Santri pecinta kebun pondok mencatat hasil panen buah tin (dalam kg per pekan) selama $7$ pekan: $14, 18, 20, 22, 25, 28, 33$. Tentukan nilai Kuartil Atas ($Q_3$) dan Desil ke-$7$ ($D_7$) hasil panen!
6. Pengurus perpustakaan mencatat jumlah santri yang meminjam kitab per hari selama $10$ hari: $12, 15, 18, 20, 20, 22, 25, 28, 30, 35$. Tentukan nilai simpangan rata-rata peminjam kitab!
7. Panitia peringatan hari santri mendata donasi infak sukarela dari $6$ alumni: $\text{Rp}100.000, \text{Rp}150.000, \text{Rp}150.000, \text{Rp}200.000, \text{Rp}250.000, \text{Rp}350.000$. Tentukan rata-rata dan simpangan baku nominal infak tersebut!
8. Santri piket kebersihan mengukur durasi membersihkan halaman masjid (dalam menit) selama $6$ kali tugas: $25, 30, 35, 40, 45, 65$. Tentukan nilai rata-rata dan tunjukkan nilai pencilan (*outlier*) yang mempengaruhi rata-rata tersebut!
9. Nilai ujian musabaqah hifdzil Qur'an santri memiliki rata-rata $82$ dengan simpangan baku $6$. Seorang santri bernama Hasan memperoleh skor $94$. Tentukan nilai $Z$-score Hasan dan berikan interpretasinya!
10. Pengurus halaqah tahfiz membandingkan hafalan santri di dua kamar:
    - Kamar Al-Fatih: Rata-rata hafalan $= 18\text{ juz}$ dengan $S = 2\text{ juz}$
    - Kamar An-Nasr: Rata-rata hafalan $= 18\text{ juz}$ dengan $S = 5\text{ juz}$  
    - Tentukan kamar manakah yang memiliki hafalan santri lebih merata dan teratur!
11. Toko Kitab Pesantren mendata jumlah pembelian mushaf Al-Qur'an selama $40$ hari yang dikelompokkan ke dalam tabel:

| Jumlah Mushaf | Hari ($f_i$) |
| :---: | :---: |
| $1 - 5$ | $6$ |
| $6 - 10$ | $14$ |
| $11 - 15$ | $12$ |
| $16 - 20$ | $8$ |

Tentukan rata-rata harian pembelian mushaf Al-Qur'an!
12. Dari data tabel pada soal nomor 11, tentukan nilai Median dari jumlah penjualan mushaf Al-Qur'an!
13. Dari data tabel pada soal nomor 11, tentukan nilai Modus dari jumlah penjualan mushaf Al-Qur'an!
14. Unit wirausaha peternakan pesantren mendata produksi susu kambing etawa (dalam liter per hari) selama $30$ hari:

| Produksi (Liter) | Frekuensi ($f_i$) |
| :---: | :---: |
| $11 - 15$ | $4$ |
| $16 - 20$ | $10$ |
| $21 - 25$ | $11$ |
| $26 - 30$ | $5$ |

Tentukan nilai Kuartil Bawah ($Q_1$) produksi susu kambing!
15. Dari data tabel soal nomor 14, tentukan nilai Kuartil Atas ($Q_3$) produksi susu kambing!
16. Dari data tabel soal nomor 14, tentukan simpangan kuartil ($Q_d$) produksi susu kambing!
17. Panitia wisuda santri mendata tinggi badan (dalam cm) dari $40$ santri calon wisudawan:

| Tinggi Badan (cm) | Frekuensi ($f_i$) |
| :---: | :---: |
| $151 - 155$ | $4$ |
| $156 - 160$ | $10$ |
| $161 - 165$ | $16$ |
| $166 - 170$ | $7$ |
| $171 - 175$ | $3$ |

Tentukan nilai Modus tinggi badan santri calon wisudawan!
18. Dari data tabel soal nomor 17, tentukan nilai rata-rata tinggi badan santri!
19. Santri pengelola poskestren mencatat berat badan santri baru di asrama: nilai rata-rata berat badan adalah $55\text{ kg}$ dengan simpangan baku $5\text{ kg}$. Jika seorang santri bernama Abdullah memiliki $Z$-score sebesar $-1{,}4$, berapakah berat badan Abdullah sesungguhnya?
20. Dua kelompok santri mengikuti pembekalan da'i muda. Kelompok pertama memiliki rata-rata waktu ceramah $20\text{ menit}$ dengan $S = 3\text{ menit}$. Kelompok kedua memiliki rata-rata waktu ceramah $30\text{ menit}$ dengan $S = 4{,}2\text{ menit}$. Hitunglah Koefisien Variasi masing-masing kelompok dan tentukan kelompok mana yang lebih konsisten durasi ceramahnya!

---

### 8. Pekerjaan Rumah (PR Pondok / Remedial & Pengayaan Mandiri)

**Petunjuk Pengerjaan:**
- Kerjakan di buku catatan tugas matematika secara mandiri, runtut, dan rapi.
- Tuliskan apa yang diketahui, rumus statistika yang digunakan, serta langkah komputasi baris demi baris.

1. **Komputasi Lengkap Data Tunggal Acak:**  
   Diberikan data nilai setoran hafalan nadzam *Imrithi* dari $12$ santri:

$$
65, \ 78, \ 82, \ 60, \ 95, \ 74, \ 85, \ 70, \ 78, \ 88, \ 78, \ 90
$$

   Tentukan nilai Mean, Median, Modus, Kuartil Bawah ($Q_1$), Kuartil Atas ($Q_3$), Simpangan Kuartil ($Q_d$), Simpangan Rata-rata ($SR$), dan Simpangan Baku ($S$)!

2. **Rekonstruksi Data dari Tabel Distribusi Frekuensi:**  
   Perhatikan tabel nilai ujian tafsir santri berikut:

| Rentang Nilai | Frekuensi ($f_i$) |
| :---: | :---: |
| $45 - 54$ | $4$ |
| $55 - 64$ | $8$ |
| $65 - 74$ | $14$ |
| $75 - 84$ | $10$ |
| $85 - 94$ | $4$ |

   - Tentukan nilai Mean, Median, dan Modusnya!  
   - Tentukan nilai Persentil ke-$75$ ($P_{75}$)!  
   - Berdasarkan nilai Mean, Median, dan Modus, bagaimanakah bentuk kurva kemiringannya? Jelaskan artinya bagi evaluasi pengajar!

3. **Studi Kasus Komparasi Kedisiplinan Dua Asrama Santri:**  
   Pembina asrama mendata poin pelanggaran kedisiplinan santri selama satu semester:
   - **Asrama Al-Farabi**: Rata-rata poin $= 14$ dengan simpangan baku $S = 2{,}1$
   - **Asrama Ibnu Rusyd**: Rata-rata poin $= 14$ dengan simpangan baku $S = 6{,}3$  
   - Hitunglah Koefisien Variasi ($KV$) masing-masing asrama!  
   - Asrama manakah yang memiliki kedisiplinan santri lebih merata dan teratur? Berikan rekomendasi langkah pembinaan asrama yang adil dan mendidik!

4. **Pertanyaan Reflektif & Pemahaman Konsep:**  
   *Jelaskan hubungan filosofis antara hisab yang adil dalam pandangan Islam dengan pentingnya menyajikan ukuran pemusatan (Mean/Median) secara berdampingan dengan ukuran penyebaran (Simpangan Baku/Varians)! Mengapa seorang pengambil kebijakan di pesantren tidak boleh hanya mengandalkan nilai rata-rata semata?*

---

### 9. Ringkasan Materi

- **Hakikat Evaluasi Statistika Deskriptif**: Mengukur ketercapaian belajar secara jujur dan objektif, mengintegrasikan kemampuan penyajian (tabel dan kurva ogive), ukuran pemusatan (Mean, Median, Modus), ukuran letak (Kuartil, Desil, Persentil), serta ukuran penyebaran (Varians, Simpangan Baku, $Z$-Score, dan $KV$).
- **Invariansi Dispersi**: Ukuran pemusatan dan ukuran letak peka terhadap penambahan maupun perkalian konstanta. Sebaliknya, ukuran penyebaran ($R, Q_d, SR, S$) **kebal (tidak berubah)** jika data ditambah/dikurangi konstanta, namun membesar/mengecil proporsional jika data dikali/dibagi konstanta.
- **Deteksi Kemiringan Sebaran (*Skewness*)**: Posisi relatif ketiga nilai pusat menentukan bentuk kurva: simetris jika $\bar{x} \approx Me \approx Mo$, miring ke kanan (*positively skewed*) jika $Mo \lt Me \lt \bar{x}$, dan miring ke kiri (*negatively skewed*) jika $\bar{x} \lt Me \lt Mo$.
- **Keadilan Hisab Berbasis Data**: Statistika deskriptif menuntun santri untuk menegakkan kejujuran ilmiah, ketelitian hisab amal, dan objektivitas evaluasi demi kemaslahatan bersama di pondok pesantren.
