# 🏎️ F1 Championship Winner Prediction

A machine learning project that predicts which **team** and **driver** will win the Formula 1 World Championship, using 70+ years of historical race data (1950–2025).

---

## 📌 Project Overview

**Business Problem:** Investors and sponsors need data-driven insights to decide which F1 teams to fund and which drivers to associate with.

**ML Approach:** Multi-class classification — predicting the championship winner (team/driver category) based on historical performance features such as win rate, race momentum, and consistency.

---

## 📂 Project Files

| File | Description |
|------|-------------|
| `F1dataset.csv` | Historical F1 race results dataset (1950–2025) |
| `F1_Championship_Prediction.ipynb` | Full Jupyter Notebook with analysis, modeling & predictions |
| `F1_winning_prediction.pptx` | Presentation summarizing methodology and key findings |

---

## 📊 Dataset

**File:** `F1dataset.csv`  
**Records:** 1,142 race results  
**Time span:** 1950 – 2025  

### Columns

| Column | Description |
|--------|-------------|
| `date` | Race date |
| `continent` | Continent where race was held |
| `grand_prix` | Name of the Grand Prix |
| `circuit` | Circuit name |
| `winner_name` | Winning driver's name |
| `team` | Winning constructor/team |
| `time` | Total race time |
| `laps` | Number of laps completed |
| `year` | Championship season year |

---

## 🔬 Notebook Structure

The notebook (`F1_Championship_Prediction.ipynb`) follows a structured 3-phase ML pipeline:

### Phase 1 — Problem & Data Understanding
- Import libraries (pandas, numpy, matplotlib, seaborn)
- Load and explore the dataset
- Analyze missing values and data types

### Phase 2 — Data Preparation
- Convert date columns to datetime format
- Handle missing values (median imputation for laps)
- Remove duplicate records
- Exploratory Data Analysis (EDA): championship winners by year, team dominance, continent distribution

### Phase 3 — Modeling
- Feature engineering: win rate, momentum score, historical performance metrics
- Train and evaluate multiple classification algorithms (Random Forest, Logistic Regression)
- Select best-performing model based on accuracy
- Generate championship probabilities per team and driver

### Results & Recommendations
- Top 3 teams ranked by predicted championship probability
- Top 3 drivers ranked by recent performance
- Clear investment and sponsorship guidance

---

## 🛠️ Requirements

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/hazem-emam/YOUR-REPO-NAME.git
   cd YOUR-REPO-NAME
   ```

2. Place `F1dataset.csv` in the same directory as the notebook.

3. Open the notebook:
   ```bash
   jupyter notebook F1_Championship_Prediction.ipynb
   ```

4. Run all cells from top to bottom.

> **Google Colab users:** Upload `F1dataset.csv` manually using the file upload cell provided in the notebook.

---

## 📈 Key Findings

- **Most predictive features:** Win count, win rate, and historical championship momentum
- **Dataset coverage:** 6 continents, 70+ years of F1 history
- **Business value:**
  - *Investors* get data-backed team rankings by championship probability
  - *Sponsors* get evidence-based driver shortlists by recent performance

---

## 👤 Author

**Hazem Emam**  
German International University (GIU)  
December 2025
