# IMPLEMENTATION PLAN: MATERI AJAR KELAS 12 PERTEMUAN 8 (MATEMATIKA SMA/MA)

- **Tanggal Pembuatan**: 2026-10-31
- **Kategori**: materi-tutor
- **Lokasi Berkas**: `.plan/2026-10-31-materi-kelas-12-pertemuan-8.md`
- **Status**: Selesai Diimplementasikan
- **Estimasi Kompleksitas**: Sedang

---

## 1. TUJUAN & RUANG LINGKUP

- **Problem Statement**: 
  Penyusunan modul materi ajar mandiri siswa untuk Kelas 12 Pertemuan 8 mata pelajaran Matematika SMA/MA (Jurusan IPA & Pesantren). Berdasarkan silabus resmi 72 pertemuan, Pertemuan 8 Semester Ganjil membahas **Statistika Deskriptif: Ukuran Penyebaran Data (Dispersion Measures)** mencakup Jangkauan ($R$), Jangkauan Antarkuartil ($H$), Simpangan Kuartil ($Q_d$), Simpangan Rata-rata ($SR$), Ragam/Varians ($S^2$), dan Simpangan Baku/Standar Deviasi ($S$) untuk data tunggal maupun data berkelompok, serta interpretasi homogenitas data.
  *(Catatan silabus alternatif: jika yang dimaksud Semester Genap Pertemuan 8, agendanya adalah Evaluasi 2 Integral. Rencana default ini mengacu pada materi ajar Semester Ganjil).*
- **Goals**: 
  1. Menghasilkan modul belajar mandiri siswa berbasis format 9 bagian baku sesuai `template-materi-ajar.md`.
  2. Menerapkan notasi KaTeX LaTeX murni untuk rumus statistik data tunggal dan berkelompok tanpa teks datar ambigu.
  3. Menyajikan contoh soal bertingkat (scaffolding terperinci: Diketahui, Ditanyakan, Langkah Runtut, Kesimpulan $\checkmark$).
  4. Menyajikan studi kasus kontekstual pesantren (analisis konsistensi dan homogenitas nilai hafalan Al-Qur'an atau ketepatan waktu ibadah santri) bebas dari istilah riba/bunga/koperasi.
  5. Menyusun paket latihan soal terpisah:
     - Latihan Soal 1 (20 soal): Data Tunggal & Konsep Penyebaran.
     - Latihan Soal 2 (20 soal): Data Berkelompok (Tabel Distribusi Frekuensi).
     - Latihan Soal 3 (20 soal): Penerapan Kontekstual Santri & Pemecahan Masalah Nyata Pesantren.
- **Out of Scope**: 
  - Rubrik penskoran instruktur/guru.
  - Statistika inferensial (uji hipotesis, regresi/korelasi) yang berada di luar materi SMA/MA kelas 12 semester ganjil.

---

## 2. KEBUTUHAN SISTEM & DEPENDENSI

- **Format Dokumen**: Markdown (.md) dengan KaTeX math renderer (`$...$` untuk inline dan `$$...$$` untuk display blok).
- **Target Pembaca**: Siswa Kelas 12 SMA/MA IPA / Santri Tingkat Akhir Pondok Pesantren.
- **Batasan Kontekstual**: Nuansa islami pesantren, nilai ketelitian dan kejujuran data, bersih dari istilah riba (bebas bunga/kredit/pinjaman/koperasi).

---

## 3. RANCANGAN ARSITEKTUR & STRUKTUR BERKAS

### Struktur Berkas Terkait
```text
d:\Project\exercise\math\
├── .plan\
│   └── 2026-10-31-materi-kelas-12-pertemuan-8.md             # [Baru] Dokumen perencanaan implementasi
└── kelas-12\
    └── pertemuan-08-ukuran-penyebaran-data.md                # [Baru] Modul materi ajar mandiri siswa
```

### Rancangan Konten Modul 9 Bagian
1. **Pengertian & Konsep Dasar**:
   - Konsep ukuran penyebaran data: mengapa ukuran pemusatan (mean/median) tidak cukup untuk menggambarkan kualitas suatu populasi/sampel.
   - Analogi keadilan dan kesetaraan dalam sunnatullah: sebaran nilai hafalan santri yang homogen (merata) vs heterogen (timpang).
2. **Bentuk Umum & Rumus Baku**:
   - **Ukuran Penyebaran Sederhana**:
     - Jangkauan: $R = X_{\max} - X_{\min}$
     - Jangkauan Antarkuartil (Hamparan): $H = Q_3 - Q_1$
     - Simpangan Kuartil (Semi-Interkuartil): $Q_d = \frac{1}{2} H = \frac{1}{2}(Q_3 - Q_1)$
   - **Simpangan Rata-rata ($SR$)**:
     - Data Tunggal: $SR = \frac{\sum |x_i - \bar{x}|}{n}$
     - Data Berkelompok: $SR = \frac{\sum f_i |x_i - \bar{x}|}{\sum f_i}$
   - **Ragam / Varians ($S^2$) & Simpangan Baku ($S$)**:
     - Data Tunggal: $S^2 = \frac{\sum (x_i - \bar{x})^2}{n}$, $\quad S = \sqrt{S^2}$
     - Data Berkelompok: $S^2 = \frac{\sum f_i (x_i - \bar{x})^2}{\sum f_i}$, $\quad S = \sqrt{S^2}$
     - Metode Rata-rata Sementara (metode koding): $S^2 = p^2 \left[ \frac{\sum f_i u_i^2}{\sum f_i} - \left(\frac{\sum f_i u_i}{\sum f_i}\right)^2 \right]$
3. **Sifat-Sifat, Karakteristik, & Aturan Khusus**:
   - Makna nilai simpangan baku ($S$): makin kecil $S$, data semakin homogen dan mendekati rata-rata; makin besar $S$, data semakin bervariasi/heterogen.
   - Sifat transformasi linier data: Jika setiap data $x_i$ ditambah/dikurang $a$, ukuran penyebaran **tetap**. Jika setiap data dikali/dibagi $b$, ukuran penyebaran **ikut terkali/terbagi $|b|$** (untuk varians terkali $b^2$).
   - Tabel komparasi rumus data tunggal vs data berkelompok.
4. **Contoh Soal & Pembahasan Terperinci**:
   - Contoh 1: Menghitung $R, H, Q_d, SR, S^2,$ dan $S$ pada data tunggal nilai setoran hafalan santri.
   - Contoh 2: Menghitung $SR, S^2,$ dan $S$ pada data berkelompok (tabel distribusi frekuensi) menggunakan tabel penolong kolom ($x_i, f_i x_i, |x_i - \bar{x}|, f_i |x_i - \bar{x}|, (x_i - \bar{x})^2, f_i(x_i - \bar{x})^2$).
5. **Penerapan Kontekstual (Studi Kasus Santri & Kehidupan Nyata)**:
   - Analisis perbandingan konsistensi dan homogenitas capaian hafalan Al-Qur'an antara dua halaqah santri dengan rata-rata sama namun simpangan baku berbeda.
6. **Pola Kunci & Cara Cepat Mengingat**:
   - Jembatan keledai urutan hitung: *"Cari Mean $\rightarrow$ Cari Selisih $\rightarrow$ Kuadratkan $\rightarrow$ Jumlahkan $\rightarrow$ Bagi $n$ $\rightarrow$ Tarik Akar"*.
   - Catatan waspada: Jangan lupa nilai mutlak pada $SR$ dan jangan lupa menarik akar dari varians untuk mendapatkan simpangan baku.
7. **Latihan Soal Mandiri Terfokus**:
   - **Latihan Soal 1 (20 Soal)**: Ukuran Penyebaran Data Tunggal & Sifat Transformasi Statistik.
   - **Latihan Soal 2 (20 Soal)**: Ukuran Penyebaran Data Berkelompok (Tabel Distribusi Frekuensi).
   - **Latihan Soal 3 (20 Soal)**: Penerapan Kontekstual Santri & Pemecahan Masalah Nyata Pesantren (Murni Soal Cerita Terapan).
8. **Pekerjaan Rumah (PR Pondok / Mandiri)**:
   - 4 soal terstruktur: 1 hitung penyebaran data tunggal, 1 hitung simpangan baku tabel distribusi frekuensi, 1 studi kasus perbandingan homogenitas santri, dan 1 refleksi pemahaman konsep mandiri.
9. **Ringkasan Materi**:
   - 4 poin intisari rumus dan interpretasi ukuran penyebaran data.

---

## 4. TAHAPAN EKSEKUSI (CHECKLIST)

- [x] **Fase 1: Persiapan Direktori & Rencana Berkas**
  - [x] Menyiapkan folder `kelas-12/` pada workspace `d:\Project\exercise\math\`.
  - [x] Menentukan nama berkas target `pertemuan-08-ukuran-penyebaran-data.md`.
- [x] **Fase 2: Penyusunan Materi Inti & Rumus Baku (Bagian 1–4)**
  - [x] Menulis Bagian 1: Pengertian, konsep dasar, dan hikmah keteraturan & keadilan data.
  - [x] Menulis Bagian 2: Rumus lengkap $R, H, Q_d, SR, S^2, S$ data tunggal dan berkelompok.
  - [x] Menulis Bagian 3: Karakteristik homogenitas data, efek transformasi linier, dan tabel komparasi.
  - [x] Menulis Bagian 4: Pembahasan contoh soal bertingkat data tunggal dan berkelompok runtut baris demi baris.
- [x] **Fase 3: Penyusunan Studi Kasus, Trik Kunci, & 3 Paket Latihan (Bagian 5–7)**
  - [x] Menulis Bagian 5: Studi kasus perbandingan homogenitas dua halaqah santri tahfiz.
  - [x] Menulis Bagian 6: Jembatan keledai alur hitung dan peringatan kesalahan umum.
  - [x] Menulis Bagian 7: Tiga paket latihan soal terpisah masing-masing 20 butir soal bertingkat (total 60 soal).
- [x] **Fase 4: Penyusunan PR, Ringkasan, & Validasi Akhir (Bagian 8–9)**
  - [x] Menulis Bagian 8: Pekerjaan rumah terstruktur 4 butir soal.
  - [x] Menulis Bagian 9: Ringkasan 4 butir esensial.
  - [x] Validasi kepatuhan KaTeX LaTeX dan ketiadaan istilah terlarang (koperasi/bunga/riba/utang/pinjaman).

---

## 5. ANALISIS RISIKO & MITIGASI

- **Risiko 1**: Kompleksitas perhitungan angka desimal pada data berkelompok dapat membingungkan siswa jika angka tidak dirancang rapi.
  - *Mitigasi*: Menyiapkan angka-angka pada contoh soal dan latihan data berkelompok dengan mean bulat atau pecahan sederhana agar tabel penolong mudah dihitung tanpa kalkulator.
- **Risiko 2**: Tertukar antara rumus varians ($S^2$) dan simpangan baku ($S$), atau lupa tanda mutlak pada simpangan rata-rata ($SR$).
  - *Mitigasi*: Memberikan penekanan visual yang tegas pada Bagian 2 dan Bagian 6 (Catatan Waspada).

---

> **AWAITING APPROVAL**: Dokumen perencanaan ini berada dalam status menunggu peninjauan dan persetujuan dari pengguna. Berkas otomatis dibuka untuk ditinjau. Berikan masukan/revisi atau konfirmasi dengan instruksi **"Lanjutkan" / "Eksekusi"** sebelum penyusunan modul materi ajar dimulai.

