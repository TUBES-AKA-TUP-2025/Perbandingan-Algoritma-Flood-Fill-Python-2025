# Perbandingan Algoritma Flood Fill: Rekursif vs Iteratif (2025)

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

Proyek ini bertujuan untuk menganalisis performa algoritma **Flood Fill** (Paint Bucket Tool) melalui dua pendekatan utama: **Rekursif** dan **Iteratif berbasis Stack**. Fokus utama analisis adalah pada efisiensi waktu eksekusi, penggunaan memori, dan stabilitas algoritma terhadap ukuran grid yang bervariasi.



## 📌 Deskripsi Proyek
Analisis ini membandingkan bagaimana kedua algoritma menangani pewarnaan area tertutup pada matriks 2D:
1.  **Versi Rekursif:** Menggunakan pemanggilan fungsi diri sendiri (Implicit Stack).
2.  **Versi Iteratif:** Menggunakan struktur data Stack manual (Explicit Stack) untuk menghindari batasan *call stack* sistem.

## 📊 Analisis Kompleksitas

| Metrik | Rekursif | Iteratif (Stack) |
| :--- | :--- | :--- |
| **Waktu (Worst Case)** | $O(N^2)$ | $O(N^2)$ |
| **Ruang (Stack Space)** | $O(N^2)$ | $O(N^2)$ |
| **Stabilitas** | Rentan *Stack Overflow* | Sangat Stabil |
| **Penyimpanan Stack** | System Call Stack | Heap Memory |



### Relasi Rekurensi (Rekursif)
Untuk grid berukuran $n$ piksel, relasi dapat dinyatakan sebagai:
$$T(n) = 4T(n/4) + \Theta(1)$$
Menghasilkan total kompleksitas $\Theta(n)$ di mana $n$ adalah jumlah total piksel dalam area yang diwarnai.

## 🚀 Fitur Utama
* **Benchmarking:** Pengukuran waktu eksekusi otomatis untuk berbagai ukuran grid (10x10 hingga 150x150+).
* **Visualisasi:** Grafik perbandingan performa menggunakan `matplotlib`.
* **Stress Test:** Demonstrasi batas rekursi Python dan keunggulan stabilitas metode iteratif.

## 🛠️ Instalasi & Penggunaan

1. **Clone Repositori:**
   ```bash
   git clone [https://github.com/username/Perbandingan-Algoritma-Flood-Fill-Python-2025.git](https://github.com/username/Perbandingan-Algoritma-Flood-Fill-Python-2025.git)
   cd Perbandingan-Algoritma-Flood-Fill-Python-2025