# 🩺 CKD Statistical Analysis

**A complete descriptive statistics project on the Chronic Kidney Disease dataset.**  
Built as a weekly study project covering NumPy, Matplotlib, Seaborn, and statistical fundamentals.

---

## 📖 About the Dataset

| Property | Value |
|---|---|
| File | `CKD_dataset.csv` |
| Rows | 4,800 patients |
| Columns | 36 clinical features |
| Target | 5 CKD stages (Healthy → Kidney Failure) |

**CKD Stages:**
- 🟢 Healthy Kidney
- 🔵 Mild CKD (Stage 1–2)
- 🟡 Moderate CKD (Stage 3)
- 🔴 Severe CKD (Stage 4)
- 🟣 Kidney Failure (Stage 5)

---

## 🧠 Topics Covered

| # | Topic | Technique |
|---|---|---|
| 1 | NumPy Basics | `np.array`, `np.mean`, `np.std`, `np.median`, `np.min`, `np.max` |
| 2 | Line Plot | Age profile with mean & median reference lines |
| 3 | Descriptive Statistics | Mean, Median, Mode per feature |
| 4 | Bar Chart | Mean vs Median comparison |
| 5 | Scatter Plot | Age vs eGFR colored by CKD stage + trend line |
| 6 | Variance & Std Dev | `np.var`, `np.std` with bar visualization |
| 7 | Error Band Line Plot | Mean ± Std Dev per stage (`errorbar`) |
| 8 | Histogram | Age frequency distribution |
| 9 | KDE Plot | eGFR density curves by CKD stage |
| 10 | Histogram + KDE Overlay | 4-panel grid for key features |
| 11 | Percentile & IQR | Q1, Q3, fences, outlier detection |
| 12 | Boxplot | Z-normalized features + eGFR per stage |
| 13 | Pandas GroupBy | Multi-stat aggregation by stage |
| 14 | Heatmap | Cross-stage clinical feature comparison |

---

## 📁 Project Structure

```
CKD-Statistical-Analysis/
│
├── CKD_Statistical_Analysis.ipynb   ← Main notebook (all analysis)
├── CKD_dataset.csv                  ← Dataset
├── README.md                        ← This file
│
└── plots/
    ├── 01_line_age_profile.png
    ├── 02_bar_mean_median.png
    ├── 03_scatter_age_egfr.png
    ├── 04_bar_std_dev.png
    ├── 05_line_egfr_std.png
    ├── 06_hist_age.png
    ├── 07_kde_egfr_stage.png
    ├── 08_histkde_four_features.png
    ├── 09_boxplot_all_features.png
    ├── 10_boxplot_egfr_stage.png
    └── 11_heatmap_stage_features.png
```

---

## 🚀 How to Run

### Option 1: Jupyter Notebook
```bash
pip install numpy pandas matplotlib seaborn scipy jupyter
jupyter notebook CKD_Statistical_Analysis.ipynb
```

### Option 2: JupyterLab
```bash
pip install jupyterlab
jupyter lab CKD_Statistical_Analysis.ipynb
```

---

## 📊 Key Findings

- **eGFR** (kidney filtration rate) decreases significantly as CKD stage worsens — from ~75 in healthy patients to ~8 in kidney failure
- **Age** shows a moderate negative correlation with eGFR (r ≈ −0.3), meaning older patients tend to have lower kidney function
- **Serum Creatinine** is the highest-variance feature, making it a strong clinical indicator
- Boxplots reveal clear separation between stages for eGFR, with minimal overlap between Healthy and Stage 4–5

---

## 🛠️ Requirements

```
numpy
pandas
matplotlib
seaborn
scipy
jupyter
```

---

## 👤 Author

**Akmal** — Data Analytics self-study project  
*Tools: Python · NumPy · Pandas · Matplotlib · Seaborn*
