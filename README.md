K-Means Clustering — Mall Customer Segmentation

> **Latihan Materi 11: K-Means Clustering**  
> Implementasi K-Means Clustering menggunakan Python pada dataset Mall Customer Segmentation.

---

##  Deskripsi Proyek

Proyek ini merupakan latihan implementasi algoritma **K-Means Clustering** untuk melakukan segmentasi pelanggan mall berdasarkan:
- **Annual Income** (Pendapatan Tahunan)
- **Spending Score** (Skor Belanja)
- **Age** (Usia)

Tujuannya adalah mengelompokkan pelanggan ke dalam beberapa segmen agar bisnis dapat memahami karakteristik tiap kelompok pelanggan dan merancang strategi pemasaran yang lebih tepat sasaran.

---



##  Visualisasi

### 1. Sebaran Data Awal (Sebelum Clustering)

Scatter plot menampilkan distribusi seluruh data pelanggan berdasarkan **Annual Income** dan **Spending Score** sebelum dilakukan proses clustering.

![Sebaran Data Awal](01_sebaran_data_awal.png)

---

### 2. Elbow Method  (Menentukan K Optimal)

Grafik Elbow Method digunakan untuk menentukan jumlah cluster (K) yang paling optimal. Titik "siku" (elbow) pada grafik menunjukkan nilai K yang ideal, yaitu saat penambahan K tidak lagi mengurangi inertia secara signifikan.

> 📌 Berdasarkan grafik, **K = 3** dipilih sebagai nilai optimal.

![Elbow Method](02_elbow_method.png)

---

### 3. Hasil K-Means Clustering (K=3)

Visualisasi hasil clustering menampilkan 3 kelompok pelanggan yang terbentuk, beserta posisi **centroid** (tanda ✕ merah) dari masing-masing cluster.

![Hasil Clustering](03_hasil_clustering.png)

---

### 4. Distribusi Fitur per Cluster (Boxplot)

Boxplot menampilkan perbandingan distribusi **Annual Income** dan **Spending Score** pada setiap cluster, sehingga memudahkan analisis karakteristik tiap kelompok.

![Boxplot Cluster](04_boxplot_cluster.png)

---

##  Hasil Analisis Cluster

| Cluster | Rata-rata Usia | Annual Income | Spending Score | Interpretasi |
|:-------:|:--------------:|:-------------:|:--------------:|:-------------|
| **0**   | 37.9 tahun     | 78.3 k$       | 68.4           |  Dewasa, penghasilan tinggi, aktif belanja |
| **1**   | 24.7 tahun     | 33.4 k$       | 76.4           |  Muda, penghasilan rendah, aktif belanja |
| **2**   | 47.6 tahun     | 56.2 k$       | 28.4           |  Paruh baya, penghasilan menengah, hemat |

---

##  Insight Bisnis

- **Cluster 0** = Pelanggan dengan daya beli tinggi dan aktif berbelanja. Cocok menjadi target utama program loyalitas dan promosi produk premium.
- **Cluster 1** = Pelanggan muda yang antusias berbelanja meski pendapatan rendah. Responsif terhadap diskon, flash sale, dan program cicilan.
- **Cluster 2** = Pelanggan yang cenderung hemat. Dapat didekati dengan penawaran produk kebutuhan sehari-hari dan promosi berbasis nilai (value-for-money).

---


