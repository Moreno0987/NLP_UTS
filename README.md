#  Prediksi Harga Rumah Menggunakan Machine Learning

## Deskripsi Proyek

Proyek ini bertujuan untuk membangun model Machine Learning dalam memprediksi harga rumah berdasarkan beberapa fitur seperti luas bangunan, jumlah kamar, jumlah kamar mandi, lokasi, dan tahun pembangunan.

Pendekatan yang digunakan adalah **Linear Regression**, baik dalam bentuk:

* Simple Linear Regression (1 fitur)
* Multiple Linear Regression (multi fitur)

Tujuan utama dari proyek ini adalah untuk memahami bagaimana berbagai faktor mempengaruhi harga rumah serta membandingkan performa dua jenis model regresi.

---

## Dataset

Dataset yang digunakan merupakan dataset publik dari Kaggle yang berisi informasi terkait properti rumah, dengan total **50.000 data**.

## Link Dataset

https://www.kaggle.com/datasets/muhammadbinimran/housing-price-prediction-data

### Fitur dalam dataset:

* `SquareFeet` → Luas bangunan
* `Bedrooms` → Jumlah kamar tidur
* `Bathrooms` → Jumlah kamar mandi
* `Neighborhood` → Lokasi (Suburb, Urban, Rural)
* `YearBuilt` → Tahun pembangunan
* `Price` → Harga rumah (target)

---

##  Tahapan Proyek

### 1. Exploratory Data Analysis (EDA)

* Statistik deskriptif
* Visualisasi distribusi harga
* Deteksi outlier
* Analisis korelasi antar fitur

### 2. Data Preprocessing

* Pengecekan missing value
* Encoding variabel kategorikal (One-Hot Encoding)
* Feature scaling menggunakan StandardScaler

### 3. Feature Engineering

* Penambahan fitur baru: `age` (umur bangunan)

### 4. Modeling

* Simple Linear Regression (menggunakan `SquareFeet`)
* Multiple Linear Regression (menggunakan semua fitur)

### 5. Evaluasi Model

Model dievaluasi menggunakan:

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* R² Score

### 6. Visualisasi

* Heatmap korelasi
* Scatter plot (Actual vs Predicted)
* Residual plot

---

## Hasil dan Analisis

* Model **Multiple Linear Regression** menunjukkan performa yang lebih baik dibandingkan Simple Linear Regression.
* Hal ini karena model mempertimbangkan lebih banyak variabel yang mempengaruhi harga rumah.
* Residual plot menunjukkan bahwa error tersebar cukup acak, yang menandakan model cukup sesuai dengan asumsi regresi linear.
* Namun, masih terdapat error yang cukup besar sehingga model belum sepenuhnya optimal.

---

##  Cara Menjalankan Proyek

1. Clone repository:

```
git clone git@github.com:Moreno0987/NLP_UTS.git
```

2. Masuk ke folder project:

```
cd housing-price-ml
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Jalankan Jupyter Notebook:

```
jupyter notebook
```

---

## Dependencies

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

---

## Kesimpulan

Model Machine Learning yang dibangun mampu memprediksi harga rumah dengan cukup baik, terutama dengan pendekatan Multiple Linear Regression.
Fitur seperti luas bangunan, lokasi, dan jumlah kamar memiliki pengaruh terhadap harga rumah.

Untuk pengembangan lebih lanjut, model dapat ditingkatkan dengan:

* menambahkan fitur yang lebih kompleks
* menggunakan algoritma lain yang lebih powerful
* melakukan hyperparameter tuning

---

## Referensi

* Kaggle Dataset
* Scikit-learn Documentation
* Pandas Documentation

---

## Author

Nama: [EXELDUS MORENO_2301020074]
Program Studi: Teknik Informatika
