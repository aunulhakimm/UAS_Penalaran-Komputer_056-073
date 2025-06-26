# 🧠 CASE BASED REASONING TERHADAP PUTUSAN PENGANIAYAAN

Proyek ini merupakan implementasi metode *Case-Based Reasoning (CBR)* untuk melakukan retrieval kasus penganiayaan berdasarkan putusan pengadilan. Sistem ini dibangun menggunakan Python dengan pipeline mulai dari preprocessing, representasi vektor (TF-IDF atau BERT), hingga evaluasi retrieval.

---

**Proyek Ini Disusun Oleh:** 👨‍🎓✒️
>**Nama: Fitra Romeo Winky**

>**NIM: 202210370311056**

>**Nama: Muhammad Aunul Hakim**

>**NIM: 202210370311073**

>**Kelas: C**

>**Mata Kuliah: Penalaran Komputer**

>**Jurusan: Informatika**

---

## ⁉️ CARA MENGGUNAKAN:
*⚠️ Notebook ini menggunakan lingkungan kerja Google Colab‼️*

| Tahap | Deskripsi |
|------|-----------|
| **Tahap 1** | Buka folder *notebook* dan perhatikan nama filenya. |
| **Tahap 2** | Setiap file sudah diberi nama dengan tahapannya masing-masing dan urut dari tahap 1 - 5. |
| **Tahap 3** | Buka setiap file di Google Colab. |
| **Tahap 4** | Buka Drive dan buat folder secara manual di MyDrive, folder direktori yang perlu dibuat adalah sebagai berikut: SEMESTER 6/Penalaran Komputer/UAS_Penalaran Komputer |
| **Tahap 5** | Jika sudah, maka letakkan folder *data* *PDF* *CSV* di direktori tersebut. |
| **Tahap 6** | Jalankan notebook seperti biasa dan sesuai tahapan. |

## 🔁 TAHAPAN NOTEBOOKS:

| Tahap | Deskripsi |
|------|-----------|
| **Tahap 1 – Membangun Case Base** | Scraping dan akuisisi data putusan dari Direktori Putusan Mahkamah Agung RI, termasuk metadata dan file PDF. |
| **Tahap 2 – Case Representation** | Konversi dokumen PDF menjadi format teks terstruktur yang dapat diekstraksi fiturnya untuk proses analisis lebih lanjut. |
| **Tahap 3 – Case Retrieval** | Pencarian kasus serupa menggunakan dua pendekatan: TF-IDF (leksikal) dan BERT (semantik). |
| **Tahap 4 – Solution Reuse** | Penggunaan kembali solusi dari kasus terdekat menggunakan strategi *majority vote* untuk prediksi putusan. |
| **Tahap 5 – Model Evaluation** | Evaluasi kuantitatif terhadap performa retrieval. |

## ⚙️ TEKNOLOGI YANG DIGUNAKAN:

- Python 3.x
- `asyncio`, `aiohttp`, `BeautifulSoup4` (Web Scraping)
- `PyMuPDF`, `pdfminer.six` (Ekstraksi PDF)
- `scikit-learn` (TF-IDF)
- `transformers`, `sentence-transformers` (BERT Embedding)
- `pandas`, `numpy`, `matplotlib` (Analisis dan Visualisasi)

## 📌 SUMBER

- Semua data diperoleh dari [https://putusan3.mahkamahagung.go.id](https://putusan3.mahkamahagung.go.id).
- Gunakan file `.ipynb` secara berurutan untuk mereplikasi proses dari awal hingga akhir.
