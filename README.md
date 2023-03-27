# Submission 1: Klasifikasi tweet positif atau negatif
Nama: Habib Azizul Haq

Username dicoding: kuroba_izzul

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Sentiment Analysis of Tweet Reviews](https://www.kaggle.com/datasets/shibbirahmad22/sentiment-analysis-of-tweet-reviews?select=train.csv) |
| Masalah | Dizaman sekarang kita sering menghabiskan waktu di media sosial, baik sekedar melihat-lihat saja atau memantau idola kita di media sosialnya. Tak jarang saat kita sedang berselancar di media sosial kita menemukan tweet yang dirasa kurang sedap atau terlalu vulgar. Tentu kita akan merasa risih dan terganggu oleh hal tersebut. |
| Solusi machine learning | Untuk mengatasi masalah tersebut kita bisa membuat sebuah model machine learning untuk mengklasifikasikan sebuah tweet, apakah tweet itu bermuatan posotif atau justru negatif. |
| Metode pengolahan | Pertama kita akan melaukan proses data ingestion. Pada proses ini kita menggunakan komponen **ExampleGen()** dan membagi dataset kita menjadi training dan evaluasi dengan perbandingan 8:2. Kedua kita akan melakukan proses Data Validation, pada proses ini kita akan menggunakan komponen **StatisticsGen()** untuk mengetahui detil dari dataset kita, komponen **ShcemaGen()** untuk membuat data schema, komponen **ExampleValidator()** untuk mengidentifikasi anomali pada dataset. Ketiga kita akan masuk ke tahap Data Preprocessing, pada proses ini kita akan menggunakan komponen **Transform()**, untuk mengubah dataset kita menjadi data yang siap digunakan oleh Model. |
| Arsitektur model | Model ini memiliki Arsiteksur **TextVectorization** untuk memetakan fitur teks ke urutan bilangan bulat, **Embedding** Mengubah bilangan bulat positif (indeks) menjadi vektor padat dengan ukuran tetap, **GlobalAveragePooling1D** penyatuan rata-rata global untuk data temporal. **Dense Layer** merupakan hidden layer untuk pemrosesan neural network, dan outputs nya hanya menggunakan sigmoid untuk mengklasifikasikan element menjadi 0 dan 1.|
| Metrik evaluasi | Metrik yang dipakai disini adalah BinaryAccuracy karena hanya klasifikasi biner. Cara kerja metrik ini yaitu membuat dua variabel lokal, total dan count yang digunakan untuk menghitung frekuensi yang y_pred yang cocok dengan y_true. Frekuensi ini pada akhirnya dikembalikan sebagai binary accuracy|
| Performa model | Model memiliki performa sangat baik dalam mengklasifikasi dengan memiliki skor true yaitu 0.94780 dengan nilai loss 0.24522 |
