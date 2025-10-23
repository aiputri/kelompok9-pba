# Proyek Analisis Sentimen dan Named Entity Recognition (NER) pada Pemberitaan Layanan Ferry di Indonesia

## Kelompok 9
1. Fadillah Nur Laili - 5026221032
2. Aliffia Isma Putri - 5026221130
3. Hasna Daffa Ulinnuha - 5026221205

## Deskripsi
Proyek ini bertujuan untuk menganalisis **persepsi publik terhadap layanan ferry di Indonesia** melalui analisis sentimen dan pengenalan entitas bernama **(NER)** menggunakan teknik pemrosesan bahasa alami **(NLP)**. Dataset berita dikumpulkan dari berbagai portal berita nasional dan telah melalui proses **pembersihan serta prapemrosesan teks** sebelum dianalisis.
![WhatsApp Image 2025-10-23 at 12 13 20_edb3bdde](https://github.com/user-attachments/assets/bbffc56f-83f2-4278-b7e1-5d4e051e1866)

![WhatsApp Image 2025-10-23 at 12 14 15_a6c0c311](https://github.com/user-attachments/assets/6b518af2-1db3-4396-bfdf-1cced9b4491f)

## Fitur Utama
- **Named Entity Recognition (NER)**: Mengekstrak entitas penting seperti nama perusahaan, organisasi, lokasi, serta tanggal yang muncul dalam teks berita.
- **Visualisasi**: Menampilkan hasil analisis sentimen, tren berita, serta word cloud untuk kata-kata yang paling sering muncul.
- **Analisis Sentimen**: Mengidentifikasi sentimen positif, negatif, dan netral dalam berita terkait layanan ferry.

## Hasil Kuantitatif
Berdasarkan pengolahan dan analisis dataset berita terkait layanan ferry di Indonesia, dapat disimpulkan bahwa:
- Pemberitaan mengenai layanan ferry bersifat **informatif dan faktual**, dengan dominasi kata benda dan kata kerja yang mencerminkan deskripsi entitas dan tindakan operasional.
- **Named Entity Recognition (NER)** menunjukkan bahwa fokus pemberitaan banyak pada produk, organisasi, angka, dan tanggal, menegaskan karakter berita yang data-driven.
- Analisis sentimen menunjukkan bahwa model **Random Forest** menjadi yang terbaik dengan **akurasi 72,09%**, mampu menangkap pola sentimen pada berita yang mayoritas netral dan faktual. Model ini lebih efektif dibandingkan baseline maupun model transformer untuk dataset dengan jumlah terbatas dan karakteristik spesifik.  
  

## Teknologi yang Digunakan
- **Bahasa Pemrograman**: Python
- **Library NLP & Machine Learning**: Scikit-learn, NLTK, Sastrawi, spaCy
- **Web Scraping**: BeautifulSoup, Requests
- **Visualisasi Data**: Matplotlib, Seaborn, WordCloud
- **Manajemen Data**: Pandas, NumPy  

## Kesimpulan
Analisis ini menunjukkan bahwa pemberitaan mengenai layanan ferry di Indonesia **cenderung netral dan informasional**, mencerminkan karakter media yang berfokus pada fakta dan data. Model Random Forest terbukti paling efektif dalam menangkap pola sentimen berita berbahasa Indonesia dengan akurasi **72,09%**. Selain itu, hasil NER menegaskan bahwa entitas yang sering muncul berkaitan dengan organisasi, produk, dan tanggal, menggambarkan pemberitaan yang berorientasi pada data dan kebijakan operasional.
