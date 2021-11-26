# 14IF_Multi-label-Emotion-Classification
14 IF 2018 - Proyek Pemrosesan Bahasa Alami (PBA) 

#Judul : Penerapan SqueezeBERT dalam Klasifikasi Emosi Multi-label dengan menggunakan PyTorch dan Tez.

#Latar Belakang: 
Saat ini banyak orang yang suka mengekspresikan emosi mereka atau berbagai peristiwa yang berarti ke orang lain melalui media sosial.
Deteksi emosi merupakan masalah klasifikasi emosi multi-label, yang terlebih dahulu akan melabeli setiap emosi pada data latih yang diberikan, kemudian berdasarkan hal
itu akan dihitung skor prediksi emosi dari suatu data testing untuk akhirnya menentukan emosi apa yang hendak disampaikan dari data testing tersebut.
Dalam proses klasifikasi emosi multi label ini akan diterapkan pada model SqueezeBERT. SqueezeBERT sudah dianggap cukup baik dan lebih cepat dalam masalah klasifikasi
multi label. Berbeda dengan model bahasa lainnya yang hanya dapat membaca input teks satu arah, model ini dirancang untuk dapat membaca inputan teks dari dua arah.
Hal ini membuat prosesnya menjadi lebih cepat.

#Tujuan :
* Menerapkan model SqueezeBERT dalam proses pengklasifikasian emosi multi label berdasarkan skor prediksi emosi yang dihasilkan terhadap data training 
dan testing dalam skala data yang besar.
* Mengetahui tingkat keakuratan klasifikasi emosi yang dihasilkan ketika dilakukan pengujian terhadap kalimat baru.

#Ruang Lingkup :
* Penelitian ini menggunakan pendekatanSqueezeBERT.
* Library yang digunakan pada proyek ini adalah PyTorch dan Tez.  PyTorch merupakan library opensource yang digunakan untuk mengembangkan dan melatih neural network.  PyTorch menggunakan dinamis sehingga lebih fleksibel untuk data yang lebih kompleks.  Tez adalah pelatih super sederhana dan ringan untuk PyTorch dan dilengkapi dengan banyak utilitas yang dapat Anda gunakan untuk menangani lebih dari 90% proyek pembelajaran mendalam di PyTorch. 
* Data set yang digunakan pada penelitian ini merupakan dataset GoEmotions(sumber:https://huggingface.co/datasets/go_emotions)
Kumpulan data GoEmotions berisi 58 ribu komentar Reddit yang dikuratori dengan cermat  kemudian diberi label sebanyak 27 kategori emosi atau Netral.  Data mentah disertakan dengan versi dataset yang lebih kecil dan disederhanakan dengan pemisahan train/val/test yang telah ditentukan sebelumnya.  Adapun konfigurasi yang disederhanakan pada dataset adalah: Teks: komentar reddit Labels: anotasi emosi comment id: pengenal unik dari komentar (dapat digunakan untuk mencari entri dalam dataset mentah) Dataset bekerja untuk klasifikasi multi-kelas, dan multi klasifikasi emosi multi-label.  Data yang digunakan merupakan data berbahasa inggris

#Hasil :
Melakukan klasifikasi terkait emosi (bahagia, sedih, pengakuan, kaget, dan lain sebagainya) berdasarkan kalimat
yang diberikan dengan terlebih dahulu melabeli setiap kelas emosi yang terdapat pada dataset yang digunakan dan akan didapatkan top 5 emosi multilabel yang paling dominan.

