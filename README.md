# 🧠 CASE BASED REASONING TERHADAP PUTUSAN PENGANIAYAAN

Proyek ini merupakan implementasi metode *Case-Based Reasoning (CBR)* untuk melakukan retrieval kasus penganiayaan berdasarkan putusan pengadilan. Sistem ini dibangun menggunakan Python dengan pipeline mulai dari preprocessing, representasi vektor (TF-IDF atau BERT), hingga evaluasi retrieval.

---

### **Tahap 1 Disusun Oleh** 👨‍🎓✒️
>**Nama: Fitra Romeo Winky**

>**NIM: 202210370311056**

>**Nama: Muhammad Aunul Hakim**

>**NIM: 202210370311073**

>**Kelas: C**

>**Mata Kuliah: Penalaran Komputer**

>**Jurusan: Informatika**

---

## 🔁 TAHAPAN NOTEBOOKS

1. 

# Sistem Case-Based Reasoning (CBR) untuk Analisis Putusan Narkotika

Repositori ini merupakan implementasi end-to-end dari sistem penalaran berbasis kasus (*Case-Based Reasoning*) yang dirancang untuk mendukung analisis putusan pengadilan perkara narkotika di Indonesia. Sistem ini terdiri dari lima tahap utama, mulai dari pembangunan basis kasus hingga evaluasi model.

di buat oleh :
 - Muhammad Syahrul Bachtiar
 - Andika Nur Islamy
## 📁 Struktur Proyek

| Tahap | Deskripsi |
|------|-----------|
| **Tahap 1 – Membangun Case Base** | Scraping dan akuisisi data putusan dari Direktori Putusan Mahkamah Agung RI, termasuk metadata dan file PDF. |
| **Tahap 2 – Case Representation** | Konversi dokumen PDF menjadi format teks terstruktur yang dapat diekstraksi fiturnya untuk proses analisis lebih lanjut. |
| **Tahap 3 – Case Retrieval** | Pencarian kasus serupa menggunakan dua pendekatan: TF-IDF (leksikal) dan BERT (semantik). |
| **Tahap 4 – Solution Reuse** | Penggunaan kembali solusi dari kasus terdekat menggunakan strategi *majority vote* untuk prediksi putusan. |
| **Tahap 5 – Model Evaluation** | Evaluasi kuantitatif terhadap performa retrieval (Hits@k dan MRR) serta simulasi tugas prediksi atribut. |

## ⚙️ Teknologi yang Digunakan

- Python 3.x
- `asyncio`, `aiohttp`, `BeautifulSoup4` (Web Scraping)
- `PyMuPDF`, `pdfminer.six` (Ekstraksi PDF)
- `scikit-learn` (TF-IDF)
- `transformers`, `sentence-transformers` (BERT Embedding)
- `pandas`, `numpy`, `matplotlib` (Analisis dan Visualisasi)

## 📊 Evaluasi

Evaluasi dilakukan menggunakan dua metrik utama:
- **Hits@k**: Mengukur apakah dokumen target muncul di hasil top-k.
- **MRR (Mean Reciprocal Rank)**: Mengukur rata-rata posisi dari hasil yang benar.

Selain itu, sistem juga diuji untuk tugas prediksi atribut "jenis perkara" menggunakan hasil Top-1 dari pencarian semantik.

## 💡 Tujuan

Proyek ini bertujuan untuk mengeksplorasi potensi *Case-Based Reasoning* yang diperkuat dengan NLP modern dalam mendukung otomasi analisis hukum, khususnya pada kasus narkotika, dengan harapan dapat memberikan kontribusi terhadap sistem pendukung pengambilan keputusan hukum di Indonesia.

## 📌 Catatan

- Semua data diperoleh dari [https://putusan3.mahkamahagung.go.id](https://putusan3.mahkamahagung.go.id).
- Gunakan file `.ipynb` secara berurutan untuk mereplikasi proses dari awal hingga akhir.

## 📥 Lisensi

Proyek ini menggunakan lisensi [MIT](LICENSE) — silakan digunakan dan dikembangkan lebih lanjut dengan mencantumkan atribusi yang sesuai.
