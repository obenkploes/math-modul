# MATEMATIKA SMA (JURUSAN IPA & PESANTREN)
## Kelas 12 - Semester Ganjil
### Pertemuan 8: Statistika Deskriptif — Ukuran Penyebaran Data

---

### 1. Pengertian & Konsep Dasar

Dalam analisis statistika, mengetahui nilai ukuran pemusatan (seperti Mean, Median, dan Modus) saja belum cukup untuk menggambarkan karakteristik suatu kelompok data secara utuh. Dua kelompok data bisa saja memiliki nilai rata-rata yang sama persis, namun memiliki sebaran data yang sangat berbeda.

Oleh karena itu, diperlukan **Ukuran Penyebaran Data (*Measures of Dispersion / Variability*)**, yaitu ukuran statistik yang menunjukkan seberapa jauh nilai-nilai data menyebar, menyimpang, atau merentang dari nilai pusatnya (terutama dari nilai rata-rata hitung / Mean).

Secara filosofis dan teologis, ukuran penyebaran data mengajarkan kita tentang **hikmah keadilan, kesetaraan, dan pemerataan ikhtiar dalam sunnatullah**. 
- Bayangkan dua kelompok halaqah santri yang sama-sama memiliki rata-rata hafalan Al-Qur'an $15\text{ juz}$.
- Pada kelompok pertama, seluruh santri hafal antara $14$ hingga $16\text{ juz}$ (**sebaran sempit / homogen**).
- Pada kelompok kedua, ada santri yang baru hafal $2\text{ juz}$ dan ada yang sudah hafal $28\text{ juz}$ (**sebaran lebar / heterogen**).
- Meskipun nilai rata-ratanya sama, potret keadilan proses belajar dan pemerataan capaian kedua kelompok tersebut sangat berbeda. Di sinilah ukuran penyebaran data berfungsi sebagai tolok ukur **tingkat homogenitas dan konsistensi data**.

---

### 2. Bentuk Umum & Rumus Baku

Ukuran penyebaran data dibedakan menjadi ukuran penyebaran sederhana (berdasarkan posisi urutan) dan ukuran penyebaran berbasis simpangan rata-rata/kuadrat.

#### A. Ukuran Penyebaran Sederhana

1. **Jangkauan / Rentang (*Range* - $R$):**
   Selisih antara nilai data terbesar ($X_{\max}$) dengan nilai data terkecil ($X_{\min}$):



R = X_{\max} - X_{\min}


2. **Jangkauan Antarkuartil / Hamparan ($H$):**
   Selisih antara kuartil atas ($Q_3$) dengan kuartil bawah ($Q_1$):



H = Q_3 - Q_1


3. **Simpangan Kuartil / Jangkauan Semi-Interkuartil ($Q_d$):**
   Setengah dari nilai jangkauan antarkuartil:



Q_d = \frac{1}{2} H = \frac{1}{2}(Q_3 - Q_1)


---

#### B. Simpangan Rata-Rata (*Mean Deviation* - $SR$)

Simpangan rata-rata mengukur rata-rata jarak mutlak setiap data terhadap nilai rata-rata hitungnya ($\bar{x}$).

1. **Untuk Data Tunggal:**



SR = \frac{\sum_{i=1}^n \lvert x_i - \bar{x} \rvert}{n}


2. **Untuk Data Berkelompok (Tabel Distribusi Frekuensi):**



SR = \frac{\sum_{i=1}^k f_i \lvert x_i - \bar{x} \rvert}{\sum_{i=1}^k f_i}


---

#### C. Ragam / Varians ($S^2$) dan Simpangan Baku / Standar Deviasi ($S$)

Varians adalah rata-rata kuadrat deviasi setiap data terhadap rata-rata hitungnya. Simpangan baku adalah akar kuadrat positif dari varians, yang memiliki satuan yang sama dengan satuan data aslinya.

1. **Untuk Data Tunggal:**
   - **Ragam / Varians ($S^2$):**



S^2 = \frac{\sum_{i=1}^n (x_i - \bar{x})^2}{n}


   - **Simpangan Baku ($S$):**



S = \sqrt{S^2} = \sqrt{\frac{\sum_{i=1}^n (x_i - \bar{x})^2}{n}}


2. **Untuk Data Berkelompok (Tabel Distribusi Frekuensi):**
   - **Ragam / Varians ($S^2$):**



S^2 = \frac{\sum_{i=1}^k f_i (x_i - \bar{x})^2}{\sum_{i=1}^k f_i}


   - **Simpangan Baku ($S$):**



S = \sqrt{S^2} = \sqrt{\frac{\sum_{i=1}^k f_i (x_i - \bar{x})^2}{\sum_{i=1}^k f_i}}


**Keterangan Simbol:**
- $n$: Banyaknya seluruh data ($\sum f_i$).
- $k$: Banyaknya kelas interval pada data berkelompok.
- $x_i$: Nilai data ke-$i$ (pada data tunggal) atau nilai titik tengah kelas ke-$i$ (pada data berkelompok, $x_i = \frac{\text{Batas Bawah} + \text{Batas Atas}}{2}$).
- $f_i$: Frekuensi kelas interval ke-$i$.
- $\bar{x}$: Nilai rata-rata hitung (*Mean*).

---

### 3. Sifat-Sifat, Karakteristik, & Aturan Khusus

#### A. Karakteristik Homogenitas Data
- **Nilai $S$ atau $S^2$ Kecil (Mendekati $0$):** Menunjukkan bahwa data terkonsentrasi sangat dekat dengan nilai rata-rata. Data bersifat **homogen** (seragam/konsisten).
- **Nilai $S$ atau $S^2$ Besar:** Menunjukkan bahwa data tersebar jauh dari nilai rata-rata. Data bersifat **heterogen** (bervariasi/timpang).
- Nilai $SR, S^2,$ dan $S$ selalu bernilai **non-negatif** ($\ge 0$). Nilai nol hanya tercapai jika seluruh data bernilai sama persis ($x_1 = x_2 = \dots = x_n$).

#### B. Pengaruh Transformasi Linier Data Terhadap Ukuran Penyebaran
Misalkan sekumpulan data awal $x_i$ memiliki jangkauan $R_x$, simpangan rata-rata $SR_x$, varians $S_x^2$, dan simpangan baku $S_x$. Jika setiap nilai data diubah melalui operasi linier:



y_i = a x_i + b \quad (a, b \in \mathbb{R})


Maka ukuran statistik yang baru berubah dengan aturan berikut:

| Ukuran Statistik | Data Asli ($x$) | Data Baru ($y = a x + b$) | Keterangan Efek Operasi |
| :--- | :---: | :---: | :--- |
| **Rata-rata (Mean)** | $\bar{x}$ | $\bar{y} = a \bar{x} + b$ | Dipengaruhi perkalian dan penjumlahan |
| **Jangkauan ($R$)** | $R_x$ | $R_y = \lvert a \rvert \cdot R_x$ | **Hanya dipengaruhi perkalian**, tidak terpengaruh pergeseran $b$ |
| **Hamparan ($H$)** | $H_x$ | $H_y = \lvert a \rvert \cdot H_x$ | **Hanya dipengaruhi perkalian**, tidak terpengaruh pergeseran $b$ |
| **Simpangan Kuartil ($Q_d$)** | $Q_{d,x}$ | $Q_{d,y} = \lvert a \rvert \cdot Q_{d,x}$ | **Hanya dipengaruhi perkalian**, tidak terpengaruh pergeseran $b$ |
| **Simpangan Rata-rata ($SR$)** | $SR_x$ | $SR_y = \lvert a \rvert \cdot SR_x$ | **Hanya dipengaruhi perkalian**, tidak terpengaruh pergeseran $b$ |
| **Simpangan Baku ($S$)** | $S_x$ | $S_y = \lvert a \rvert \cdot S_x$ | **Hanya dipengaruhi perkalian**, tidak terpengaruh pergeseran $b$ |
| **Ragam / Varians ($S^2$)** | $S_x^2$ | $S_y^2 = a^2 \cdot S_x^2$ | **Terkali dengan kuadrat faktor pengali $a^2$** |

---

### 4. Contoh Soal & Pembahasan Terperinci

#### Contoh 1 (Tingkat Dasar: Ukuran Penyebaran Data Tunggal)
**Soal:**
Diberikan data nilai ujian tasmi' Al-Qur'an dari $8$ orang santri sebagai berikut:



4, \ 6, \ 6, \ 7, \ 8, \ 9, \ 10, \ 14

Tentukan:
a. Jangkauan ($R$), Jangkauan Antarkuartil ($H$), dan Simpangan Kuartil ($Q_d$).  
b. Simpangan Rata-rata ($SR$).  
c. Ragam ($S^2$) dan Simpangan Baku ($S$).

**Penyelesaian:**
- **Diketahui:**
  Data terurut: $4, 6, 6, 7, 8, 9, 10, 14$ dengan $n = 8$.
- **Ditanyakan:**
  $R, H, Q_d, SR, S^2,$ dan $S$.
- **Langkah Penyelesaian:**
  1. *Menghitung Nilai Rata-rata ($\bar{x}$):*



\bar{x} = \frac{4 + 6 + 6 + 7 + 8 + 9 + 10 + 14}{8} = \frac{64}{8} = 8


  2. *Menghitung $R, H,$ dan $Q_d$:*
     - $X_{\max} = 14$ dan $X_{\min} = 4 \implies R = 14 - 4 = 10$.
     - Letak kuartil untuk $n = 8$:
       - Paruh bawah: $4, 6, 6, 7 \implies Q_1 = \frac{6 + 6}{2} = 6$.
       - Paruh atas: $8, 9, 10, 14 \implies Q_3 = \frac{9 + 10}{2} = 9{,}5$.
     - Hamparan ($H$):



H = Q_3 - Q_1 = 9{,}5 - 6 = 3{,}5


     - Simpangan Kuartil ($Q_d$):



Q_d = \frac{1}{2} H = \frac{1}{2}(3{,}5) = 1{,}75


  3. *Menghitung Simpangan Rata-rata ($SR$):*
     Daftar nilai mutlak deviasi $\lvert x_i - \bar{x} \rvert$:
     - $\lvert 4 - 8 \rvert = 4$
     - $\lvert 6 - 8 \rvert = 2$
     - $\lvert 6 - 8 \rvert = 2$
     - $\lvert 7 - 8 \rvert = 1$
     - $\lvert 8 - 8 \rvert = 0$
     - $\lvert 9 - 8 \rvert = 1$
     - $\lvert 10 - 8 \rvert = 2$
     - $\lvert 14 - 8 \rvert = 6$



\sum_{i=1}^8 \lvert x_i - \bar{x} \rvert = 4 + 2 + 2 + 1 + 0 + 1 + 2 + 6 = 18




SR = \frac{18}{8} = 2{,}25


  4. *Menghitung Ragam ($S^2$) dan Simpangan Baku ($S$):*
     Kuadrat masing-masing deviasi $(x_i - \bar{x})^2$:
     - $(4 - 8)^2 = 16$
     - $(6 - 8)^2 = 4$
     - $(6 - 8)^2 = 4$
     - $(7 - 8)^2 = 1$
     - $(8 - 8)^2 = 0$
     - $(9 - 8)^2 = 1$
     - $(10 - 8)^2 = 4$
     - $(14 - 8)^2 = 36$



\sum_{i=1}^8 (x_i - \bar{x})^2 = 16 + 4 + 4 + 1 + 0 + 1 + 4 + 36 = 66




S^2 = \frac{66}{8} = 8{,}25




S = \sqrt{8{,}25} = \sqrt{\frac{33}{4}} = \frac{\sqrt{33}}{2} \approx 2{,}87

- **Kesimpulan:** 
  $R = 10$, $H = 3{,}5$, $Q_d = 1{,}75$, $SR = 2{,}25$, $S^2 = 8{,}25$, dan $S = \frac{\sqrt{33}}{2} \approx 2{,}87$ ($\checkmark\ \text{Benar}$).

---

#### Contoh 2 (Pengembangan: Ukuran Penyebaran Data Berkelompok)
**Soal:**
Tabel berikut menyajikan data lama waktu muthala'ah (belajar mandiri kitab kuning) harian dari $20$ orang santri:

| Waktu (Menit) | Frekuensi ($f_i$) |
| :---: | :---: |
| $1 - 5$ | $2$ |
| $6 - 10$ | $7$ |
| $11 - 15$ | $8$ |
| $16 - 20$ | $3$ |

Hitunglah nilai Simpangan Rata-rata ($SR$), Ragam ($S^2$), dan Simpangan Baku ($S$) dari data berkelompok tersebut!

**Penyelesaian:**
- **Diketahui:**
  Data berkelompok dengan $n = \sum f_i = 20$.
- **Ditanyakan:**
  $SR$, $S^2$, dan $S$.
- **Langkah Penyelesaian:**
  1. *Susun Tabel Penolong Perhitungan:*

| Kelas | $f_i$ | Titik Tengah ($x_i$) | $f_i x_i$ | $\lvert x_i - \bar{x} \rvert$ | $f_i \lvert x_i - \bar{x} \rvert$ | $(x_i - \bar{x})^2$ | $f_i (x_i - \bar{x})^2$ |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| $1 - 5$ | $2$ | $3$ | $6$ | $\lvert 3 - 11 \rvert = 8$ | $16$ | $64$ | $128$ |
| $6 - 10$ | $7$ | $8$ | $56$ | $\lvert 8 - 11 \rvert = 3$ | $21$ | $9$ | $63$ |
| $11 - 15$ | $8$ | $13$ | $104$ | $\lvert 13 - 11 \rvert = 2$ | $16$ | $4$ | $32$ |
| $16 - 20$ | $3$ | $18$ | $54$ | $\lvert 18 - 11 \rvert = 7$ | $21$ | $49$ | $147$ |
| **Total** | **$\sum f_i = 20$** | — | **$\sum f_i x_i = 220$** | — | **$\sum = 74$** | — | **$\sum = 370$** |

  2. *Hitung Nilai Rata-rata ($\bar{x}$):*



\bar{x} = \frac{\sum f_i x_i}{\sum f_i} = \frac{220}{20} = 11\text{ menit}


  3. *Hitung Simpangan Rata-rata ($SR$):*



SR = \frac{\sum f_i \lvert x_i - \bar{x} \rvert}{\sum f_i} = \frac{74}{20} = 3{,}7\text{ menit}


  4. *Hitung Ragam ($S^2$) dan Simpangan Baku ($S$):*



S^2 = \frac{\sum f_i (x_i - \bar{x})^2}{\sum f_i} = \frac{370}{20} = 18{,}5




S = \sqrt{18{,}5} = \sqrt{\frac{37}{2}} = \frac{\sqrt{74}}{2} \approx 4{,}30\text{ menit}

- **Kesimpulan:** 
  Nilai $SR = 3{,}7\text{ menit}$, Ragam $S^2 = 18{,}5$, dan Simpangan Baku $S = \frac{\sqrt{74}}{2} \approx 4{,}30\text{ menit}$ ($\checkmark\ \text{Benar}$).

---

### 5. Penerapan Kontekstual (Studi Kasus Santri & Kehidupan Nyata)

#### Analisis Komparasi Konsistensi Dua Halaqah Tahfiz Santri
> Pengasuh pondok pesantren mengevaluasi capaian hafalan Al-Qur'an dari dua kelompok halaqah santri tingkat akhir menjelang wisuda tasmi' $30\text{ juz}$. Masing-masing halaqah terdiri atas $10$ orang santri.
> - **Halaqah Al-Fatih**: Memiliki nilai rata-rata hafalan $\bar{x}_1 = 20\text{ juz}$ dengan simpangan baku $S_1 = 1{,}5\text{ juz}$.
> - **Halaqah An-Nur**: Memiliki nilai rata-rata hafalan $\bar{x}_2 = 20\text{ juz}$ dengan simpangan baku $S_2 = 6{,}2\text{ juz}$.
>
> Sebagai santri analis data, tentukan:
> 1. Halaqah manakah yang memiliki capaian hafalan lebih konsisten dan merata (homogen)?
> 2. Berikan interpretasi kondisi riil santri di lapangan berdasarkan data simpangan baku tersebut!

**Langkah Analisis:**

1. **Membandingkan Nilai Simpangan Baku:**
   - Diketahui: $\bar{x}_1 = \bar{x}_2 = 20\text{ juz}$.
   - Simpangan baku: $S_1 = 1{,}5 < S_2 = 6{,}2$.

2. **Interpretasi Statistik:**
   - **Tingkat Homogenitas**: Karena $S_1 < S_2$, maka persebaran data hafalan pada Halaqah Al-Fatih jauh lebih sempit di sekitar nilai rata-rata $20\text{ juz}$. Ini membuktikan bahwa Halaqah Al-Fatih **jauh lebih homogen dan konsisten**.
   - **Potret Kondisi Lapangan**:
     - Pada **Halaqah Al-Fatih** ($S_1 = 1{,}5$), mayoritas santri berada pada rentang hafalan $20 \pm 1{,}5$, yaitu berkisar antara $18{,}5$ hingga $21{,}5\text{ juz}$. Kecepatan belajar antar-santri relatif seragam dan tidak ada yang tertinggal jauh.
     - Pada **Halaqah An-Nur** ($S_2 = 6{,}2$), rentang sebaran hafalan melebar dari $20 \pm 6{,}2$, yaitu sekitar $13{,}8$ hingga $26{,}2\text{ juz}$. Hal ini mengindikasikan adanya kesenjangan (*gap*) yang lebar: sebagian santri sudah melesat mendekati khatam ($30\text{ juz}$), namun ada sebagian santri lain yang masih tertinggal di bawah $14\text{ juz}$.

3. **Rekomendasi Kebijakan Pesantren:**
   Pengasuh asrama perlu memberikan pendampingan khusus (*mentoring*) bagi santri yang tertinggal di Halaqah An-Nur, sedangkan Halaqah Al-Fatih dapat mempertahankan metode belajarnya yang sudah solid dan merata.

---

### 6. Pola Kunci & Cara Cepat Mengingat

- **Alur Kerja Menghitung Simpangan Baku Data Berkelompok:**



\text{Titik Tengah } (x_i) \longrightarrow \bar{x} \longrightarrow \text{Deviasi } (x_i - \bar{x}) \longrightarrow \text{Kuadrat } (x_i - \bar{x})^2 \longrightarrow \text{Kalikan } f_i \longrightarrow \text{Bagi } \sum f_i \longrightarrow \text{Tarik Akar } (S)


- **Jembatan Keledai Efek Transformasi Data ($y = ax + b$):**
  > *"Pusat kena semua ($a$ dan $b$), Sebaran hanya kena kali ($\lvert a \rvert$), Geser ($b$) dicuekin!"*

- **Catatan Waspada (Common Pitfalls):**
  - ⚠️ **Lupa Menarik Akar**: Nilai $\frac{\sum f_i(x_i - \bar{x})^2}{\sum f_i}$ adalah **Ragam / Varians ($S^2$)**, bukan simpangan baku. Untuk mendapatkan simpangan baku ($S$), hasil tersebut **wajib ditarik akarnya**.
  - ⚠️ **Lupa Tanda Mutlak pada $SR$**: Pada simpangan rata-rata, semua deviasi bernilai positif ($\lvert x_i - \bar{x} \rvert$). Jika tanda mutlak diabaikan, jumlah deviasi $\sum f_i(x_i - \bar{x})$ selalu menghasilkan angka nol ($0$).
  - ⚠️ **Transformasi Varians Terkuadratkan**: Ingat bahwa varians data baru adalah $S_y^2 = a^2 \cdot S_x^2$. Jika data dikali $3$, variansnya menjadi $3^2 = 9$ kali lebih besar.

---

### 7. Latihan Soal

---

#### Latihan Soal 1: Ukuran Penyebaran Data Tunggal & Sifat Transformasi Statistik (20 Soal)

**A. Pemahaman Konsep & Sifat Transformasi**
1. Diberikan data: $6, 6, 6, 6, 6$. Tanpa menghitung dengan rumus rumit, tentukan nilai simpangan baku dari data tersebut dan jelaskan alasannya!
2. Jelaskan perbedaan mendasar antara simpangan rata-rata ($SR$) dan simpangan baku ($S$) ditinjau dari cara memperlakukan deviasi bernilai negatif!
3. Sekumpulan data memiliki rata-rata $45$, jangkauan $16$, dan simpangan baku $6$. Jika setiap nilai data dikalikan $2$ kemudian dikurangi $10$, tentukan nilai rata-rata, jangkauan, dan simpangan baku data yang baru!
4. Suatu data memiliki varians $S^2 = 12$. Jika seluruh data dikalikan dengan $-3$ lalu ditambah $15$, tentukan nilai varians dan simpangan baku data yang baru!

**B. Operasi Hitung Data Tunggal**  
*(Petunjuk: Hitunglah nilai $R, H, Q_d, SR, S^2,$ dan $S$ untuk setiap kumpulan data berikut)*
5. Data: $3, 4, 5, 6, 7, 8, 9$
6. Data: $2, 4, 6, 8, 10, 12$
7. Data: $5, 7, 8, 8, 9, 11$
8. Data: $10, 12, 12, 14, 15, 17, 18, 22$
9. Data: $1, 3, 5, 7, 9, 11, 13, 15$
10. Data: $6, 7, 8, 8, 9, 9, 10, 11$
11. Data: $12, 14, 15, 15, 16, 18, 20$
12. Data: $20, 25, 30, 35, 40$
13. Data: $4, 5, 6, 6, 7, 8, 9, 11$
14. Data: $8, 8, 9, 10, 11, 12, 12$

**C. Sifat Aljabar & Penalaran Dispersi**
15. Diketahui lima buah bilangan bulat positif berurutan: $n, n+1, n+2, n+3, n+4$. Tunjukkan bahwa simpangan baku dari kelima bilangan tersebut selalu bernilai $\sqrt{2}$ untuk sembarang nilai $n$!
16. Sekumpulan data berukuran $n = 10$ memiliki nilai $\sum x_i = 120$ dan $\sum x_i^2 = 1.540$. Tentukan nilai ragam ($S^2$) dan simpangan baku ($S$) data tersebut!
17. Diberikan data: $x_1, x_2, x_3, x_4, x_5$ dengan rata-rata $8$ dan varians $4$. Tentukan nilai $\sum_{i=1}^5 x_i^2$!
18. Dari $6$ data pengamatan diperoleh simpangan rata-rata sebesar $3{,}5$. Jika jumlah nilai data adalah $48$, tentukan nilai rata-rata hitung dan jumlah seluruh deviasi mutlaknya!
19. Dua data baru bernilai $10$ dan $10$ ditambahkan ke dalam kumpulan data yang memiliki rata-rata $10$ dan simpangan baku $4$. Selidikilah apakah simpangan baku data yang baru akan membesar, mengecil, atau tetap!
20. Diberikan sekumpulan data dengan jangkauan $R = 24$. Jika data tersebut dikelompokkan ke dalam kelas-kelas interval dengan panjang kelas $p = 5$, tentukan estimasi banyak kelas yang terbentuk berdasarkan aturan jangkauan!

---

#### Latihan Soal 2: Ukuran Penyebaran Data Berkelompok (Tabel Distribusi Frekuensi) (20 Soal)

**A. Pemahaman Konsep Data Berkelompok**
1. Dalam menghitung ukuran penyebaran data berkelompok, mengapa nilai yang digunakan sebagai wakil kelas interval adalah nilai titik tengah ($x_i$)?
2. Tuliskan rumus menentukan titik tengah ($x_i$) dari suatu kelas interval dengan batas bawah $BB$ dan batas atas $BA$!
3. Jelaskan mengapa nilai simpangan baku data berkelompok umumnya merupakan nilai pendekatan (estimasi) dan bukan nilai eksak sebagaimana pada data tunggal aslinya!
4. Pada tabel distribusi frekuensi, jika seluruh frekuensi pada setiap kelas interval digandakan menjadi dua kali lipat ($2f_i$), selidikilah apakah nilai simpangan bakunya berubah!

**B. Operasi Hitung Simpangan Rata-Rata ($SR$) Data Berkelompok**  
*(Petunjuk: Hitunglah nilai Simpangan Rata-rata dari tabel distribusi frekuensi berikut)*
5. 
| Nilai | Frekuensi |
| :---: | :---: |
| $21 - 25$ | $2$ |
| $26 - 30$ | $8$ |
| $31 - 35$ | $6$ |
| $36 - 40$ | $4$ |

6. 
| Nilai | Frekuensi |
| :---: | :---: |
| $10 - 14$ | $4$ |
| $15 - 19$ | $6$ |
| $20 - 24$ | $7$ |
| $25 - 29$ | $3$ |

7. 
| Nilai | Frekuensi |
| :---: | :---: |
| $41 - 45$ | $3$ |
| $46 - 50$ | $5$ |
| $51 - 55$ | $8$ |
| $56 - 60$ | $4$ |

8. 
| Nilai | Frekuensi |
| :---: | :---: |
| $1 - 5$ | $3$ |
| $6 - 10$ | $5$ |
| $11 - 15$ | $10$ |
| $16 - 20$ | $2$ |

9. 
| Nilai | Frekuensi |
| :---: | :---: |
| $50 - 54$ | $4$ |
| $55 - 59$ | $6$ |
| $60 - 64$ | $8$ |
| $65 - 69$ | $2$ |

**C. Operasi Hitung Ragam ($S^2$) dan Simpangan Baku ($S$) Data Berkelompok**  
*(Petunjuk: Lengkapi tabel penolong dan hitung nilai Varians serta Simpangan Baku)*
10. 
| Nilai | Frekuensi |
| :---: | :---: |
| $11 - 15$ | $2$ |
| $16 - 20$ | $5$ |
| $21 - 25$ | $8$ |
| $26 - 30$ | $5$ |

11. 
| Nilai | Frekuensi |
| :---: | :---: |
| $31 - 35$ | $4$ |
| $36 - 40$ | $6$ |
| $41 - 45$ | $7$ |
| $46 - 50$ | $3$ |

12. 
| Nilai | Frekuensi |
| :---: | :---: |
| $5 - 9$ | $3$ |
| $10 - 14$ | $7$ |
| $15 - 19$ | $6$ |
| $20 - 24$ | $4$ |

13. 
| Nilai | Frekuensi |
| :---: | :---: |
| $61 - 65$ | $2$ |
| $66 - 70$ | $8$ |
| $71 - 75$ | $6$ |
| $76 - 80$ | $4$ |

14. 
| Nilai | Frekuensi |
| :---: | :---: |
| $20 - 29$ | $3$ |
| $30 - 39$ | $5$ |
| $40 - 49$ | $8$ |
| $50 - 59$ | $4$ |

15. 
| Nilai | Frekuensi |
| :---: | :---: |
| $40 - 44$ | $2$ |
| $45 - 49$ | $4$ |
| $50 - 54$ | $8$ |
| $55 - 59$ | $4$ |
| $60 - 64$ | $2$ |

16. 
| Nilai | Frekuensi |
| :---: | :---: |
| $70 - 74$ | $3$ |
| $75 - 79$ | $7$ |
| $80 - 84$ | $10$ |
| $85 - 89$ | $6$ |
| $90 - 94$ | $4$ |

17. Dari tabel distribusi frekuensi data berkelompok dengan panjang kelas $p = 5$, diperoleh $\sum f_i = 30$, $\sum f_i x_i = 750$, dan $\sum f_i x_i^2 = 19.350$. Tentukan nilai mean, varians, dan simpangan bakunya!
18. Suatu tabel distribusi frekuensi memiliki nilai rata-rata $\bar{x} = 65$ dan simpangan baku $S = 5$. Jika seluruh tepi kelas ditambah $2$, tentukan nilai rata-rata dan simpangan baku yang baru!
19. Diketahui data berkelompok dengan $\sum f_i = 40$ dan $\sum f_i (x_i - \bar{x})^2 = 640$. Tentukan nilai simpangan baku data tersebut!
20. Sebuah tabel distribusi frekuensi memiliki 5 kelas interval simetris dengan frekuensi berturut-turut $2, 6, 10, 6, 2$ dan titik tengah kelas ketiga adalah $25$. Jika panjang kelas adalah $4$, tentukan nilai varians data tersebut!

---

#### Latihan Soal 3: Penerapan Kontekstual Santri & Pemecahan Masalah Nyata Pesantren (20 Soal)

*(Petunjuk: Selesaikan setiap permasalahan kontekstual santri berikut dengan menganalisis ukuran penyebaran datanya)*

1. Pengasuh halaqah tahfiz mencatat jumlah ayat hafalan baru yang disetorkan $7$ orang santri pada hari Senin: $12, 14, 15, 15, 16, 18, 22$ ayat. Tentukan jangkauan, simpangan rata-rata, dan simpangan bakunya!
2. Nilai tes membaca kitab kuning gundul (fathul qorib) dari $6$ orang santri asrama adalah: $75, 78, 80, 82, 85, 92$. Hitunglah varians dan simpangan baku nilai ujian tersebut!
3. Dua kelompok kamar asrama santri mengikuti lomba kebersihan kamar mingguan dengan catatan nilai selama $5$ pekan:
   - Kamar Abu Bakar: $80, 82, 84, 86, 88$
   - Kamar Umar bin Khattab: $74, 80, 85, 90, 91$  
   Tentukan rata-rata dan simpangan baku masing-masing kamar, lalu tentukan kamar manakah yang paling konsisten menjaga kebersihan!
4. Santri piket mencatat durasi waktu (dalam menit) bangun sebelum azan subuh untuk melaksanakan salat tahajud dari $8$ santri: $20, 25, 30, 30, 35, 40, 45, 55\text{ menit}$. Tentukan jangkauan antarkuartil dan simpangan kuartilnya!
5. Pengurus dapur umum menimbang berat beras (dalam kg) yang dimasak per hari selama sepekan: $45, 48, 50, 50, 52, 54, 58\text{ kg}$. Tentukan simpangan rata-rata kebutuhan beras harian tersebut!
6. Catatan waktu santri menyelesaikan tasmi' hafalan $1\text{ juz}$ sekali duduk (dalam menit) dari $6$ santri adalah: $42, 45, 48, 50, 52, 57\text{ menit}$. Hitunglah simpangan baku durasi tasmi' santri!
7. Sebanyak $30$ orang santri mengikuti ujian kosakata mufradat bahasa Arab dengan distribusi frekuensi sebagai berikut:

| Skor Mufradat | Frekuensi |
| :---: | :---: |
| $61 - 70$ | $5$ |
| $71 - 80$ | $12$ |
| $81 - 90$ | $9$ |
| $91 - 100$ | $4$ |

Tentukan simpangan rata-rata dari skor mufradat santri tersebut!
8. Berdasarkan data tabel pada soal nomor 7, hitunglah nilai ragam dan simpangan bakunya!
9. Pengurus poskestren mendata suhu tubuh (dalam $^\circ\text{C}$) dari santri yang melakukan pemeriksaan berkala: $36{,}2; 36{,}4; 36{,}5; 36{,}5; 36{,}6; 36{,}8; 37{,}0$. Tentukan jangkauan dan simpangan baku suhu tubuh santri!
10. Catatan perolehan infak sukarela dari $10$ rombongan majelis taklim pondok adalah (dalam ribuan rupiah): $40, 45, 50, 50, 55, 60, 65, 70, 75, 90$. Tentukan simpangan kuartil ($Q_d$) dana infak tersebut!
11. Toko Kitab Pesantren mencatat jumlah penjualan kitab nahwu jurumiyah per hari selama $8$ hari berturut-turut: $14, 16, 18, 18, 20, 22, 24, 28\text{ eksemplar}$. Hitung varians dan simpangan baku penjualan kitab!
12. Data jarak tempuh jalan kaki santri (dalam ratusan meter) saat rihlah tadabur alam tercatat: $15, 18, 20, 22, 25, 26, 30$. Tentukan simpangan rata-rata jarak tempuh santri!
13. Ujian hafalan matan jazariyah diikuti oleh $40$ santri tahfiz dengan hasil sebagai berikut:

| Nilai Ujian | Frekuensi |
| :---: | :---: |
| $51 - 60$ | $4$ |
| $61 - 70$ | $10$ |
| $71 - 80$ | $16$ |
| $81 - 90$ | $7$ |
| $91 - 100$ | $3$ |

Hitung nilai rata-rata dan simpangan baku nilai ujian matan jazariyah santri!
14. Unit kebun buah tin pesantren mencatat berat buah tin yang dipanen per pohon (dalam gram) pada $7$ pohon percontohan: $320, 340, 350, 350, 360, 380, 410\text{ gram}$. Tentukan jangkauan, hamparan, dan simpangan rata-ratanya!
15. Panitia penerimaan santri baru mencatat nilai tes potensi akademik dari $50$ pendaftar:

| Nilai TPA | Frekuensi |
| :---: | :---: |
| $60 - 64$ | $5$ |
| $65 - 69$ | $12$ |
| $70 - 74$ | $18$ |
| $75 - 79$ | $10$ |
| $80 - 84$ | $5$ |

Tentukan simpangan rata-rata dan simpangan baku nilai tes pendaftar santri baru!
16. Waktu yang dihabiskan santri untuk mengulang hafalan (*muraja'ah*) mandiri di masjid (dalam menit per hari) dari $5$ santri teladan adalah: $90, 100, 110, 120, 130\text{ menit}$. Tentukan varians dan simpangan bakunya!
17. Hasil panen madu murni dari stup lebah pesantren selama $6$ bulan tercatat: $12, 14, 15, 16, 18, 21\text{ liter}$. Tentukan simpangan baku hasil panen madu!
18. Data lama santri mukim di pondok pesantren (dalam tahun) dari $8$ orang asatidz muda adalah: $4, 5, 6, 6, 7, 8, 9, 11\text{ tahun}$. Tentukan simpangan rata-rata lama mengabdi asatidz tersebut!
19. Dua kelas tahfiz putri memiliki nilai rata-rata tajwid yang sama yaitu $85$. Kelas Khadijah memiliki simpangan baku $S = 2{,}4$, sedangkan Kelas Aisyah memiliki simpangan baku $S = 5{,}8$. Analisislah kelas manakah yang memerlukan perhatian lebih dari guru tahfiz dan jelaskan alasannya berdasarkan konsep penyebaran data!
20. Santri bagian multimedia pesantren mengukur kecepatan internet asrama (dalam Mbps) pada $6$ titik pemancar ruang belajar: $18, 20, 22, 24, 26, 34\text{ Mbps}$. Hitunglah jangkauan, varians, dan simpangan baku kecepatan akses internet tersebut!

---

### 8. Pekerjaan Rumah (PR Pondok / Mandiri)

**Petunjuk Pengerjaan:**
- Kerjakan di buku catatan tugas matematika secara mandiri, runtut, dan rapi.
- Tuliskan apa yang diketahui, rumus ukuran penyebaran yang digunakan, serta langkah penyelesaian baris demi baris.

1. Tentukan nilai Jangkauan ($R$), Jangkauan Antarkuartil ($H$), Simpangan Kuartil ($Q_d$), Simpangan Rata-rata ($SR$), Ragam ($S^2$), dan Simpangan Baku ($S$) dari data nilai ujian fiqih santri berikut:



6, \ 7, \ 8, \ 8, \ 9, \ 10, \ 12, \ 12


2. Diberikan tabel distribusi frekuensi nilai ujian tajwid santri:

| Nilai | Frekuensi |
| :---: | :---: |
| $61 - 65$ | $3$ |
| $66 - 70$ | $5$ |
| $71 - 75$ | $8$ |
| $76 - 80$ | $4$ |

Lengkapilah tabel penolong dan hitunglah nilai Simpangan Rata-rata ($SR$), Ragam ($S^2$), dan Simpangan Baku ($S$)!
3. **Soal Kontekstual Aktivitas Pondok Pesantren:**  
   Pengurus asrama santri membandingkan kedisiplinan waktu tidur malam santri di dua lorong kamar (Lorong Al-Quds dan Lorong Al-Andalus) selama $7$ hari pengamatan.
   - Lorong Al-Quds memiliki rata-rata waktu tidur pukul $22.00$ dengan simpangan baku $S = 8\text{ menit}$.
   - Lorong Al-Andalus memiliki rata-rata waktu tidur pukul $22.00$ dengan simpangan baku $S = 35\text{ menit}$.  
   - Lorong manakah yang memiliki kedisiplinan waktu tidur lebih konsisten?  
   - Jelaskan makna perbedaan simpangan baku tersebut terhadap ketertiban suasana malam di asrama santri!
4. **Pertanyaan Pemahaman Konsep:**  
   *Jelaskan dengan kata-katamu sendiri: Mengapa nilai rata-rata (mean) saja tidak cukup untuk menggambarkan kualitas suatu kelompok data? Mengapa kita perlu menghitung simpangan baku (standar deviasi)? Berikan satu contoh analogi konkret dalam kehidupan sehari-hari santri!*

---

### 9. Ringkasan Materi

- **Ukuran Penyebaran Data**: Mengukur sejauh mana data menyebar dari nilai rata-rata pusatnya. Ukuran penyebaran mencakup Jangkauan ($R = X_{\max} - X_{\min}$), Jangkauan Antarkuartil ($H = Q_3 - Q_1$), Simpangan Kuartil ($Q_d = \frac{1}{2}H$), Simpangan Rata-rata ($SR$), Ragam ($S^2$), dan Simpangan Baku ($S$).
- **Simpangan Baku ($S$) & Ragam ($S^2$)**: Merupakan tolok ukur utama variabilitas data. Untuk data tunggal dirumuskan $S^2 = \frac{\sum (x_i - \bar{x})^2}{n}$ dan untuk data kelompok $S^2 = \frac{\sum f_i(x_i - \bar{x})^2}{\sum f_i}$, di mana $S = \sqrt{S^2}$.
- **Tingkat Homogenitas Data**: Nilai simpangan baku yang semakin kecil menandakan bahwa data semakin seragam, konsisten, dan homogen (berkumpul rapat di sekitar mean). Sebaliknya, nilai simpangan baku yang besar menandakan data heterogen dan timpang.
- **Efek Transformasi Linier Data ($y = ax + b$)**: Operasi pergeseran/penjumlahan ($b$) sama sekali **tidak mengubah** ukuran penyebaran data. Seluruh ukuran penyebaran ($R, H, Q_d, SR, S$) hanya terpengaruh oleh faktor pengali $\lvert a \rvert$ ($S_y = \lvert a \rvert S_x$), dan varians terpengaruh oleh kuadrat pengali ($S_y^2 = a^2 S_x^2$).
