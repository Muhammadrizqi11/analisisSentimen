
# Analisis Sentimen Komentar YouTube studi kasus video ferry irwandi terhadap Isu Kerusakan Alam Raja Ampat

## 📌 Project Overview

Proyek ini bertujuan untuk menganalisis komentar YouTube pada video yang membahas isu kerusakan lingkungan akibat penambangan di Raja Ampat. Dengan menggunakan model AI (IBM Granite), komentar-komentar dianalisis untuk mengidentifikasi sentimen, indikasi aktivitas buzzer, dan topik utama yang dibahas publik.

Pendekatan ini digunakan untuk memahami bagaimana publik merespons isu lingkungan, serta mengukur persepsi terhadap konten yang bersifat kontroversial di media sosial.

---

## 📂 Raw Dataset Link

- [komentar_raja_ampat.csv](./komentar_raja_ampat.csv) — Dataset asli hasil scraping dari YouTube
- [hasil_final_sentimen_raja_ampat.csv](./hasil_final_sentimen_raja_ampat.csv) — Dataset hasil analisis & parsing menggunakan IBM Granite

---

## 📊 Insight & Findings

- Mayoritas komentar menunjukkan **keprihatinan terhadap kerusakan alam**, tetapi model AI awal sering mengklasifikasikan sebagai sentimen "negatif" karena kata-kata emosional.
- **Topik dominan** dalam komentar adalah *kerusakan lingkungan* dan *penolakan terhadap aktivitas tambang*.
- Indikasi buzzer relatif rendah, menunjukkan bahwa komentar berasal dari audiens organik, bukan aktor berbayar.
- Model AI seperti IBM Granite efektif secara struktural, tetapi perlu **penyesuaian konteks sosial** agar akurat dalam isu moral dan lingkungan.

---

## 🤖 AI Support Explanation

- Model AI yang digunakan: `ibm-granite/granite-3.3-8b-instruct` via [Replicate](https://replicate.com)
- Platform: Google Colab
- Proses yang dilakukan:
  1. Scraping komentar dari YouTube
  2. Pembersihan teks dan transformasi batch
  3. Prompting ke model IBM Granite
  4. Parsing hasil model ke dalam bentuk DataFrame
  5. Visualisasi: sentimen, topik, buzzer

Model IBM Granite digunakan untuk mengotomatisasi klasifikasi sentimen dan topik. Prompt dimodifikasi untuk memastikan bahwa komentar yang *peduli lingkungan* diklasifikasikan sebagai **positif**, meskipun secara emosional negatif.

---

## ✅ Author

[Rizqi Muhammad](https://github.com/Muhammadrizqi11)

---


