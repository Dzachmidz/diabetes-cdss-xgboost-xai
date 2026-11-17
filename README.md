# CDSS XGBoost + XAI: Deteksi Dini Risiko Diabetes

Repositori ini berisi implementasi **Clinical Decision Support System (CDSS)** berbasis machine learning (**XGBoost**) yang dilengkapi dengan **Explainable AI (XAI)** menggunakan SHAP untuk deteksi dini risiko penyakit diabetes.

Proyek ini dikembangkan untuk tugas mata kuliah **Kecerdasan Artifisial - Magister**.

---

## Struktur Repositori

```text
├── data/                                                # Dataset diabetes
│   ├── BRFSS2015_Diabetes_Binary_NoPrediabetes.csv
│   ├── diabetes_binary_5050split_health_indicators_BRFSS2015.csv
│   ├── diabetes_dataset__2019.csv
│   └── pima_indians_diabetes.csv
├── docs/                                                # Laporan & dokumentasi proyek
│   └── CDSS XGBoost + XAI Deteksi Dini Risiko Diabetes – Kelompok 2.pdf
├── Models.ipynb                                         # Notebook eksplorasi data, pemodelan, dan analisis XAI
├── .gitignore
└── README.md
```

---

## Dataset yang Digunakan
1. **BRFSS 2015 (Behavioral Risk Factor Surveillance System)** - CDC
2. **Pima Indians Diabetes Database** - National Institute of Diabetes and Digestive and Kidney Diseases
3. **Diabetes Dataset 2019**

---

## 🛠️ Metodologi & Fitur Utama
* **Data Auditing & Preprocessing:** Penanganan nilai hilang, duplikat, dan nilai non-fisiologis.
* **Klasifikasi Risiko:** Menggunakan algoritma **XGBoost Classifier** dan perbandingan dengan baseline model lainnya.
* **Explainability (XAI):** Interpretasi model global dan lokal (misal: analisis fitur dominan terhadap risiko diabetes) menggunakan **SHAP**.
* **Validasi & Evaluasi:** Pengujian sensitivitas protokol, bootstrap paired differences, dan evaluasi metrik klasifikasi.

---

## Cara Menjalankan
1. Clone repositori ini:
   ```bash
   git clone <URL_REPO_GITHUB_KAMU>
   cd <NAMA_FOLDER>
   ```
2. Pastikan dependensi terpasang (disarankan menggunakan virtual environment):
   ```bash
   pip install numpy pandas scikit-learn xgboost shap matplotlib seaborn jupyter
   ```
3. Buka notebook:
   ```bash
   jupyter notebook Models.ipynb
   ```
   *(Notebook sudah otomatis mengenali file dataset yang berada di dalam folder `data/`).*
