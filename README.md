# 🧠 Mental Health in Tech Industry — Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green?style=flat)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat)

> An end-to-end Exploratory Data Analysis of the **OSMI Mental Health in Tech Survey (2014)** — uncovering patterns in treatment-seeking behavior, workplace culture, and mental health policy effectiveness across the global tech industry.

---

## 📌 Project Overview

Mental health disorders are increasingly prevalent in the tech industry, yet stigma and lack of workplace support prevent many employees from seeking help. This project analyzes survey responses from **1,259 tech employees** across **27 variables** to surface actionable insights for organizations.

**Type:** EDA (Exploratory Data Analysis)  
**Dataset:** [OSMI Mental Health in Tech Survey](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey)  
**Tools:** Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

---

## 🎯 Business Objective

Help tech companies understand the mental health landscape of their workforce so they can:
- Design effective mental health benefit programs
- Build a psychologically safe workplace culture
- Reduce stigma and increase treatment uptake
- Benchmark their policies against industry norms

---

## 📁 Project Structure

```
mental-health-eda/
│
├── Mental_Health_EDA_Solved.ipynb   # Main notebook with full EDA
├── survey.csv                        # Dataset (place in same directory)
└── README.md                         # Project documentation
```

---

## 📊 Dataset Description

| Column | Description |
|---|---|
| `Age` | Respondent's age |
| `Gender` | Self-reported gender |
| `Country` | Country of residence |
| `family_history` | Family history of mental illness |
| `treatment` | **Target** — Has sought mental health treatment |
| `work_interfere` | How often mental health interferes with work |
| `no_employees` | Company size |
| `remote_work` | Works remotely > 50% of time |
| `benefits` | Employer provides mental health benefits |
| `anonymity` | Anonymity protected when using mental health resources |
| `leave` | Ease of taking medical leave for mental health |
| `mental_health_consequence` | Fear of negative consequence for mental health disclosure |
| `coworkers` | Comfort discussing mental health with coworkers |
| `supervisor` | Comfort discussing mental health with supervisor |
| `obs_consequence` | Has witnessed negative consequences for mental health disclosure |

*27 columns total — see notebook for full description.*

---

## 🔍 Key Findings

| Finding | Insight |
|---|---|
| **50.7%** of respondents sought treatment | Mental health issues are widespread in tech |
| **Family history** is the #1 predictor | 76% with family history sought treatment vs. 34% without |
| **Gender gap** exists | Female employees seek treatment at ~75% vs. ~44% for males |
| **Work interference** is a strong signal | 88% of 'Often' group sought treatment vs. 18% of 'Never' group |
| **Anonymity matters** | Protected anonymity raises treatment rates by ~14 percentage points |
| **Awareness gap** | Many employees don't know their company's mental health benefits |

---

## 📈 Charts Included (15 Visualizations)

1. Treatment Rate — Pie Chart + by Gender
2. Age Distribution by Treatment (KDE)
3. Family History vs Treatment Rate
4. Work Interference vs Treatment (Ordinal Trend)
5. Company Size vs Treatment Rate
6. Benefits Availability vs Treatment
7. Anonymity Protection vs Treatment
8. Remote Work vs Treatment
9. Coworker & Supervisor Comfort vs Treatment
10. Top 10 Countries by Respondents
11. Fear of Mental Health Consequences vs Treatment
12. Ease of Leave Distribution
13. Observed Consequences vs Treatment
14. Correlation Heatmap
15. Pair Plot (Age & Work Interference by Gender)

---

## 🛠️ Data Wrangling Summary

- **Dropped** `comments` (86.9% missing) and `Timestamp` (not analytically useful)
- **Cleaned `Age`** — removed outliers outside the range [18, 75]
- **Standardized `Gender`** — mapped 49 inconsistent entries → Male / Female / Other
- **Imputed missing values** in `state`, `self_employed`, and `work_interfere`

---

## 💡 Business Recommendations

1. **Communicate benefits clearly** — many employees don't know what's available
2. **Guarantee anonymity** — it has a measurable positive impact on help-seeking
3. **Train managers** — supervisors have the greatest influence on psychological safety
4. **Target high-risk groups** — employees with family history and high work interference
5. **Simplify leave processes** — remove bureaucratic barriers and publish policies
6. **Close the gender gap** — run awareness campaigns specifically for male employees
7. **Support small companies** — leverage third-party EAP programs for smaller teams

---

## ⚙️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/mental-health-eda.git
   cd mental-health-eda
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch the notebook**
   ```bash
   jupyter notebook Mental_Health_EDA_Solved.ipynb
   ```

4. **Run all cells** — the notebook is designed to execute end-to-end without errors.

> ⚠️ Make sure `survey.csv` is in the same directory as the notebook before running.

---

## 📦 Requirements

```
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- Dataset sourced from [OSMI (Open Sourcing Mental Illness)](https://osmihelp.org/)
- Available on [Kaggle](https://www.kaggle.com/datasets/osmi/mental-health-in-tech-survey)
