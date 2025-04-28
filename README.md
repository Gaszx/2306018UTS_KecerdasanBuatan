# UTS Kecerdasan Buatan 2025

**Nama**: Bagas Sujiwo 
**NIM**: 2306018  
**Dosen Pengampu**: Leni Fitriani, S.T., M.Kom

## Deskripsi Proyek
Ujian Tengah Semester (UTS) Mata Kuliah Kecerdasan Buatan. Terdiri dari dua tugas utama:

1. **Soal 1**: Pembuatan Sistem Pakar Deteksi Hama Tanaman berbasis aturan logika.
2. **Soal 2**: Review jurnal tentang penerapan AI dan ide pengembangan lanjutan.

---

## Struktur Repository
```
UTS_KecerdasanBuatan/
├── ScreenShot/
│   ├── Soal-1_SistemPakar_prolog.png
│   └── Soal-1_SistemPakar_py.png
├── Soal-1/
│   ├── Soal_1_SistemPakar.ipynb
│   ├── soal_1_sistempakar.py
│   └── soal_1_sistempakar[Prolog]
├── Soal-2/
│   ├── Review Jurnal.docx
│   └── The Strategy for Developing a Marketplace Promotion Model Based on AI to Improve Online Marketing in Indonesia.pdf
└── README.md
```

> **Catatan**: Gunakan jalur folder `UTS_KecerdasanBuatan` sebagai root saat menjalankan skrip dan membaca dokumen.

---

## Soal 1: Sistem Pakar Deteksi Hama Tanaman

### Deskripsi
Membuat sistem pakar berbasis logika proposisional untuk mengidentifikasi jenis hama tanaman berdasarkan gejala:
- Daun menguning
- Terdapat bercak hitam
- Daun berlubang
- Tanaman layu

### Langkah Pengerjaan
1. **Definisi Aturan Logika**  
   Minimal 4 aturan:  
   - Jika daun menguning **dan** tanaman layu → kemungkinan hama kutu daun.  
   - Jika bercak hitam **dan** daun berlubang → kemungkinan hama ulat.  
   - Jika daun menguning **dan** bercak hitam → kemungkinan hama jamur.  
   - Jika daun berlubang **dan** tanaman layu → kemungkinan hama wereng.

2. **Pseudocode**
   ```
   // Input gejala sebagai boolean (Y/N)
   INPUT: daun_menguning, bercak_hitam, daun_berlubang, tanaman_layu

   IF daun_menguning AND tanaman_layu:
       DIAGNOSA = "Kutu Daun"
   ELIF bercak_hitam AND daun_berlubang:
       DIAGNOSA = "Ulat"
   ELIF daun_menguning AND bercak_hitam:
       DIAGNOSA = "Jamur"
   ELIF daun_berlubang AND tanaman_layu:
       DIAGNOSA = "Wereng"
   ELSE:
       DIAGNOSA = "Gejala tidak dikenali"
   OUTPUT: DIAGNOSA
   ```

3. **Implementasi**  
   File: `Soal-1/soal_1_sistempakar.py`  
   Jalankan:
   ```bash
   cd UTS_KecerdasanBuatan/Soal-1
   python3 soal_1_sistempakar.py
   ```
   - Ikuti instruksi input gejala (Y/N).
   - Sistem akan menampilkan diagnosa hama.

4. **Inferensi**  
   Sistem mengevaluasi setiap aturan secara berurutan hingga menemukan kecocokan pertama. Jika tidak ada, hasilnya “Gejala tidak dikenali.”

---

## Soal 2: Review Jurnal AI

### Judul & Sumber
> **Studi Kasus Pengembangan dan Penggunaan Artificial Intelligence (AI) Sebagai Penunjang Kegiatan Masyarakat Indonesia**  
> _International Journal of Social Science and Business (IJSSB), SINTA 2_

File review: `Soal-2/Review Jurnal.docx`  
PDF asli: `Soal-2/The Strategy for Developing a Marketplace Promotion Model Based on AI to Improve Online Marketing in Indonesia.pdf`

### Ringkasan
- **Tujuan**: Menganalisis penerapan AI di sektor publik, kesehatan, pendidikan, dan transportasi cerdas.  
- **Metode AI**: Machine Learning untuk prediksi, NLP untuk chatbot layanan publik, Computer Vision untuk deteksi dini.  
- **Manfaat**:
  - Mempercepat pelayanan publik.  
  - Deteksi dini masalah kesehatan.  
  - Pendidikan adaptif berbasis data.  
  - Transportasi cerdas dengan prediksi rute.

### Ide Pengembangan Lanjutan
1. AI yang menghormati etika & budaya lokal.  
2. Aplikasi mobile ringan untuk daerah terpencil.  
3. Rekomendasi cerdas berbasis data komunitas.  
4. Explainable AI (_XAI_) untuk transparansi.

### Ide Aplikasi Komunitas

**CocoGarut SmartHub**: Aplikasi AI-driven untuk penjualan dan distribusi kelapa di Garut yang menghubungkan petani, pengepul, dan pembeli akhir.

- **Profil Panen Pintar**: Petani mengirimkan prediksi panen harian dan foto sampel buah; AI merekomendasikan hari panen optimal berdasarkan data cuaca dan kematangan.
- **Rekomendasi Pembeli Adaptif**: Neural network ringan mempelajari pola belanja konsumen (santan, kopra, olahan) dan menampilkan penawaran lokal dengan bundling produk tetangga.
- **Logistik Dinamis**: Algoritma rute berbobot merencanakan jadwal dan jalur pickup kelapa paling efisien, menurunkan biaya angkut hingga 20%.
- **Analisis Kualitas Otomatis**: Computer vision menilai tingkat kesegaran buah sebelum pengiriman, memberikan skor mutunya dan memastikan konsistensi kualitas.

---

## Dokumentasi Proses
1. **Analisis Masalah**: Menentukan gejala hama dan kebutuhan review jurnal.  
2. **Perancangan**: Menyusun aturan logika dan kerangka review.  
3. **Implementasi**: Kode Python untuk sistem pakar dan dokumen review.  
4. **Pengujian**: Menjalankan berbagai skenario input untuk validasi diagnosa.  
5. **Penyusunan**: Menyusun README sebagai ringkasan lengkap.

---

## Referensi
- Jurnal AI Masyarakat Indonesia, IJSSB Vol. 8 No. 1, 2024.  
- Documentasi Python AI Libraries: TensorFlow, scikit-learn, spaCy.  
- Artikel Machine Learning & NLP (Towards Data Science).

---

**Garut, 28 April 2025**

**Leni Fitriani, S.T., M.Kom**

