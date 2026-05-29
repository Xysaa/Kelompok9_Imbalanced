# 🧠 Penanganan Imbalanced Dataset pada Prediksi Stroke
**Kelompok 9**

---

## 👥 Anggota Kelompok

| NIM | Nama |
|---|---|
| 123140003 | Muhammad Fadhilah Akbar |
| 123140030 | Annisa Al-Qoriah |
| 123140031 | Muhammad Romadhon Santoso |
| 123140033 | Sigit Kurnia Hartawan |
| 123140038 | Stevanus Cahya Anggara |
| 123140063 | Pradana Figo Ariasya |

---

## 📌 Deskripsi Project

Project ini bertujuan untuk membangun model klasifikasi prediksi **stroke** menggunakan dataset kesehatan, dengan fokus pada penanganan **imbalanced class** (ketidakseimbangan kelas) yang umum terjadi pada dataset medis.

Tiga pendekatan dibandingkan:
| Metode | Deskripsi |
|---|---|
| **Baseline** | Tanpa penanganan imbalanced |
| **SMOTE** | Synthetic Minority Over-sampling Technique |
| **SMOTE-ENN** | Kombinasi SMOTE dengan Edited Nearest Neighbours |

Model yang digunakan: **Random Forest Classifier**

---

## 📂 Struktur Folder

```
Daming/
├── data/
│   └── healthcare-dataset-stroke-data.csv   # Dataset utama
├── docs/
│   └── (laporan, referensi, dll)
├── kelompok9_imbalanced.ipynb               # Notebook utama
└── README.md                                # File ini
```

---

## 🚀 Cara Menjalankan Notebook

### Menggunakan VS Code
1. Install ekstensi **Jupyter** di VS Code (search di Extensions panel)
2. Pastikan Python & library sudah terinstall:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
   ```
3. Buka file `kelompok9_imbalanced.ipynb` di VS Code
4. Pilih kernel Python yang sesuai (pojok kanan atas)
5. Klik **"Run All"** (▶▶) untuk menjalankan semua cell sekaligus

### Menggunakan Jupyter Notebook/Lab
```bash
jupyter notebook kelompok9_imbalanced.ipynb
# atau
jupyter lab
```
Lalu klik **Kernel → Restart & Run All**

---

## 📦 Library yang Dibutuhkan

```
pandas
numpy
matplotlib
seaborn
scikit-learn
imbalanced-learn
```

---

## 📊 Dataset

- **Sumber:** [Kaggle - Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)
- **File:** `data/healthcare-dataset-stroke-data.csv`
- **Jumlah baris:** ~5.110 pasien
- **Target:** `stroke` (0 = tidak stroke, 1 = stroke)

---

## 📈 Metrik Evaluasi

- Accuracy, Precision, Recall, F1-Score, ROC-AUC
- Confusion Matrix per metode
- Visualisasi perbandingan performa antar metode