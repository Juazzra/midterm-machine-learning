# UTS Machine Learning: Customer Segmentation Clustering

Repository ini disusun sebagai tugas Ujian Tengah Semester (UTS) mata kuliah Machine Learning. Proyek ini bertujuan untuk melakukan **Clustering (Pengelompokan)** pada data pelanggan kartu kredit untuk memahami pola perilaku penggunaan kartu kredit.

## 👤 Identitas Mahasiswa
* **Nama:** Juandra Alghifary
* **NIM:** 1103220165

## 📊 Deskripsi Dataset
Dataset yang digunakan adalah `clusteringmidterm.csv` yang berisi data transaksi pengguna kartu kredit selama 6 bulan.
* **Total Baris:** 8950 data
* **Fitur Utama:** `BALANCE`, `PURCHASES`, `CASH_ADVANCE`, `CREDIT_LIMIT`, `PAYMENTS`, dll.
* **Tujuan:** Mengelompokkan customer ke dalam segmen yang berbeda (misal: Hemat, Boros, Sering Tarik Tunai).

## 🛠️ Metodologi
1.  **Data Preprocessing:**
    * Menghapus kolom `CUST_ID` (tidak relevan untuk clustering).
    * Mengisi nilai kosong (*Missing Values*) dengan nilai rata-rata (Mean).
    * Melakukan **Standard Scaling** agar skala data seragam.
2.  **Modeling:**
    * Algoritma: **K-Means Clustering**.
    * Menentukan jumlah cluster (k) terbaik menggunakan **Elbow Method**.
    * Jumlah Cluster yang dipilih: **k = 4**.
3.  **Visualisasi:**
    * Menggunakan **PCA (Principal Component Analysis)** untuk mereduksi dimensi data menjadi 2D agar hasil cluster bisa divisualisasikan dalam grafik scatter plot.

## 🚀 Cara Menjalankan Code
1.  Pastikan Python dan library berikut sudah terinstall:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
2.  Clone repository ini atau download file `tugas_clustering.ipynb`.
3.  Pastikan file dataset `clusteringmidterm.csv` berada dalam satu folder dengan notebook.
4.  Jalankan notebook menggunakan Jupyter Notebook, Google Colab, atau VS Code.

## 📈 Hasil Analisis
Model berhasil membagi pelanggan menjadi 4 kelompok (Cluster) dengan karakteristik penggunaan saldo dan pembayaran yang berbeda, yang divisualisasikan menggunakan grafik PCA.
