# 🩺 Sistem Pakar Diagnosa Penyakit Mata Berbasis Web  
### Penerapan Metode **Forward Chaining**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222222?logo=github)

---

## 👥 Informasi Kelompok

**Mata Kuliah** : Logika Informatika  
**Jenis Tugas** : Penerapan Metode Forward Chaining  
**Kelompok** : Arif  

### Anggota Kelompok
- **JUNDULLOH RIZKI ANANDA** – Ketua Kelompok  
- **ADITTIA RAMADHAN** – Anggota  
- **ALIF MAS SASTRO NUGROHO** – Anggota  
- **ARIF RAHMAN HAKIM** – Anggota  
- **SUPRIYAN** – Anggota  

---

## 📘 Latar Belakang

Kesehatan mata merupakan aspek penting dalam kualitas hidup manusia. Namun, keterbatasan akses terhadap dokter spesialis mata, terutama di daerah tertentu, sering menyebabkan keterlambatan diagnosis penyakit mata. Oleh karena itu, diperlukan sebuah sistem yang dapat membantu memberikan **diagnosis awal secara cepat dan sistematis**.

Proyek ini merupakan implementasi **tugas mata kuliah Logika Informatika** yang menerapkan konsep **Sistem Pakar** dengan metode **Forward Chaining** dalam bentuk **aplikasi berbasis web**.

---

## 📄 Dasar Penelitian (Jurnal Acuan)

Sistem ini mengacu pada jurnal ilmiah berikut:

> **Eri Sasmita Susanto & Anggia Purbadhanti (2023)**  
> *Implementasi Metode Forward Chaining Untuk Mendiagnosis Penyakit Mata Berbasis Web*  
> Jurnal **Digital Transformation Technology (Digitech)**  
> Vol. 3, No. 2, Hal. 362–370  
> DOI: https://doi.org/10.47709/digitech.v3i2.2551  

Penelitian tersebut membahas penerapan metode **Forward Chaining** untuk mendiagnosis penyakit mata berdasarkan **gejala klinis**, khususnya pada kasus **penurunan penglihatan tanpa disertai mata merah**.

---

## 🎯 Tujuan Sistem

- Menerapkan konsep **forward chaining** dalam bentuk sistem pakar
- Membantu pengguna mengenali **kemungkinan penyakit mata secara dini**
- Memberikan **edukasi awal** sebelum pemeriksaan medis lanjutan
- Menjadi media pembelajaran penerapan logika IF–THEN dalam informatika

---

## 🧠 Konsep Forward Chaining

Metode **Forward Chaining** adalah teknik inferensi yang dimulai dari **fakta atau gejala awal**, kemudian mencocokkannya dengan **aturan (rules)** dalam basis pengetahuan hingga menghasilkan **kesimpulan (diagnosis)**.

Alur logika sistem:
1. Pengguna memilih atau menjawab gejala
2. Sistem mencocokkan gejala dengan aturan IF–THEN
3. Jika kondisi terpenuhi, sistem menarik kesimpulan berupa diagnosis penyakit

---

## 📊 Data Pengetahuan (berdasarkan jurnal)

### 🦠 Jenis Penyakit Mata
Sistem ini mengacu pada **14 jenis penyakit mata**, di antaranya:
- **P001**: Katarak Kongenital  
- **P005**: Katarak Toksik  
- **P006**: Katarak Sekunder  
- **P007**: Glaukoma Primer  
- **P011**: Retinopati Diabetes Melitus  
- **P012**: Retinopati Diabetes Proliferatif  

### 👁️ Gejala Klinis
Terdapat **32 gejala**, contoh:
- **G001**: Penglihatan turun perlahan tanpa mata merah  
- **G004**: Kemampuan penglihatan berkurang  
- **G005**: Pandangan ganda pada objek yang sama  
- **G010**: Kesulitan membedakan warna  
- **G015**: Kekeruhan pada lensa mata
- **G028**: Ukuran kacamata minus sering berubah  

---

## 🔗 Contoh Aturan (Rule IF–THEN)

Contoh aturan forward chaining yang digunakan:

```text
Responden 5   : IF G001 AND G015 THEN P005 (Katarak Toksik)
Responden 6   : IF G001 AND G005 AND G010 AND G028 THEN P006 (Katarak Sekunder)
Responden 12  : IF G01 AND G15 AND G04 AND G14 THEN P012 (Retinopati Diabetes Proliferatif)
