# Submission 1: Klasifikasi tweet positif atau negatif
Nama: Habib Azizul Haq

Username dicoding: kuroba_izzul

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Sentiment Analysis of Tweet Reviews](https://www.kaggle.com/datasets/shibbirahmad22/sentiment-analysis-of-tweet-reviews?select=train.csv) |
| Masalah | Dizaman sekarang kita sering menghabiskan waktu di media sosial, baik sekedar melihat-lihat saja atau memantau idola kita di media sosialnya. Tak jarang saat kita sedang berselancar di media sosial kita menemukan tweet yang dirasa kurang sedap atau terlalu vulgar. Tentu kita akan merasa risih dan terganggu oleh hal tersebut. |
| Solusi machine learning | Untuk mengatasi masalah tersebut kita bisa membuat sebuah model machine learning untuk mengklasifikasikan sebuah tweet, apakah tweet itu bermuatan posotif atau justru negatif. |
| Metode pengolahan | Pertama kita akan melaukan proses data ingestion. Pada proses ini kita menggunakan komponen **ExampleGen()** dan membagi dataset kita menjadi training dan evaluasi dengan perbandingan 8:2. Kedua kita akan melakukan proses Data Validation, pada proses ini kita akan menggunakan komponen **StatisticsGen()** untuk mengetahui detil dari dataset kita, komponen **ShcemaGen()** untuk membuat data schema, komponen **ExampleValidator()** untuk mengidentifikasi anomali pada dataset. Ketiga kita akan masuk ke tahap Data Preprocessing, pada proses ini kita akan menggunakan komponen **Transform()**, untuk mengubah dataset kita menjadi data yang siap digunakan oleh Model. |
| Arsitektur model | Deskripsi arsitektur model yang diguanakan |
| Metrik evaluasi | Deksripsi metrik yang digunakan untuk mengevaluasi performa model |
| Performa model | Deksripsi performa model yang dibuat |
