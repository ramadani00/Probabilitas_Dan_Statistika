## Deskripsi
Repository ini berisi analisis data sosial-ekonomi rumah tangga untuk menentukan kelayakan penerima **BPNT (Bantuan Pangan Non-Tunai)** menggunakan metode **Regresi Logistik**. Proyek ini mencakup proses pengolahan data, visualisasi, hingga evaluasi model prediksi.

## Dataset
Dataset yang digunakan berisi informasi sosial-ekonomi rumah tangga dengan variabel-variabel berikut:

- **BPNT**: Status penerimaan bantuan sosial berbentuk pangan (0: tidak menerima, 1: menerima).
- **Klasifikasi Desa/Kota**: Wilayah tempat tinggal rumah tangga (1: desa, 2: kota).
- **Jumlah Balita**: Jumlah anak balita dalam rumah tangga.
- **Jumlah ART**: Jumlah anggota rumah tangga.
- **Status Tempat Tinggal**: Kepemilikan tempat tinggal (1: milik sendiri, 2: sewa).
- **Luas Bangunan**: Luas rumah dalam meter persegi.
- **Jenis Atap**: Tipe atap rumah (1: berkualitas rendah, 2: sedang/tinggi).
- **Jenis Dinding**: Tipe dinding rumah (1: berkualitas rendah, 2: sedang/tinggi).
- **Sumber Air Minum**: Sumber air utama rumah tangga (1: bersih, 2: tidak bersih).
- **Bahan Bakar Masak**: Jenis bahan bakar memasak (1: gas/listrik, 2: kayu/bahan lain).
- **Fasilitas KUR**: Akses terhadap fasilitas pinjaman usaha (1: tidak, 2: ya).
- **Motor**: Kepemilikan motor (1: tidak, 2: ya).
- **Mobil**: Kepemilikan mobil (1: tidak, 2: ya).
- **Penghasilan Utama**: Jenis penghasilan utama rumah tangga (1: pekerjaan tetap, 2: tidak tetap).

## Fitur Utama
1. **Preprocessing Data**:
   - Mengubah data numerik menjadi kategori untuk mempermudah analisis.
   - Menangani nilai yang hilang (missing values).

2. **Visualisasi Data**:
   - Grafik pie chart untuk distribusi penerima BPNT.
   - Analisis karakteristik penerima BPNT berdasarkan variabel-variabel seperti jumlah balita, jumlah ART, dll.

3. **Modeling**:
   - Model regresi logistik untuk memprediksi penerima BPNT.
   - Evaluasi model menggunakan metrik seperti **accuracy**, **confusion matrix**, **ROC curve**, dan **AUC**.

4. **Interpretasi Model**:
   - Analisis odds ratio untuk memahami pengaruh setiap variabel.
   - Evaluasi multikolinearitas menggunakan **Variance Inflation Factor (VIF)**.

## Teknologi yang Digunakan
- **Python** dengan library:
  - `pandas`: Pengolahan data.
  - `seaborn` & `matplotlib`: Visualisasi data.
  - `scikit-learn`: Pemisahan data dan evaluasi model.
  - `statsmodels`: Pembentukan model regresi logistik.
  - `numpy`: Operasi numerik.
- **Jupyter Notebook** atau IDE seperti **VSCode** untuk pemrograman interaktif.

## Cara Menggunakan
1. Clone repository ini:
   ```bash
   git clone https://github.com/ramadani00/Lab7Web.git
   ```
2. Pastikan Anda memiliki Python dan library yang diperlukan terinstal. Anda dapat menginstalnya dengan:
   ```bash
   pip install pandas seaborn scikit-learn statsmodels matplotlib numpy
   ```
3. Jalankan file Python atau Notebook untuk melakukan analisis dan evaluasi.

## Hasil Evaluasi
- **Accuracy Model**: 73.74%
- **ROC Curve (AUC)**: 0.71
- **Confusion Matrix**:
  ```
  [[389  21]
   [130  35]]
  ```
