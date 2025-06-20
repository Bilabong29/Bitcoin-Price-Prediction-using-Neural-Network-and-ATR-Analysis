# Prediksi Harga Bitcoin dengan Jaringan Saraf dan Analisis ATR

**Deskripsi Proyek:**

Proyek ini bertujuan untuk membangun model peramalan harga penutupan (Close Price) Bitcoin menggunakan pendekatan Machine Learning, khususnya Jaringan Saraf Tiruan (Neural Network). Model ini memanfaatkan data historis harga Bitcoin bersama dengan indikator teknis Average True Range (ATR) sebagai fitur untuk memprediksi harga di masa depan.

**Dataset:**

Dataset yang digunakan adalah `hasil_atr_btc.csv` yang berisi data historis harga Bitcoin (Open, High, Low, Close, Volume) serta beberapa indikator teknis seperti EMA200, MACD, RSI, SMA200, dan ATR. Data telah diolah dan disiapkan untuk digunakan dalam pelatihan model.

**Metodologi:**

1.  **Memuat dan Mempersiapkan Data:** Data dibaca dari file CSV, kolom yang tidak relevan dihapus (jika ada), dan kolom tanggal diubah menjadi tipe data datetime serta dijadikan indeks. Pemeriksaan nilai yang hilang dilakukan untuk memastikan kualitas data.
2.  **Preprocessing Data:** Data dibagi menjadi fitur (X) dan target (y). Fitur yang dipilih adalah Open, High, Low, Volume, dan ATR. Data dinormalisasi menggunakan `MinMaxScaler` untuk memastikan semua fitur berada dalam rentang yang sama, yang penting untuk kinerja Jaringan Saraf. Data kemudian dibagi menjadi set pelatihan dan pengujian.
3.  **Membangun Model Jaringan Saraf:** Model Sequential Jaringan Saraf Tiruan dibangun menggunakan TensorFlow/Keras. Model terdiri dari layer input, dua hidden layer dengan aktivasi ReLU, dan layer output dengan aktivasi linear untuk tugas regresi.
4.  **Melatih Model:** Model dikompilasi menggunakan optimizer 'adam' dan loss function 'mean_squared_error'. Model dilatih menggunakan data pelatihan selama beberapa epoch, dengan validasi pada data pengujian.
5.  **Evaluasi Model:** Model dievaluasi menggunakan metrik Mean Absolute Error (MAE) dan Root Mean Squared Error (RMSE) pada data pengujian yang dinormalisasi kembali ke skala aslinya.
6.  **Visualisasi Hasil:** Hasil pelatihan (Loss vs Epoch) dan perbandingan harga aktual vs prediksi divisualisasikan untuk menganalisis kinerja model secara grafis.

**Persyaratan (Dependencies):**

*   pandas
*   numpy
*   tensorflow
*   sklearn
*   matplotlib
*   seaborn 

**Result**
![image](https://github.com/user-attachments/assets/68bd1b3a-e917-44e1-9c3d-123feecc87ec)

![image](https://github.com/user-attachments/assets/63259301-beb9-4369-a946-360e7347089b)
