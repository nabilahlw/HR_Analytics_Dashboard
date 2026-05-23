# 📊 HR Attrition Analysis

Proyek analisis data HR untuk memahami pola **attrition (pengunduran diri karyawan)** menggunakan Python (Pandas, Seaborn, Matplotlib) dan visualisasi interaktif dengan **Power BI**.

## 🎬Tampilan dashboard dengan Power BI:
![Dashboard HR](hr_dashboard.png)

## ✨ Insight yang Dianalisis

- Persentase attrition berdasarkan **Gender & Job Role**
- Hubungan **Work Life Balance** dengan attrition
- Attrition berdasarkan **kelompok usia**
- Top Job Role dengan attrition **tertinggi & terendah**
- Rata-rata **gaji bulanan** per Job Role
- Rata-rata **lama bekerja** berdasarkan Job Role & kepuasan kerja
- Distribusi **jurusan kuliah** vs Job Role

## 🛠️ Teknologi yang Digunakan

| Teknologi | Fungsi |
|-----------|--------|
| Python 3.x | Bahasa pemrograman utama |
| Pandas | Manipulasi & analisis data |
| Seaborn | Visualisasi statistik |
| Matplotlib | Plot & grafik |
| Jupyter Notebook / Google Colab | Environment analisis |
| Power BI | Dashboard interaktif |
| Microsoft Excel (.xlsx) | Sumber data |

## 📁 Struktur File

```
HR-Attrition-Analysis/
├── HR_Attrition_Analystic.ipynb       ← Notebook analisis utama
├── HR_Attrition_Analytics_Dashboard.pbix  ← File Power BI dashboard
├── HR_Statistic.xlsx                  ← Dataset HR
├── HR Attrition Analysis Presentation.pdf  ← Presentasi hasil
├── hr_dashboard.png                   ← Screenshot dashboard
└── README.md
```
---
## ⚙️ Cara Menjalankan — Jupyter Notebook

### Prasyarat

Pastikan sudah terinstall:
- [Python 3.x](https://www.python.org/downloads/)
- pip (sudah include saat install Python)

### Opsi A: Google Colab (Paling Mudah, Tanpa Install)

1. Buka [colab.research.google.com](https://colab.research.google.com)
2. Klik **File → Upload Notebook**
3. Upload file `HR_Attrition_Analystic.ipynb`
4. Upload dataset: klik ikon **folder** di panel kiri → **Upload** → pilih `HR_Statistic.xlsx`
5. Jalankan semua cell: klik **Runtime → Run All**

### Opsi B: Jupyter Notebook Lokal

**Step 1 — Install library yang dibutuhkan**

Buka terminal / command prompt, jalankan:
```bash
pip install pandas openpyxl seaborn matplotlib jupyter
```

**Step 2 — Jalankan Jupyter**
```bash
jupyter notebook
```

Browser akan terbuka otomatis di `http://localhost:8888`

**Step 3 — Buka Notebook**
1. Navigasi ke folder project
2. Klik file `HR_Attrition_Analystic.ipynb`

**Step 4 — Jalankan Notebook**
- Jalankan per cell: tekan **Shift + Enter**
- Jalankan semua sekaligus: klik **Kernel → Restart & Run All**

**Step 5 — Upload Dataset**

Di cell pertama ada kode upload file:
```python
file_name = list(uploaded.keys())[0]
```
Jalankan cell tersebut → akan muncul tombol **Choose File** → pilih `HR_Statistic.xlsx`

### Opsi C: VS Code

1. Install extension **Jupyter** di VS Code
2. Buka folder project di VS Code
3. Buka file `.ipynb`
4. Klik **Run All** di bagian atas

---

## ⚙️ Cara Membuka Dashboard Power BI

### Prasyarat

- Install [Power BI Desktop](https://powerbi.microsoft.com/desktop) 

### Step by Step

**Step 1 — Download & Install Power BI Desktop**
1. Buka [powerbi.microsoft.com/desktop](https://powerbi.microsoft.com/desktop)
2. Klik **Download free** → install seperti biasa

**Step 2 — Buka File Dashboard**
1. Buka Power BI Desktop
2. Klik **File → Open report**
3. Pilih file `HR_Attrition_Analytics_Dashboard.pbix`

**Step 3 — Refresh Data (jika diperlukan)**
1. Klik tab **Home**
2. Klik **Refresh** — pastikan file `HR_Statistic.xlsx` ada di folder yang sama
3. Jika muncul dialog lokasi file → arahkan ke `HR_Statistic.xlsx`

**Step 4 — Eksplorasi Dashboard**

Dashboard memiliki filter interaktif:
- **JobRole** — filter berdasarkan posisi
- **Age Group** — filter berdasarkan kelompok usia

---

## 📊 Alur Analisis

```
HR_Statistic.xlsx (Dataset)
        ↓
Data Loading & Exploration
(df.head(), df.info(), df.describe())
        ↓
Data Cleaning
(hapus kolom tidak perlu, encode kategori, hapus duplikat)
        ↓
Exploratory Data Analysis (EDA)
(crosstab, groupby, value_counts)
        ↓
Visualisasi
(Seaborn & Matplotlib)
        ↓
Dashboard Power BI
(Visualisasi interaktif)
```

---
