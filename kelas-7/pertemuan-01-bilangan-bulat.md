# BILANGAN BULAT
## Pertemuan 1: Konsep Bilangan Bulat dan Sifat Operasi Hitung

---

### 1. Pengertian & Konsep Dasar

Bilangan bulat adalah himpunan bilangan yang terdiri atas bilangan bulat positif (bilangan asli), bilangan nol ($0$), dan bilangan bulat negatif. Himpunan bilangan bulat dilambangkan secara matematis dengan huruf $\mathbb{Z}$ (dari bahasa Jerman *Zahlen*):

$$
\mathbb{Z} = \{\dots, -3, -2, -1, 0, 1, 2, 3, \dots}
$$

Pada garis bilangan horizontal:
- Bilangan di sebelah kanan nol bernilai **positif** ($\mathbb{Z}^+ = \{1, 2, 3, \dots\}$).
- Bilangan di sebelah kiri nol bernilai **negatif** ($\mathbb{Z}^- = \{\dots, -3, -2, -1\}$).
- Bilangan $0$ merupakan bilangan netral (bukan positif dan bukan negatif).
- Semakin ke kanan letak suatu bilangan pada garis bilangan, nilainya semakin **besar**. Sebaliknya, semakin ke kiri, nilainya semakin **kecil**.

```
<---|-------|-------|-------|-------|-------|-------|--->
   -3      -2      -1       0       1       2       3
<--- Nilai Semakin Kecil          Nilai Semakin Besar --->
```

**Contoh / Analogi Sederhana:**
- **Suhu Udara:** Suhu di daerah pegunungan sekitar pondok saat fajar mencapai $3^\circ\text{C}$ di bawah nol, ditulis $-3^\circ\text{C}$. Suhu di dalam ruang kelas asrama adalah $24^\circ\text{C}$ di atas nol, ditulis $+24^\circ\text{C}$ atau cukup $24^\circ\text{C}$.
- **Permukaan Air Laut:** Penyelam berada pada kedalaman $15\text{ m}$ di bawah permukaan air laut (dinyatakan $-15\text{ m}$), sedangkan burung camar terbang pada ketinggian $10\text{ m}$ di atas permukaan laut (dinyatakan $+10\text{ m}$).
- **Keuangan Kas Asrama:** Penerimaan dana infak santri sebesar $\text{Rp}50.000$ dinyatakan $+50.000$, sedangkan pengeluaran kas untuk pembelian perlengkapan kebersihan kamar sebesar $\text{Rp}15.000$ dinyatakan $-15.000$.

---

### 2. Bentuk Umum & Rumus Baku

Operasi hitung pada bilangan bulat mencakup penjumlahan, pengurangan, perkalian, dan pembagian untuk setiap bilangan bulat $a, b, c \in \mathbb{Z}$.

#### A. Sifat-Sifat Operasi Hitung

1. **Sifat Komutatif (Pertukaran):**
   - Penjumlahan: 

$$
a + b = b + a
$$

   - Perkalian: 

$$
a \times b = b \times a
$$

   *(Catatan: Pengurangan dan pembagian **tidak** bersifat komutatif: $a - b \neq b - a$ dan $a \div b \neq b \div a$)*

2. **Sifat Asosiatif (Pengelompokan):**
   - Penjumlahan: 

$$
(a + b) + c = a + (b + c)
$$

   - Perkalian: 

$$
(a \times b) \times c = a \times (b \times c)
$$

3. **Sifat Distributif (Penyebaran Perkalian):**
   - Terhadap Penjumlahan: 

$$
a \times (b + c) = (a \times b) + (a \times c)
$$

   - Terhadap Pengurangan: 

$$
a \times (b - c) = (a \times b) - (a \times c)
$$

4. **Unsur Identitas & Invers:**
   - Unsur identitas penjumlahan adalah $0$: 

$$
a + 0 = 0 + a = a
$$

   - Invers penjumlahan (lawan bilangan): 

$$
a + (-a) = 0
$$

   - Unsur identitas perkalian adalah $1$: 

$$
a \times 1 = 1 \times a = a
$$

#### B. Urutan Kekuatan Operasi Hitung (Hierarki Kabataku)

Jika dalam satu soal terdapat beberapa operasi hitung sekaligus, urutan pengerjaannya wajib mematuhi aturan berikut:
1. Operasi di dalam tanda kurung $(...)$ atau tanda kurung siku $[...]$ diselesaikan paling awal.
2. Perkalian $(\times)$ dan Pembagian $(\div)$ setara tingkatannya, dikerjakan berurutan dari sebelah kiri ke kanan.
3. Penjumlahan $(+)$ dan Pengurangan $(-)$ setara tingkatannya, dikerjakan berurutan dari sebelah kiri ke kanan.

**Keterangan Simbol:**
- $a, b, c$ = sembarang bilangan bulat ($a, b, c \in \mathbb{Z}$)
- $-a$ = lawan (invers aditif) dari bilangan $a$
- $|a|$ = nilai mutlak dari $a$ (jarak bilangan $a$ dari titik $0$ pada garis bilangan)

---

### 3. Sifat-Sifat, Karakteristik, & Aturan Khusus

Beberapa aturan mutlak operasi tanda pada bilangan bulat:

1. **Aturan Pengurangan Bilangan Bulat:**
   Mengurangkan suatu bilangan sama artinya dengan menjumlahkan bilangan tersebut dengan lawannya:

$$
a - b = a + (-b)
$$

$$
a - (-b) = a + b
$$

2. **Aturan Tanda pada Perkalian dan Pembagian:**
   - Perkalian/pembagian dua bilangan bertanda sama menghasilkan bilangan **positif**.
   - Perkalian/pembagian dua bilangan bertanda beda menghasilkan bilangan **negatif**.

| Operasi | Tanda Bilangan 1 | Tanda Bilangan 2 | Tanda Hasil Akhir | Contoh Perhitungan |
| :--- | :---: | :---: | :---: | :--- |
| **Perkalian** | Positif $(+)$ | Positif $(+)$ | Positif $(+)$ | $6 \times 7 = 42$ |
| **Perkalian** | Positif $(+)$ | Negatif $(-)$ | Negatif $(-)$ | $6 \times (-7) = -42$ |
| **Perkalian** | Negatif $(-)$ | Positif $(+)$ | Negatif $(-)$ | $(-6) \times 7 = -42$ |
| **Perkalian** | Negatif $(-)$ | Negatif $(-)$ | Positif $(+)$ | $(-6) \times (-7) = 42$ |
| **Pembagian** | Positif $(+)$ | Positif $(+)$ | Positif $(+)$ | $36 \div 4 = 9$ |
| **Pembagian** | Positif $(+)$ | Negatif $(-)$ | Negatif $(-)$ | $36 \div (-4) = -9$ |
| **Pembagian** | Negatif $(-)$ | Positif $(+)$ | Negatif $(-)$ | $(-36) \div 4 = -9$ |
| **Pembagian** | Negatif $(-)$ | Negatif $(-)$ | Positif $(+)$ | $(-36) \div (-4) = 9$ |

3. **Operasi yang Melibatkan Angka Nol:**
   - Perkalian dengan nol: $a \times 0 = 0 \times a = 0$.
   - Nol dibagi bilangan bukan nol: $\frac{0}{a} = 0$ (untuk $a \neq 0$).
   - Pembagian bilangan dengan nol: $\frac{a}{0}$ menghasilkan nilai **tidak terdefinisi** (*undefined*).

---

### 4. Contoh Soal & Pembahasan Terperinci

#### Contoh 1 (Tingkat Dasar)
**Soal:**
Tentukan hasil dari operasi hitung penjumlahan dan pengurangan bilangan bulat berikut:

$$
-18 + (-12) - (-25)
$$

**Penyelesaian:**
- **Diketahui:**
  - Bilangan yang dioperasikan: $-18$, $-12$, dan $-25$.
- **Ditanyakan:**
  - Hasil dari $-18 + (-12) - (-25)$
- **Langkah Penyelesaian:**
  1. Ubah operasi pengurangan dengan bilangan negatif menjadi penjumlahan dengan lawannya:

$$
-18 + (-12) - (-25) = -18 + (-12) + 25
$$

  2. Kerjakan penjumlahan berurutan dari kiri:

$$
-18 + (-12) = -(18 + 12) = -30
$$

  3. Lanjutkan penjumlahan dengan bilangan berikutnya:

$$
-30 + 25 = -(30 - 25) = -5
$$

- **Kesimpulan:** 
  Jadi, hasil akhir dari $-18 + (-12) - (-25)$ adalah $-5$ ($\checkmark\ \text{Benar}$)

---

#### Contoh 2 (Bentuk Variasi & Campuran Kabataku)
**Soal:**
Hitunglah nilai dari ekspresi operasi hitung campuran berikut:

$$
45 - (-24) \div (-6) + 7 \times (-4)
$$

**Penyelesaian:**
- **Diketahui:**
  - Operasi hitung memuat pengurangan, pembagian, penjumlahan, dan perkalian.
- **Ditanyakan:**
  - Hasil dari $45 - (-24) \div (-6) + 7 \times (-4)$
- **Langkah Penyelesaian:**
  1. Selesaikan operasi pembagian dan perkalian terlebih dahulu (aturan Kabataku):
     - Pembagian: 

$$
(-24) \div (-6) = +4
$$

     - Perkalian: 

$$
7 \times (-4) = -28
$$

  2. Masukkan hasil pembagian dan perkalian ke dalam urutan operasi:

$$
45 - 4 + (-28)
$$

  3. Selesaikan operasi pengurangan dan penjumlahan secara berurutan dari kiri ke kanan:
     - Pengurangan:

$$
45 - 4 = 41
$$

     - Penjumlahan dengan bilangan negatif:

$$
41 + (-28) = 41 - 28 = 13
$$

- **Kesimpulan:** 
  Jadi, hasil akhir dari $45 - (-24) \div (-6) + 7 \times (-4)$ adalah $13$ ($\checkmark\ \text{Benar}$)

---

### 5. Penerapan Kontekstual (Studi Kasus Nyata / Santri)

#### Contoh Kasus:
> Pada perlombaan Cerdas Cermat Cendekia Santri tingkat daerah, panitia menetapkan sistem penilaian dengan aturan berikut:
> - Jawaban benar diberi skor $+4$
> - Jawaban salah diberi skor $-2$
> - Soal yang tidak dijawab diberi skor $-1$
>
> Regu santri dari Pondok Pesantren Al-Hikmah mengikuti lomba tersebut yang terdiri atas total $30$ butir soal. Regu ini berhasil menjawab $22$ soal dengan benar dan $5$ soal salah, sedangkan sisanya tidak dijawab karena waktu habis. Berapakah total skor akhir yang diperoleh regu santri tersebut?

**Langkah Pemecahan:**

1. **Rincian Data Soal:**
   - Jumlah seluruh soal = $30$ butir soal
   - Soal dijawab benar = $22$ butir soal (setiap soal bernilai $+4$)
   - Soal dijawab salah = $5$ butir soal (setiap soal bernilai $-2$)
   - Soal tidak dijawab:

$$
30 - (22 + 5) = 30 - 27 = 3\text{ butir soal}\quad (\text{setiap soal bernilai } -1)
$$

2. **Perhitungan Total Skor:**

$$
\begin{aligned}
\text{Total Skor} &= (22 \times 4) + (5 \times (-2)) + (3 \times (-1)) \\
&= 88 + (-10) + (-3) \\
&= 88 - 10 - 3 \\
&= 78 - 3 \\
&= 75
\end{aligned}
$$

3. **Jawaban Kontekstual:**
   Jadi, total skor akhir yang diperoleh regu santri Pondok Pesantren Al-Hikmah adalah $75$ poin.

---

### 6. Pola Kunci & Cara Cepat Mengingat

- **Jembatan Keledai Hierarki Operasi: "Ka-Ba-Ta-Ku"**
  - **Tanda Kurung** diselesaikan terlebih dahulu sebelum operasi lainnya.
  - **Ka**li dan **Ba**gi dikerjakan setara berurutan dari kiri ke kanan.
  - **Ta**mbah dan **Ku**rang dikerjakan setara berurutan dari kiri ke kanan.

- **Pola Tanda Minus Bertemu Minus:**
  *Dua tanda minus yang berurutan langsung berubah menjadi tanda positif (tambah):*

$$
-(-x) \longrightarrow +x
$$

- **Pola Perkalian/Pembagian Dua Tanda:**
  - Tanda **sama** $\longrightarrow$ hasil **positif** ($+ \times + = +$ dan $- \times - = +$)
  - Tanda **beda** $\longrightarrow$ hasil **negatif** ($+ \times - = -$ dan $- \times + = -$)

- **Catatan Waspada (Jangan Sampai Keliru):**
  - ⚠️ *Jangan menjumlahkan sebelum mengalikan!* Pada bentuk $10 + 2 \times 5$, jangan hitung $(10+2) \times 5 = 60$, melainkan $10 + (2 \times 5) = 10 + 10 = 20$.
  - ⚠️ *Urutan pengerjaan perkalian dan pembagian setara:* Kerjakan runtut dari kiri ke kanan. Misalnya pada $36 \div 6 \times 2$, selesaikan pembagian terlebih dahulu: $(36 \div 6) \times 2 = 6 \times 2 = 12$, bukan $36 \div (6 \times 2) = 36 \div 12 = 3$.
  - ⚠️ *Pengurangan berurutan harus diselesaikan dari kiri ke kanan:*

$$
20 - 8 - 3 = (20 - 8) - 3 = 12 - 3 = 9
$$

    *(Bukan $20 - (8 - 3) = 20 - 5 = 15$, ini kesalahan fatal).*

---

### 7. Latihan Soal

---

#### Latihan Soal 1 (20 Soal)

**A. Pemahaman Konsep & Garis Bilangan**
1. Sebuah kapal selam beroperasi pada kedalaman $120\text{ m}$ di bawah permukaan air laut. Tuliskan lambang bilangan bulat yang sesuai untuk posisi kapal selam tersebut!
2. Sisipkan tanda perbandingan yang tepat ($<$, $>$, atau $=$) pada pernyataan berikut:  

$$
-18 \ \dots \ -11
$$

3. Urutkan himpunan bilangan bulat berikut dari nilai yang terkecil hingga terbesar:  

$$
-15,\ 9,\ -30,\ 0,\ 17,\ -4,\ -21
$$

4. Tentukan lawan bilangan (invers aditif) dan nilai mutlak dari bilangan $-58$!

**B. Operasi Hitung Bilangan Bulat**  
*(Petunjuk: Hitunglah hasil akhir dari setiap operasi hitung berikut)*
5. $47 + (-68)$
6. $(-35) - (-49)$
7. $(-45) + 82 - 37 - (-24)$
8. $15 \times (-8)$
9. $196 \div (-14)$
10. $(-4) \times (-5) \times (-6)$
11. $(-18) \times (-15) \div (-10)$
12. $42 + (-54) \div 6 - 7 \times (-5)$
13. $(36 - 60) \div (-8) + 6 \times (-4)$
14. $90 - [48 + (-16) \times 4] \div (-8)$

**C. Sifat Hitung & Penerapan Kontekstual**
15. Hitunglah secara cepat dengan menggunakan sifat komutatif dan asosiatif:  

$$
(-25) \times 49 \times 4
$$

16. Hitunglah secara efisien dengan menggunakan sifat distributif:  

$$
34 \times 28 + 34 \times 72
$$

17. Suhu mula-mula di sebuah kota pegunungan pada pagi hari adalah $-6^\circ\text{C}$. Menjelang siang, suhu naik sebesar $14^\circ\text{C}$. Pada malam hari, suhu turun kembali sebesar $9^\circ\text{C}$. Berapakah suhu udara kota tersebut pada malam hari?
18. Seekor burung terbang pada ketinggian $25\text{ m}$ di atas permukaan laut, sedangkan seekor ikan berenang tepat di bawahnya pada kedalaman $18\text{ m}$ di bawah permukaan laut. Berapakah jarak vertikal antara burung dan ikan tersebut?
19. Pada babak penyisihan lomba cerdas cermat santri dengan $30$ butir soal, setiap jawaban benar diberi nilai $+4$, jawaban salah diberi nilai $-2$, dan tidak dijawab diberi nilai $-1$. Regu santri menjawab $21$ soal benar, $6$ soal salah, dan sisanya tidak dijawab. Hitunglah total nilai yang diperoleh regu tersebut!
20. Bendahara kamar santri mencatat kas awal sebesar $\text{Rp}250.000$. Selama dua pekan terdapat pengeluaran untuk membeli galon air minum sebesar $\text{Rp}65.000$ dan alat kebersihan sebesar $\text{Rp}45.000$, kemudian menerima infak iuran kebersihan dari anggota kamar sebesar $\text{Rp}120.000$. Tuliskan bentuk operasi bilangannya dan tentukan saldo akhir kas kamar santri tersebut!

---

#### Latihan Soal 2 (20 Soal)

**A. Pemahaman Konsep & Garis Bilangan**
1. Seorang penyelam mutiara berada pada kedalaman $45\text{ m}$ di bawah permukaan air laut. Tuliskan lambang bilangan bulat yang sesuai untuk posisi penyelam tersebut!
2. Sisipkan tanda perbandingan yang tepat ($<$, $>$, atau $=$) pada pernyataan berikut:  

$$
-29 \ \dots \ -35
$$

3. Urutkan himpunan bilangan bulat berikut dari nilai yang terbesar hingga terkecil:  

$$
42,\ -50,\ -18,\ 65,\ -7,\ 24,\ -1
$$

4. Tentukan lawan bilangan (invers aditif) dan nilai mutlak dari bilangan $-49$!

**B. Operasi Hitung Bilangan Bulat**  
*(Petunjuk: Hitunglah hasil akhir dari setiap operasi hitung berikut)*
5. $(-56) + 73$
6. $(-37) - (-75)$
7. $68 - 95 + (-42) - (-39)$
8. $18 \times (-7)$
9. $228 \div (-12)$
10. $(-3) \times (-7) \times (-4)$
11. $(-24) \times (-14) \div (-8)$
12. $55 - (-48) \div 8 + 6 \times (-6)$
13. $(52 - 80) \div (-7) + 5 \times (-8)$
14. $100 - [65 + (-18) \times 3] \div (-11)$

**C. Sifat Hitung & Penerapan Kontekstual**
15. Hitunglah secara cepat dengan menggunakan sifat komutatif dan asosiatif:  

$$
(-125) \times (-38) \times (-8)
$$

16. Hitunglah secara efisien dengan menggunakan sifat distributif:  

$$
46 \times 87 - 46 \times 37
$$

17. Sebongkah daging beku bersuhu $-15^\circ\text{C}$ dikeluarkan dari ruang pendingin dapur santri. Saat dimasak di atas wajan, suhunya naik rata-rata $4^\circ\text{C}$ setiap $3\text{ menit}$. Berapakah suhu daging tersebut setelah dimasak selama $18\text{ menit}$?
18. Sebuah lift di gedung asrama santri mula-mula berada di lantai $9$. Lift tersebut bergerak turun sejauh $12$ lantai ke lantai bawah tanah (*basement*), kemudian bergerak naik lagi sejauh $5$ lantai. Pada lantai berapakah lift tersebut berhenti sekarang?
19. Dalam tes seleksi olimpiade sains santri yang terdiri atas $40$ butir soal, aturan penilaian yang berlaku: jawaban benar diberi nilai $+4$, jawaban salah diberi nilai $-2$, dan soal kosong diberi nilai $-1$. Ahmad berhasil menjawab benar $32$ soal, salah $5$ soal, dan sisanya tidak dijawab. Berapakah total nilai akhir yang diraih Ahmad?
20. Santri pengurus dapur umum pondok menyiapkan anggaran sebesar $\text{Rp}480.000$ untuk membeli buah hidangan buka puasa sunnah santri. Pengurus membeli $30\text{ butir}$ melon dengan harga $\text{Rp}12.000$ per butir, dan $10\text{ butir}$ semangka dengan harga $\text{Rp}9.000$ per butir. Tentukan sisa atau kekurangan dana pengurus dapur dalam notasi bilangan bulat bertanda!

---

### 8. Pekerjaan Rumah (PR Pondok / Mandiri)

**Petunjuk:**
- Kerjakan di buku tugas masing-masing secara mandiri dan rapi.
- Tuliskan apa yang diketahui, aturan/sifat hitung yang digunakan, dan langkah perhitungannya baris demi baris.

1. Tentukan hasil perhitungan dari operasi campuran berikut:

$$
[(-36) + 12] \div (-8) - (-5) \times 7
$$

2. Hitunglah hasil dari operasi hitung campuran berikut:

$$
(-14) \times 5 - (-64) \div 8 + (-27)
$$

3. **Soal Kontekstual Aktivitas Pondok:**  
   Toko Kitab Pesantren mendatangkan $12$ kardus kitab nahwu dengan biaya pengadaan $\text{Rp}150.000$ per kardus. Pada pekan pertama, tersalurkan kepada para santri sebanyak $8$ kardus dengan infak pengganti $\text{Rp}180.000$ per kardus. Pada pekan kedua, sisa $4$ kardus disalurkan dengan infak subsidi $\text{Rp}135.000$ per kardus karena sebagian sampul kardus basah terkena tempias air hujan.  
   - Hitung total biaya pengadaan kitab yang dikeluarkan Toko Kitab Pesantren!  
   - Hitung total dana penerimaan dari penyaluran seluruh kitab!  
   - Tentukan selisih dana akhir toko kitab dan nyatakan dalam bentuk bilangan bulat bertanda positif (jika surplus dana) atau negatif (jika defisit dana)!
4. **Pertanyaan Pemahaman Konsep:**  
   *Jelaskan dengan kata-katamu sendiri: mengapa hasil perkalian dua bilangan negatif (misalnya $(-3) \times (-4)$) selalu menghasilkan bilangan positif ($+12$)? Buatlah satu contoh ilustrasi logis (misalnya menggunakan pola deret perkalian berurutan).*

---

### 9. Ringkasan Materi

- **Himpunan Bilangan Bulat**: $\mathbb{Z} = \{\dots, -2, -1, 0, 1, 2, \dots\}$. Bilangan bulat mencakup bilangan bulat negatif, bilangan nol, dan bilangan bulat positif.
- **Sifat Operasi Hitung**: Penjumlahan dan perkalian memenuhi sifat komutatif ($a+b = b+a$; $a \times b = b \times a$) dan asosiatif ($(a+b)+c = a+(b+c)$), serta perkalian memenuhi sifat distributif ($a \times (b \pm c) = a \times b \pm a \times c$).
- **Aturan Tanda Perkalian & Pembagian**: Dua bilangan bertanda sama menghasilkan bilangan positif, sedangkan dua bilangan bertanda beda menghasilkan bilangan negatif.
- **Hierarki Kabataku**: Urutan pengerjaan operasi hitung wajib mendahulukan tanda kurung, kemudian perkalian dan pembagian (setara dari kiri ke kanan), lalu diakhiri dengan penjumlahan dan pengurangan (setara dari kiri ke kanan).
