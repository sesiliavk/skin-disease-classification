# Skin Disease Classification Using Deep Learning-Based Computer Vision

## Repository Outline
1. README.md: Berisi gambaran umum dan penjelasan proyek.
2. Sesilia_Virdha.ipynb: Notebook utama yang berisi seluruh kode untuk tahapan deep learning, mulai dari pra-pemrosesan data, eksplorasi data, pelatihan model, evaluasi, hingga pemilihan model terbaik.
3. Sesilia_Virdha_inference.ipynb: File notebook untuk menjalankan inference atau prediksi menggunakan model terbaik yang telah dilatih.
4. Deployment/: Folder yang berisi semua file yang diperlukan untuk proses deployment model (misalnya app.py untuk aplikasi web, requirements.txt untuk dependensi, dll.).
5. url.txt: Berisi link dataset, deployment, dan model

## Problem Background
Penyakit kulit merupakan salah satu masalah kesehatan yang umum terjadi di berbagai lapisan masyarakat. Beberapa jenis penyakit kulit seperti Acne, Eczema, Basal Cell Carcinoma, Rosacea, dan Actinic Keratosis dapat memengaruhi kualitas hidup seseorang, baik dari segi kesehatan maupun aspek psikososial. Deteksi dini dan klasifikasi yang akurat terhadap penyakit kulit sangat penting untuk memastikan penanganan yang tepat dan efektif.

Namun, akses terhadap dokter spesialis kulit yang berpengalaman tidak selalu mudah dan merata, terutama di daerah terpencil atau bagi mereka yang memiliki keterbatasan waktu dan biaya. Oleh karena itu, teknologi berbasis kecerdasan buatan, khususnya computer vision dan deep learning, dapat menjadi solusi inovatif untuk membantu diagnosis dini dan mandiri.

## Project Output
Proyek ini bertujuan untuk membangun sebuah model computer vision berbasis deep learning yang dapat digunakan untuk mengklasifikasikan gambar wajah berdasarkan lima jenis penyakit kulit seperti Acne, Eczema, Basal Cell Carcinoma, Rosacea, dan Actinic Keratosis. Dengan model ini, diharapkan masyarakat dapat melakukan pemeriksaan awal secara mandiri, sehingga mempercepat proses identifikasi penyakit dan mendukung langkah medis lebih lanjut.

## Data
Data yang digunakan dalam proyek ini memiliki 5 kelas yang akan menjadi kategori penyakit kulit wajah (Acne, Actinic Keratosis, Basal Cell Carcinoma, Eczema, dan Rosacea). Dataset ini terbagi menjadi dua subset, yaitu training dan testing. Sekitar 2.394 gambar, dengan distribusi seimbang, masing-masing kategori memiliki sekitar 399–400 gambar. Gambar berformat JPEG dengan resolusi bervariasi, menampilkan kondisi kulit pada area wajah.

## Method
Proyek ini menerapkan pendekatan deep learning untuk mengklasifikasikan gambar wajah ke dalam lima kategori penyakit kulit: Acne, Eczema, Basal Cell Carcinoma, Rosacea, dan Actinic Keratosis. Metode yang digunakan meliputi preprocessing, augmentasi data, pemodelan baseline, dan peningkatan performa melalui transfer learning.
Dua model digunakan untuk dibandingkan:
1. Artificial Neural Network (ANN): Model baseline dibangun menggunakan arsitektur Sequential dengan beberapa lapisan Dense dan Dropout, serta output layer softmax untuk klasifikasi multi-kelas. Model ini dilatih dari awal dengan data yang telah di-preprocess.
2. DenseNet121 (Transfer Learning): Sebagai upaya peningkatan performa, proyek ini juga menerapkan transfer learning menggunakan arsitektur CNN pretrained DenseNet121. Layer feature extraction dari DenseNet121 digunakan sebagai dasar, kemudian ditambahkan beberapa Dense layer untuk klasifikasi. Proses fine-tuning dilakukan pada beberapa layer akhir untuk meningkatkan akurasi prediksi.

Model terbaik dipilih berdasarkan evaluasi performa menggunakan metrik Akurasi

## Stacks
1. bahasa pemrograman: python
2. tools: visual studio code, hugging face, kaggle
3. library: pandas, numpy, matplotlib, seaborn, Scikit-learn, Tensorflow, Keras, Streamlit

## Reference
dataset = https://www.kaggle.com/datasets/amellia/face-skin-disease

deployment = https://huggingface.co/spaces/sesiliavk/cv_gc7

Model = https://drive.google.com/file/d/1VtDJkqyVqSXwsT_hOB3H5BmHGy1O8E5v/view?usp=sharing
