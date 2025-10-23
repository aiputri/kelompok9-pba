# 🚢 Proyek Analisis Sentimen dan Named Entity Recognition (NER) pada Pemberitaan Layanan Ferry di Indonesia

## Kelompok 9
1. Fadillah Nur Laili - 5026221032
2. Aliffia Isma Putri - 5026221130
3. Hasna Daffa Ulinnuha - 5026221205

## 🧭 Deskripsi
Proyek ini bertujuan untuk menganalisis persepsi publik terhadap layanan ferry di Indonesia melalui pendekatan *Natural Language Processing* (NLP), khususnya analisis sentimen dan *Named Entity Recognition* (NER).  
Data dikumpulkan dari berbagai portal berita daring nasional seperti **Kompas**, **Detik**, dan **CNBC Indonesia**, dengan total **285 artikel berita** yang telah dikumpulkan menggunakan metode *web scraping*.  

Analisis dilakukan untuk memahami bagaimana media membingkai isu layanan ferry, meliputi aspek **infrastruktur, operasional, tiket, keselamatan**, serta **digitalisasi layanan**.  
Selain itu, penelitian ini juga menilai kinerja beberapa metode analisis sentimen dan mengidentifikasi entitas utama yang sering muncul dalam berita untuk melihat fokus pemberitaan media.

---

## ⚙️ Fitur Utama
- **Analisis Sentimen:**  
  Mengidentifikasi polaritas sentimen (positif, negatif, netral) dari setiap artikel berita. Model **Random Forest** terbukti menghasilkan akurasi terbaik sebesar **72,09%**, lebih unggul dari pendekatan leksikon dan model transformer untuk dataset berukuran kecil.

- **Named Entity Recognition (NER):**  
  Mengekstraksi entitas penting dari teks seperti **nama produk, organisasi, angka, dan tanggal**, yang menunjukkan karakter berita yang cenderung data-driven dan informasional.

- **Analisis Frekuensi & Topik:**  
  Menghitung kemunculan kata dan topik dominan seperti *kapal*, *pelabuhan*, *penumpang*, *feri*, dan *tiket*, serta memetakan topik utama pemberitaan — seperti **infrastruktur (34,7%)**, **operasional & jadwal (26,3%)**, dan **tiket & tarif (11,6%)**.

- **Visualisasi Data:**  
  Menampilkan hasil analisis dalam bentuk **grafik tren pemberitaan per kuartal**, **word cloud**, dan **diagram batang topik dominan** untuk mempermudah interpretasi hasil.

---

## 📊 Hasil Utama
- **Total Artikel:** 285 berita (2018–2025)  
- **Rata-rata Panjang Artikel:** 247 kata  
- **Total Kata Dianalisis:** 68.796 kata  
- **Distribusi Sentimen:**  
  - Netral: 86.3%  
  - Positif: 6.3%  
  - Negatif: 7.4%  

- **Topik Teratas:**  
  1. Infrastruktur (34.7%)  
  2. Operasional & Jadwal (26.3%)  
  3. Tiket & Tarif (11.6%)  
  4. Keselamatan & Kecelakaan (6.7%)  
  5. Musim Mudik (6.7%)

---

## 🧠 Insight
Pemberitaan mengenai layanan ferry di Indonesia **bersifat informasional dan faktual**, dengan dominasi kata benda dan kata kerja yang menggambarkan entitas serta tindakan operasional.  
Hasil NER menunjukkan fokus berita pada **produk, organisasi, dan angka**, mencerminkan karakter berita yang **data-driven**.  
Model **Random Forest** menghasilkan performa terbaik (akurasi 72,09%) karena mampu menangkap pola sentimen dalam teks berbahasa Indonesia yang mayoritas netral dan faktual.  

---

## 📁 Teknologi yang Digunakan
- **Python**
- **BeautifulSoup & Newspaper3k** – Web scraping  
- **Sastrawi** – Preprocessing (stemming & stopwords removal)  
- **Stanza & IndoBERT** – POS Tagging dan NER  
- **Scikit-learn** – Machine Learning (Random Forest)  
- **Matplotlib & WordCloud** – Visualisasi data  

---

## 📅 Kesimpulan
Analisis ini menunjukkan bahwa pemberitaan layanan ferry di Indonesia berfokus pada aspek **infrastruktur dan operasional**, dengan kecenderungan sentimen **netral**.  
Pendekatan NLP memberikan wawasan yang mendalam mengenai bagaimana media daring membingkai isu transportasi laut, serta dapat dimanfaatkan oleh pemerintah dan operator untuk **meningkatkan strategi komunikasi publik dan pelayanan transportasi.**