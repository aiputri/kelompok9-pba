# Peningkatan Analisis Sentimen Pemberitaan Layanan Ferry Menggunakan Fine-Tuning IndoBERT

## Kelompok 9
**Departemen Sistem Informasi - Institut Teknologi Sepuluh Nopember**
1. **Fadillah Nur Laili** - 5026221032
2. **Aliffia Isma Putri** - 5026221130
3. **Hasna Daffa Ulinnuha** - 5026221205

## Deskripsi
Proyek ini bertujuan untuk menganalisis **persepsi publik terhadap layanan ferry di Indonesia** melalui pendekatan *Natural Language Processing* (NLP). Analisis dilakukan terhadap **285 artikel berita nasional** (Detik, Kompas, CNBC) terkait "Ferizy" dan layanan penyeberangan.

Penelitian ini membandingkan performa model **Machine Learning Klasik** (Random Forest, Naive Bayes, dll) dengan model **Deep Learning berbasis Transformer (IndoBERT)** yang dilakukan proses *Fine-Tuning* untuk tugas klasifikasi sentimen dan pengenalan entitas bernama (*Named Entity Recognition*).

![WhatsApp Image 2025-10-23 at 12 13 20_edb3bdde](https://github.com/user-attachments/assets/bbffc56f-83f2-4278-b7e1-5d4e051e1866)

![WhatsApp Image 2025-10-23 at 12 14 15_a6c0c311](https://github.com/user-attachments/assets/6b518af2-1db3-4396-bfdf-1cced9b4491f)

## Fitur Utama
- **Web Scraping & Dataset Building**: Pengumpulan data otomatis menggunakan library `Newspaper3k` dan `BeautifulSoup`.
- **Linguistic Analysis (POS Tagging)**: Analisis struktur kalimat menggunakan library `Stanza` untuk mengidentifikasi dominasi kata benda dan kerja.
- **Named Entity Recognition (NER)**: Ekstraksi entitas penting menggunakan model IndoBERT untuk mendeteksi Produk, Organisasi, Angka, dan Lokasi.
- **Analisis Sentimen Komparatif**:
  - **Pendekatan Klasik**: Implementasi algoritma Random Forest, Naive Bayes, SVM, dan Logistic Regression.
  - **Pendekatan Modern**: Implementasi dan *Fine-Tuning* model pre-trained `IndoBERT-base-p1`.

## Hasil Kuantitatif & Temuan
Berdasarkan pengolahan data terhadap 285 artikel berita:

### 1. Karakteristik Pemberitaan
- **Informatif & Faktual**: Hasil POS Tagging didominasi oleh *Proper Noun* (25,598 token) dan *Noun* (23,697 token), menunjukkan berita berfokus pada objek dan entitas nyata.
- **Data-Driven**: Hasil NER menunjukkan entitas terbanyak adalah **PRD (Product)** sebanyak 4.157 dan **CRD (Cardinal Number)** sebanyak 1.753, menandakan pemberitaan sarat akan data operasional (harga, kuota, statistik).

### 2. Performa Model Analisis Sentimen
- **Model Klasik Terbaik**: **Random Forest** mencapai akurasi **72,09%**. Model ini efektif untuk dataset terbatas dengan pola kata yang jelas.
- **Model Transformer Terbaik**: **Fine-Tuned IndoBERT** berhasil mencapai performa optimal dengan akurasi **75,44%**.
- **Kesimpulan Model**: IndoBERT terbukti lebih unggul dalam menangkap konteks linguistik yang kompleks dan sentimen implisit dibandingkan model tradisional.

| Model | Akurasi | Keterangan |
| :--- | :--- | :--- |
| **Fine-Tuned IndoBERT** | **75,44%** | **Performa Terbaik (Optimal Context Understanding)** |
| Random Forest | 72,09% | Terbaik di kategori Machine Learning Klasik |
| Naive Bayes | 65,12% | - |
| SVM Linear | 63,95% | - |
| Logistic Regression | 62,79% | - |

## Teknologi yang Digunakan
- **Bahasa Pemrograman**: Python
- **Deep Learning / Transformer**: PyTorch, Hugging Face Transformers (`indobenchmark/indobert-base-p1`)
- **NLP Toolkit**: Stanza (POS Tagging), Sastrawi (Stemming)
- **Machine Learning**: Scikit-learn
- **Data Acquisition**: Newspaper3k, BeautifulSoup
- **Data Analysis & Visualization**: Pandas, NumPy, Matplotlib, Seaborn, WordCloud

## Kesimpulan
Penelitian ini menyimpulkan bahwa pemberitaan layanan ferry di Indonesia didominasi oleh sentimen **netral** dengan fokus pada aspek operasional dan kebijakan pemerintah. Meskipun model klasik seperti **Random Forest** memberikan hasil yang kompetitif (72,09%), penerapan teknik **Fine-Tuning pada IndoBERT** terbukti memberikan hasil paling akurat (**75,44%**) dan seimbang dalam memetakan opini publik, menjadikannya metode yang direkomendasikan untuk sistem monitoring media yang lebih canggih.

---
*Dibuat untuk memenuhi Laporan Project B - Mata Kuliah Pengolahan Bahasa Alami (NLP).*
