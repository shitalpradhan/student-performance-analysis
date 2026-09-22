# Student Performance Analysis and Academic Insights

A Data Analytics internship project exploring factors associated with students'
final grades using a dataset of 395 secondary-school students from two Portuguese
schools.

---

## Project Description

This project analyses the `student_data.csv` dataset, which contains demographic,
family, academic, lifestyle, and health-related information about students. The
target variable is **G3** — the student's final grade on a 0–20 scale.

The analysis follows a four-level framework:
- **Observations** — factual statements directly supported by the data
- **Insights** — meaningful patterns derived from observations
- **Hypotheses** — plausible, testable explanations for insights
- **Recommendations** — practical actions grounded in evidence

A machine learning model (Random Forest Regressor) is also built as an
early-warning tool using only pre-year background information, with G1 and G2
explicitly excluded to avoid target leakage.

---

## Dataset

- **File:** `student_data.csv` (not modified at any point)
- **Rows:** 395 students
- **Columns:** 33 variables (demographic, academic, family, lifestyle, health)
- **Target:** `G3` — final grade (0–20)
- **Source:** Obtained from Kaggle —
  [Student Performance Data](https://www.kaggle.com/datasets/devansodariya/student-performance-data)

> The original dataset is preserved unchanged throughout the project.

---

## Setup

1. **Clone or download** this project folder.
2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Launch the notebook:**
   ```bash
   jupyter notebook student_performance_analysis.ipynb
   ```
   or
   ```bash
   jupyter lab student_performance_analysis.ipynb
   ```
4. **Run all cells** from top to bottom (Kernel → Restart & Run All).

> Python 3.10 or higher is recommended.

---

## Project Structure

| File / Folder | Purpose |
|---|---|
| `student_data.csv` | Original dataset (read-only) |
| `student_performance_analysis.ipynb` | Main analysis notebook |
| `requirements.txt` | Reproducible environment specification |
| `README.md` | Project overview and setup guide (this file) |
| `report.md` | Written project report |
| `figures/` | Chart PNGs saved by the notebook |
| `student-performance-plan.md` | Approved project plan |

---

## How to Read the Results

- Run the notebook to reproduce all statistics, charts, and model evaluations.
- Read `report.md` for the written narrative of findings and recommendations.
- Charts are saved automatically to the `figures/` folder during the notebook run.

---

## Notes

- All statistics and model results are calculated directly from the dataset.
  No findings are assumed or invented.
- G1 (first period grade) and G2 (second period grade) are excluded from the
  machine learning model to avoid target leakage — see Section 4 of the
  notebook for the full explanation.
- G3 = 0 is treated as an observed data pattern. Its cause is not documented
  in the dataset and is not assumed in this project.
