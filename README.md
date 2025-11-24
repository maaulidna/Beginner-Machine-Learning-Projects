# Proyek Machine Learning Pemula

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Repositori ini berisi submission akhir untuk kursus **Belajar Machine Learning untuk Pemula** dari Dicoding. Proyek ini mengimplementasikan dua pendekatan machine learning: **Clustering** dan **Klasifikasi**.

## 📚 Daftar Isi

- [Tentang Proyek](#tentang-proyek)
- [Struktur Proyek](#struktur-proyek)
- [Dataset](#dataset)
- [Teknologi yang Digunakan](#teknologi-yang-digunakan)
- [Instalasi](#instalasi)
- [Cara Menggunakan](#cara-menggunakan)
- [Hasil dan Analisis](#hasil-dan-analisis)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)
- [Kontak](#kontak)

## 🎯 Tentang Proyek

Proyek ini merupakan implementasi dua teknik machine learning fundamental:

### 1. **Clustering (Unsupervised Learning)**
Menggunakan algoritma clustering untuk mengelompokkan data tanpa label. Teknik ini berguna untuk:
- Segmentasi pelanggan
- Analisis pola data
- Deteksi anomali
- Eksplorasi data

### 2. **Klasifikasi (Supervised Learning)**
Menggunakan algoritma klasifikasi untuk memprediksi kategori atau kelas dari data berdasarkan fitur-fitur yang ada. Teknik ini berguna untuk:
- Prediksi kategori
- Pengambilan keputusan otomatis
- Pattern recognition
- Analisis prediktif

## 📁 Struktur Proyek

```
proyek-machine-learning-pemula/
│
├── README.md
│   └── Dokumentasi proyek
│
├── [Clustering]_Submission_Akhir_BMLP_MC009d5X2352 (2).ipynb
│   └── Notebook utama untuk analisis clustering
│
├── [Klasifikasi]_Submission_Akhir_BMLP_MC009D5X2352 (4).ipynb
│   └── Notebook utama untuk analisis klasifikasi
│
├── Clustering/
│   ├── data_clustering (2).csv
│   │   └── Dataset untuk clustering
│   ├── data_clustering_inverse (6).csv
│   │   └── Dataset hasil inverse transform
│   ├── model_clustering (2).h5
│   │   └── Model clustering yang tersimpan
│   └── PCA_model_clustering (1).h5
│       └── Model PCA untuk dimensionality reduction
│
└── Klasifikasi/
    ├── decision_tree_model (2).h5
    │   └── Model Decision Tree
    ├── explore_LogisticRegression_classification (2).h5
    │   └── Model Logistic Regression
    └── tuning_classification (3).h5
        └── Model hasil hyperparameter tuning
```

## 📊 Dataset

Proyek ini menggunakan dataset yang sesuai dengan kebutuhan masing-masing teknik:

### Clustering
- `data_clustering (2).csv` - Dataset utama untuk analisis clustering
- `data_clustering_inverse (6).csv` - Dataset hasil inverse transformation dari proses normalisasi

### Klasifikasi
- Dataset untuk klasifikasi (embedded dalam notebook atau diunduh otomatis)

> **Catatan**: Dataset clustering sudah tersedia dalam repository. Pastikan path dataset sesuai saat menjalankan notebook.

## 🛠️ Teknologi yang Digunakan

### Bahasa Pemrograman
- Python 3.8+

### Libraries
- **Data Processing**:
  - NumPy
  - Pandas
  
- **Visualization**:
  - Matplotlib
  - Seaborn
  
- **Machine Learning**:
  - Scikit-learn
  - TensorFlow/Keras (untuk save/load model .h5)
  
- **Development**:
  - Jupyter Notebook

## 🚀 Instalasi

### 1. Clone Repository

```bash
git clone https://github.com/maaulidna/proyek-machine-learning-pemula.git
cd proyek-machine-learning-pemula
```

### 2. Buat Virtual Environment (Opsional tapi Disarankan)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/Mac
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter tensorflow
```

> **Catatan**: TensorFlow/Keras diperlukan untuk loading model .h5

Atau jika ada file requirements.txt:

```bash
pip install -r requirements.txt
```

## 💻 Cara Menggunakan

### Menjalankan Notebook

1. Buka Jupyter Notebook:
```bash
jupyter notebook
```

2. Pilih notebook yang ingin dijalankan:
   - `[Clustering]_Submission_Akhir_BMLP_MC009d5X2352 (2).ipynb` untuk analisis clustering
   - `[Klasifikasi]_Submission_Akhir_BMLP_MC009D5X2352 (4).ipynb` untuk analisis klasifikasi

3. Jalankan cell secara berurutan (Shift + Enter)

### Workflow Umum

#### Untuk Clustering:
1. **Data Loading**: Import dan load dataset
2. **Exploratory Data Analysis (EDA)**: Analisis dan visualisasi data
3. **Data Preprocessing**: Cleaning, normalisasi, dan transformasi
4. **Clustering**: Implementasi algoritma (K-Means, DBSCAN, dll.)
5. **Evaluation**: Evaluasi menggunakan metrik seperti Silhouette Score, Elbow Method
6. **Visualization**: Visualisasi cluster hasil

#### Untuk Klasifikasi:
1. **Data Loading**: Import dan load dataset
2. **Exploratory Data Analysis (EDA)**: Analisis distribusi kelas dan fitur
3. **Data Preprocessing**: Feature engineering, encoding, scaling
4. **Train-Test Split**: Pembagian data training dan testing
5. **Model Training**: Training model klasifikasi
6. **Evaluation**: Evaluasi menggunakan accuracy, precision, recall, F1-score
7. **Prediction**: Prediksi pada data baru

## 📈 Hasil dan Analisis

### Clustering
Proyek clustering mengimplementasikan berbagai teknik:

- **Dimensionality Reduction**: Menggunakan PCA (Principal Component Analysis)
  - Model: `PCA_model_clustering (1).h5`
  - Tujuan: Mengurangi dimensi fitur untuk visualisasi dan efisiensi komputasi

- **Model Clustering**: 
  - Model tersimpan: `model_clustering (2).h5`
  - Menghasilkan pengelompokan data berdasarkan pola yang ditemukan
  
- **Dataset Output**:
  - `data_clustering_inverse (6).csv` - Data hasil inverse transform untuk interpretasi

### Klasifikasi
Proyek klasifikasi mengeksplorasi beberapa algoritma:

- **Decision Tree**:
  - Model: `decision_tree_model (2).h5`
  - Algoritma tree-based untuk klasifikasi

- **Logistic Regression**:
  - Model: `explore_LogisticRegression_classification (2).h5`
  - Algoritma klasifikasi linear

- **Hyperparameter Tuning**:
  - Model: `tuning_classification (3).h5`
  - Model hasil optimasi hyperparameter untuk performa terbaik

> **Catatan**: Semua model disimpan dalam format .h5 untuk kemudahan deployment dan reusability.

## 🤝 Kontribusi

Kontribusi, issues, dan feature requests sangat diterima! Jangan ragu untuk check [issues page](https://github.com/maaulidna/proyek-machine-learning-pemula/issues).

### Cara Berkontribusi:

1. Fork repositori ini
2. Buat branch baru (`git checkout -b feature/AmazingFeature`)
3. Commit perubahan (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📝 Lisensi

Proyek ini dilisensikan di bawah MIT License - lihat file [LICENSE](LICENSE) untuk detail.

## 👤 Kontak

**Maulidna**

- GitHub: [@maaulidna](https://github.com/maaulidna)
- Project Link: [https://github.com/maaulidna/proyek-machine-learning-pemula](https://github.com/maaulidna/proyek-machine-learning-pemula)

## 🙏 Acknowledgments

- [Dicoding Indonesia](https://www.dicoding.com/) - Platform pembelajaran
- [Scikit-learn Documentation](https://scikit-learn.org/) - Referensi algoritma ML
- Semua kontributor yang telah membantu proyek ini

---

⭐ Jangan lupa berikan star jika proyek ini membantu Anda!

**#MachineLearning #Python #DataScience #Dicoding**
