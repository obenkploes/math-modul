# Rencana Modul Materi Ajar: Matematika SMA Kelas 12 Pertemuan 9
**Topik**: Statistika Deskriptif Terpadu — Latihan & Aplikasi Analisis Data Riil Santri  
**Jenjang**: SMA / MA (Jurusan IPA & Pesantren)  
**Semester**: Ganjil  
**Alokasi Waktu**: 1 Pertemuan Mandiri (Materi Pembelajaran + 60 Latihan Soal Terpartisi + PR Mandiri)  
**Status**: Selesai Diimplementasikan (*Completed*)

---

## 1. Tujuan Pembelajaran & Ruang Lingkup Materi

### A. Tujuan Pembelajaran Siswa
Setelah mempelajari modul ini secara mandiri, santri diharapkan mampu:
1. Mengintegrasikan seluruh kompetensi statistika deskriptif (penyajian data tabel/grafik, ukuran pemusatan, ukuran letak, dan ukuran penyebaran) dalam satu alur analisis terpadu.
2. Membaca, menginterpretasi, dan menyajikan data mentah hasil pengamatan aktivitas santri ke dalam tabel distribusi frekuensi, histogram, poligon, dan ogive.
3. Melakukan komparasi performa dua atau lebih kelompok santri (misalnya antar-kamar, antar-halaqah tahfiz) menggunakan kombinasi nilai ukuran pemusatan (Mean/Median) dan ukuran variabilitas (Simpangan Baku/Varians).
4. Menarik kesimpulan analitis dan menyusun rekomendasi objektif berbasis data (*data-driven decision making*) untuk kemaslahatan pengelolaan pondok pesantren.

### B. Ruang Lingkup Materi Pertemuan 9
- **Integrasi Analisis Statistika Deskriptif**:
  - Alur investigasi data: *Pengumpulan $\to$ Pengorganisasian (Tabel & Ogive) $\to$ Pengukuran Karakteristik (Pusat, Letak, Sebar) $\to$ Interpretasi & Rekomendasi*.
- **Komparasi Multivariat Sederhana**:
  - Mengapa membandingkan rata-rata saja bisa menyesatkan (*Simpson's Paradox / Data Skewness*).
  - Menggunakan Koefisien Variasi ($KV = \frac{S}{\bar{x}} \times 100\%$) dan Angka Baku ($Z = \frac{x - \bar{x}}{S}$) untuk membandingkan konsistensi data dengan skala atau satuan yang berbeda.
- **Penerapan Kontekstual Pesantren**:
  - Evaluasi target muthola'ah kitab kuning, rekap capaian tasmi' Al-Qur'an $30\text{ juz}$, audit logistik konsumsi dapur santri, dan pemantauan kesehatan berkala di poskestren.

---

## 2. Struktur Modul (Format 9 Bagian Standar Siswa)

Modul disusun murni sebagai **bahan belajar mandiri siswa** (*student-facing*) tanpa rubrik penilaian pengajar:

1. **Pengertian & Konsep Dasar**
   - Hakikat analisis data dalam Islam: Kejujuran, ketelitian, dan objektivitas hisab (*QS. Al-Inshiqaq: 8*, *QS. Al-Zalzalah: 7-8*).
   - Mengapa seorang santri perlu memiliki keterampilan membaca data di era modern.
2. **Bentuk Umum & Rumus Baku Terpadu**
   - Rangkuman sintesis seluruh formula statistika deskriptif:
     - Aturan Sturges ($k = 1 + 3{,}3 \log n$, $p = \frac{R}{k}$)
     - Ukuran Pemusatan: $\bar{x} = \frac{\sum f_i x_i}{\sum f_i}$, $Me = L + \left(\frac{\frac{1}{2}n - \sum f_k}{f_{me}}\right) p$, $Mo = L + \left(\frac{d_1}{d_1 + d_2}\right) p$
     - Ukuran Letak: $Q_i = L + \left(\frac{\frac{i}{4}n - \sum f_k}{f_Q}\right) p$, $P_i = L + \left(\frac{\frac{i}{100}n - \sum f_k}{f_P}\right) p$
     - Ukuran Penyebaran: $SR = \frac{\sum f_i \lvert x_i - \bar{x} \rvert}{\sum f_i}$, $S = \sqrt{\frac{\sum f_i (x_i - \bar{x})^2}{\sum f_i}}$
     - Alat Ukur Komparasi Standar: Angka Baku $Z = \frac{x - \bar{x}}{S}$ dan Koefisien Variasi $KV = \frac{S}{\bar{x}} \times 100\%$.
3. **Sifat-Sifat, Karakteristik, & Matriks Keputusan Analisis**
   - Matriks pemilihan ukuran statistik berdasarkan jenis distribusi data (simetris normal vs miring/skewed).
   - Interpretasi nilai $Z$-score (santri di atas rata-rata vs memerlukan pendampingan).
4. **Contoh Soal & Pembahasan Terperinci**
   - **Contoh 1 (Tingkat Dasar - Data Tunggal Komprehensif)**: Dari data mentah skor ujian nahwu $10$ santri, hitung seluruh parameter statistik (Mean, Median, Modus, $Q_1, Q_3, H, Q_d, SR, S$), tentukan $Z$-score santri tertentu, dan interpretasikan hasilnya.
   - **Contoh 2 (Pengembangan - Data Berkelompok Komprehensif)**: Diberikan tabel distribusi frekuensi durasi muthala'ah mandiri $40$ santri, tentukan ogive, hitung Mean, Median, Modus, Persentil ke-$80$, dan Simpangan Baku, serta analisis kategori santri paling konsisten.
5. **Penerapan Kontekstual Santri**
   - Studi kasus komprehensif: Evaluasi kesiapan wisuda tasmi' Al-Qur'an santri antar-asrama berdasarkan mean, median, dan simpangan baku.
6. **Pola Kunci & Cara Cepat Mengingat**
   - Diagram alur investigasi data (*Roadmap Statistika Deskriptif*).
   - Catatan waspada jebolan umum (*common pitfalls*).
7. **Latihan Soal Mandiri (Total 60 Soal Terpartisi)**
   - **Set 1: Analisis Terpadu Data Tunggal & Transformasi Statistik (20 Soal)**
     - 4 soal pemahaman konsep & interpretasi $Z$-score / $KV$.
     - 10 soal komputasi terpadu (menghitung paket lengkap pusat, letak, sebar).
     - 6 soal penalaran & analisis aljabar statistika.
   - **Set 2: Analisis Terpadu Data Berkelompok & Kurva Frekuensi (20 Soal)**
     - 4 soal konsep tabel, frekuensi kumulatif, dan kurva ogive.
     - 10 soal komputasi data berkelompok (Mean, Median, Modus, Kuartil/Desil/Persentil, Simpangan Baku).
     - 6 soal analisis komparasi distribusi frekuensi.
   - **Set 3: Studi Kasus Kontekstual Santri & Pemecahan Masalah Nyata Pesantren (20 Soal)**
     - 20 butir soal cerita mandiri mengangkat tema hafalan Al-Qur'an, muthala'ah kitab kuning, poskestren, logistik asrama, infak majelis taklim, dan kebun pesantren.
8. **Pekerjaan Rumah (PR Mandiri / Pondok)**
   - 4 butir soal berbobot (perhitungan data tunggal, pengolahan tabel kelompok, studi kasus komparasi dua kelompok santri, dan esai refleksi analitis).
9. **Ringkasan Materi**
   - 4 poin esensial sintesis statistika deskriptif.

---

## 3. Batasan Teknis & Kepatuhan Standar

1. **Strict KaTeX LaTeX Rendering**:
   - Seluruh tag display math `$$` diletakkan rata kiri (*column 0*) dengan baris kosong sebelum dan sesudahnya (mencegah indentasi blok kode `<pre><code>`).
   - Rumus dalam sel tabel Markdown menggunakan `\lvert ... \rvert` untuk nilai mutlak/determinan.
2. **Kepatuhan Nilai Pesantren & Bebas Riba**:
   - Tidak menggunakan istilah perbankan konvensional / ribawi (*koperasi*, *bunga*, *riba*, *pinjaman*, *utang*, *kredit*, *bank*).
   - Fokus muatan kontekstual pada adab thalabul 'ilmi, infak sukarela, serta efisiensi sarana prasarana pondok pesantren.
3. **Pemisahan Latihan Soal**:
   - Soal latihan dipisah secara tegas ke dalam 3 set berurutan nomor 1–20 dengan instruksi umum terpadu.

---

## 4. Rencana Berkas Output

- Path Berkas: `d:\Project\exercise\math\kelas-12\pertemuan-09-latihan-dan-aplikasi-statistika.md`

