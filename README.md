# 🩺 Sistem Pakar Diagnosa Penyakit Mata Berbasis Web  
### Menggunakan Metode **Forward Chaining**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222222?logo=github)

---

## 📌 Deskripsi Proyek

Proyek ini merupakan implementasi dari penelitian berjudul **“Implementasi Metode Forward Chaining Untuk Mendiagnosis Penyakit Mata Berbasis Web”** oleh **Eri Sasmita Susanto & Anggia Purbadhanti** (Universitas Teknologi Sumbawa, 2023), yang dipublikasikan dalam jurnal *Digital Transformation Technology (Digitech)*, Vol. 3, No. 2, hlm. 362–370 ([DOI: 10.47709/digitech.v3i2.2551](https://doi.org/10.47709/digitech.v3i2.2551)).

Sistem ini dirancang untuk membantu masyarakat **mengenali gejala awal penyakit mata**, khususnya **penurunan penglihatan tanpa disertai mata merah**, melalui pendekatan **sistem pakar berbasis aturan** menggunakan metode **Forward Chaining**. Tujuannya adalah meminimalkan biaya dan waktu konsultasi langsung ke klinik, sekaligus memberikan edukasi awal mengenai kemungkinan diagnosis.

---

## 🔍 Fitur Utama

- ✅ Antarmuka web berbasis HTML, CSS, dan JavaScript  
- ✅ Tampilan gelap/terang (*dark/light mode*) dengan penyimpanan preferensi  
- ✅ Halaman **About** berisi profil tim pengembang  
- ✅ Contoh halaman diagnosis (misal: `P06.html` → **Katarak Sekunder**)  
- ✅ Representasi aturan logika IF-THEN (`G10.html`)  
- ✅ Visualisasi konsep sistem pakar berdasarkan jurnal asli

> ⚠️ **Catatan**: Implementasi *forward chaining* saat ini bersifat **statis (contoh kasus)** sesuai struktur file yang tersedia. Untuk sistem dinamis penuh, diperlukan pengembangan lebih lanjut (misalnya dengan JavaScript atau backend PHP seperti pada jurnal).

---

## 🧠 Dasar Logika: Forward Chaining

Metode *Forward Chaining* dimulai dari **fakta/gejala yang diketahui**, lalu mencocokkannya dengan **aturan IF-THEN** dalam basis pengetahuan untuk menghasilkan **kesimpulan/diagnosis**.

### Data dari Jurnal:
- **14 jenis penyakit mata**, di antaranya:
  - `P001`: Katarak Kongenital  
  - `P006`: Katarak Sekunder  
  - `P007`: Glaukoma Primer  
  - `P011`: Retinopati Diabetes Melitus  
- **32 gejala klinis**, contoh:
  - `G001`: Penglihatan turun perlahan tanpa mata merah  
  - `G005`: Pandangan ganda pada objek yang sama  
  - `G010`: Tidak jelas dalam menginterpretasikan warna  
  - `G028`: Ukuran kacamata minus yang berubah  

### Contoh Aturan (dari Tabel 3 jurnal):
```text
R5: IF G001 AND G015 THEN P005 (Katarak Toksik)
R6: IF G001 AND G005 AND G010 AND G028 THEN P006 (Katarak Sekunder)