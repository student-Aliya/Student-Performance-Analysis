# Student Performance Analysis — Exploratory Data Analysis (EDA)

A complete exploratory data analysis of a student performance dataset, built with Python, Pandas, and Seaborn. This project examines what factors are associated with academic performance (GPA) across 2,392 students — including study habits, absences, parental support, and demographics.

## 📊 Project Overview

- **Dataset:** 2,392 student records, 15 features (demographics, study habits, parental involvement, extracurriculars, GPA)
- **Goal:** Understand the dataset's structure, clean it, and visualize the relationships that drive GPA
- **Approach:** Univariate distributions → bivariate relationships → multivariate correlation analysis

## 🔑 Key Insights

- **Absences is the dominant factor** — correlation of **−0.92** with GPA, far outweighing any other variable
- **Study time has a weak positive relationship** with GPA (correlation ≈ **0.18**)
- **Parental support and tutoring** show similarly modest positive associations (≈ 0.15–0.19)
- **Demographics barely matter** — Age, Gender, and Ethnicity show negligible correlation with GPA
- The dataset is clean out of the box: **no missing values, no duplicate records**

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Core language |
| Pandas | Data loading, cleaning, summary statistics |
| NumPy | Numerical operations |
| Matplotlib | Base plotting / figure export |
| Seaborn | Statistical visualizations |
| Jupyter Notebook | Interactive analysis environment |

## 📁 Repository Structure

```
Student-Performance-Analysis/
├── notebooks/
│   └── student_performance_analysis.ipynb   # Full EDA notebook
├── data/
│   └── Student_performance_data.csv         # Dataset
├── images/                                  # Exported chart images
│   ├── gpa_histogram.png
│   ├── gpa_boxplot.png
│   ├── gender_countplot.png
│   ├── Studytime_vs_gpa.png
│   ├── correlation_heatmap.png
│   └── pairplot.png
├── reports/
│   └── Student_Performance_EDA_Report python.docx  # Full written report
├── requirements.txt
└── README.md
```

> Note: adjust folder names above if your local layout differs — the notebook saves figures to `../images/`, so keep the notebook one level inside a folder next to `images/`.

## 📈 Visualizations

| Chart | What it shows |
|---|---|
| Histogram + KDE | Distribution of GPA across all students |
| Box Plot | GPA spread and outlier check |
| Count Plot | Gender distribution / class balance |
| Scatter Plot | Study Time Weekly vs GPA |
| Correlation Heatmap | Pairwise correlation across all numeric features |
| Pair Plot | Joint relationships between GPA, Study Time, Absences, and Age |

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd student-performance-eda
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Launch the notebook:
   ```bash
   jupyter notebook notebooks/student_performance_analysis.ipynb
   ```

## 📄 Full Report

A detailed 12-page write-up covering methodology, all visualizations, key findings, and future improvement ideas is available in [`report/Student_Performance_EDA_Report.docx`](report/Student_Performance_EDA_Report.docx).

## 🔮 Future Improvements

- Build a predictive model (regression / tree-based) to estimate GPA and rank feature importance
- Confirm categorical label mappings (Gender, Ethnicity, ParentalEducation, etc.) against a data dictionary
- Add statistical significance testing alongside correlation coefficients
- Deploy an interactive Streamlit dashboard for dynamic exploration

## 👤 Author

**Aliya Batool**
📅 July 2026

---

⭐ If you found this project useful, consider giving it a star!
