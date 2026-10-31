# Repositori Modul Pembelajaran Mandiri Matematika
### Jenjang SMP/MTs & SMA/MA (Jurusan IPA & Pesantren)

Repositori ini berisi kumpulan modul bahan ajar mandiri siswa untuk mata pelajaran **Matematika SMP/MTs (Kelas 7, 8, 9)** dan **Matematika SMA/MA (Kelas 10, 11, 12 Jurusan IPA)** dengan adaptasi kurikulum pesantren. Seluruh materi dirancang terstruktur, bertahap (*scaffolded*), menggunakan formula KaTeX LaTeX presisi, serta mengintegrasikan hikmah keteraturan ciptaan Allah SWT dan studi kasus kontekstual kehidupan pondok pesantren.

---

## 🎯 Visi & Karakteristik Utama

1. **Murni Bahan Ajar Mandiri Siswa (*Student-Facing*)**
   - Disusun dengan gaya bahasa komunikatif, dialogis, dan mudah dipahami siswa saat belajar mandiri tanpa pendampingan langsung.
   - Bebas dari rubrik penilaian pengajar, kunci jawaban tersembunyi, maupun lembar instruktur.

2. **Standar Struktur 9 Bagian Modul**
   Setiap modul pertemuan wajib mengikuti format baku 9 bagian:
   1. **Pengertian & Konsep Dasar**: Definisi intuitif, motivasi belajar, dan hikmah/filosofi sunnatullah.
   2. **Bentuk Umum & Rumus Baku**: Notasi matematis formal dan definisi simbol.
   3. **Sifat-Sifat, Karakteristik, & Aturan Khusus**: Syarat keberlakuan rumus, tabel komparasi, dan batasan operasi.
   4. **Contoh Soal & Pembahasan Terperinci**: Scaffolding bertingkat (Diketahui $\to$ Ditanyakan $\to$ Langkah Penyelesaian $\to$ Kesimpulan $\checkmark$).
   5. **Penerapan Kontekstual**: Studi kasus aktivitas santri dan kehidupan nyata di pondok pesantren.
   6. **Pola Kunci & Cara Cepat Mengingat**: Jembatan keledai visual (*mnemonic*), alur kerja, dan catatan waspada kesalahan umum (*common pitfalls*).
   7. **Latihan Soal Mandiri**: Kumpulan soal terpartisi per topik fokus (masing-masing tepat 20 butir soal bernomor urut rapi 1–20 dengan petunjuk umum).
   8. **Pekerjaan Rumah (PR Mandiri / Pondok)**: Tugas penguatan konsep dan aplikasi kontekstual santri.
   9. **Ringkasan Materi**: 3–4 poin esensial ringkas sebagai intisari materi pertemuan.

3. **Standar KaTeX LaTeX Universal**
   - Notasi sebaris (*inline*) menggunakan tanda dolar tunggal (`$x$`).
   - Notasi blok (*display*) menggunakan blok ganda pada baris tersendiri yang diletakkan rata kiri (*column 0*) dengan baris kosong sebelum dan sesudahnya untuk menjamin render sempurna di seluruh Markdown engine (VS Code, GitHub, Obsidian, Typora).
   - Penggunaan `\lvert ... \rvert` untuk nilai mutlak/determinan pada tabel Markdown guna mencegah kerusakan parsing kolom.

4. **Konteks Santri & Bebas Transaksi Non-Syariah (*Strict Constraint*)**
   - Seluruh studi kasus dan soal cerita mengangkat tema positif lingkungan pesantren: hafalan Al-Qur'an (*tasmi'* & *muraja'ah*), kajian kitab kuning (*muthala'ah*), infak sukarela majelis, manajemen logistik dapur santri, jadwal piket/ibadah, pos kesehatan pesantren (poskestren), dan unit usaha mandiri pesantren (seperti toko kitab atau kebun asrama).
   - **Prinsip Muamalah Bersih**: Seluruh muatan transaksi dan soal cerita wajib berlandaskan prinsip syariah murni dan dilarang memuat istilah perbankan atau pembiayaan konvensional non-syariah.

---

## 📁 Struktur Direktori Repositori

```text
math/
├── .plan/                                              # Dokumen perancangan pra-eksekusi (Two-Phase Protocol)
│   ├── 2026-10-31-materi-kelas-11-pertemuan-7.md
│   └── 2026-10-31-materi-kelas-12-pertemuan-8.md
├── kelas-7/                                            # Modul Matematika SMP Kelas 7
│   └── pertemuan-01-bilangan-bulat.md
├── kelas-8/                                            # Modul Matematika SMP Kelas 8
├── kelas-9/                                            # Modul Matematika SMP Kelas 9
├── kelas-10/                                           # Modul Matematika SMA Kelas 10 (IPA & Pesantren)
├── kelas-11/                                           # Modul Matematika SMA Kelas 11 (IPA & Pesantren)
│   └── pertemuan-07-determinan-dan-invers-matriks.md
├── kelas-12/                                           # Modul Matematika SMA Kelas 12 (IPA & Pesantren)
│   └── pertemuan-08-ukuran-penyebaran-data.md
└── README.md                                           # Dokumentasi utama repositori
```

---

## 📚 Cakupan Silabus Lengkap (72 Pertemuan per Jenjang)

### A. Matematika SMP / MTs (72 Pertemuan)

| Jenjang | Semester | Pertemuan Efektif | Pokok Bahasan Utama |
| :--- | :--- | :---: | :--- |
| **Kelas 7** | Ganjil | 12 Pertemuan | Bilangan Bulat, Operasi Pecahan, Aljabar Dasar, Himpunan, PLSV & PtLSV |
| | Genap | 12 Pertemuan | Perbandingan & Skala, Aritmetika Syariah, Sudut & Garis, Segiempat & Segitiga, Penyajian Data |
| **Kelas 8** | Ganjil | 12 Pertemuan | Pola Bilangan & Barisan, Koordinat Kartesius, Relasi & Fungsi, Persamaan Garis Lurus, SPLDV |
| | Genap | 12 Pertemuan | Teorema Pythagoras & Tripel, Lingkaran (Sudut, Busur, Juring), Bangun Ruang Sisi Datar (BRSD) |
| **Kelas 9** | Ganjil | 12 Pertemuan | Bilangan Berpangkat & Bentuk Akar, Persamaan Kuadrat, Fungsi Kuadrat & Aplikasi Parabola |
| | Genap | 12 Pertemuan | Transformasi Geometri, Kesebangunan & Kekongruenan, Bangun Ruang Sisi Lengkung (BRSL) |

---

### B. Matematika SMA / MA - Jurusan IPA & Pesantren (72 Pertemuan)

| Jenjang | Semester | Pertemuan Efektif | Pokok Bahasan Utama |
| :--- | :--- | :---: | :--- |
| **Kelas 10** | Ganjil | 12 Pertemuan | Eksponen & Bentuk Akar, Fungsi & Persamaan Logaritma, Persamaan/Pertidaksamaan Nilai Mutlak, SPLTV |
| | Genap | 12 Pertemuan | Fungsi Kuadrat, Komposisi & Invers Fungsi, Trigonometri Dasar (Perbandingan & Sudut Istimewa), Aturan Sinus & Cosinus, Vektor Ruang |
| **Kelas 11** | Ganjil | 12 Pertemuan | Induksi Matematika, Program Linear & Uji Titik Pojok, Aljabar Matriks, Determinan & Invers, Aturan Cramer, Transformasi Geometri Matriks |
| | Genap | 12 Pertemuan | Barisan & Deret (Aritmetika, Geometri, Tak Hingga), Limit Fungsi Aljabar & Trigonometri, Turunan Fungsi Aljabar, Aplikasi Turunan |
| **Kelas 12** | Ganjil | 12 Pertemuan | Geometri Ruang / Dimensi Tiga (Jarak & Sudut), Statistika Deskriptif (Distribusi Frekuensi, Ukuran Pemusatan, Ukuran Letak, Ukuran Penyebaran Data) |
| | Genap | 12 Pertemuan | Kaidah Pencacahan (Faktorial, Permutasi, Kombinasi), Teori Peluang Kejadian Majemuk, Kalkulus Integral (Tak Tentu, Tentu, Luas Daerah, Volume Benda Putar) |

---

## 🛠️ Pedoman Penyusunan & Kontribusi Modul Baru

Setiap modul baru yang ditambahkan ke repositori ini wajib mematuhi standar operasional berikut:

1. **Protokol Perencanaan Dua Fase (*Two-Phase Protocol*)**
   - Sebelum berkas modul dibuat, susun berkas rencana pada direktori `.plan/YYYY-MM-DD-<topik>.md`.
   - Lakukan tinjauan ruang lingkup materi, notasi, dan partisi latihan soal sebelum materi ajar final digenerasikan.

2. **Standardisasi Latihan Soal**
   - Latihan soal dipecah menjadi set terpisah yang fokus (misalnya: *Set 1: Konsep & Perhitungan Dasar*, *Set 2: Perhitungan Lanjutan/Kelompok*, *Set 3: Penerapan Kontekstual Santri*).
   - Setiap set memuat tepat **20 soal** bernomor urut 1–20.
   - Menggunakan instruksi umum di bagian atas set (tanpa petunjuk repetitif pada setiap nomor soal).

3. **Verifikasi Kepatuhan Syariah & Validitas KaTeX**
   - Pastikan seluruh studi kasus selaras dengan adab dan nuansa islami pesantren.
   - Pastikan seluruh blok persamaan tidak terindentasi spasi dan baris formula valid tanpa eror KaTeX.

---

## 📖 Berkas Modul yang Telah Tersedia

- Kelas 7 Pertemuan 1: [Operasi Hitung Bilangan Bulat](file:///d:/Project/exercise/math/kelas-7/pertemuan-01-bilangan-bulat.md)
- Kelas 11 Pertemuan 7: [Determinan dan Invers Matriks](file:///d:/Project/exercise/math/kelas-11/pertemuan-07-determinan-dan-invers-matriks.md)
- Kelas 12 Pertemuan 8: [Ukuran Penyebaran Data](file:///d:/Project/exercise/math/kelas-12/pertemuan-08-ukuran-penyebaran-data.md)
