# Nigeria's Power Crisis: A Data-Driven Analysis (2023–2024)

A data science capstone project analyzing 731 days of Nigeria's national 
power grid data to uncover generation trends, grid instability, and 
systemic deterioration between January 2023 and December 2024.

---

## Key Findings

- Mean daily generation declined **8.6%** year-over-year (4,019 MWh → 3,674 MWh)
- Grid variability increased **41%**, indicating chronic instability
- Frequency violations occurred on **48.9% of days** in 2024
- Statistical anomalies increased **5.5x** from 2023 to 2024
- The 5 worst generation days in the entire dataset all occurred in **Q4 2024**

---

## Repository Structure
```
├── data/
│   ├── nigeria_power_genertion_raw/                  # Original unmodified dataset
│   └── nigeria_power_generation_clean/                # Preprocessed and cleaned dataset
├── notebooks/
│   ├── Emmanuel_Olafisoye_Data_Cleaning_Notebook_Karatu_2nd_Semester.ipynb   # Data cleaning and preparation
│   └── Emmanuel_Olafisoye_Analysis_Notebook_2nd_Semester_Karatu.ipynb        # Main analysis and visualizations
├── report/
│   ├── Emmanuel_Olafisoye_Proposal_Document_Karatu_Second_Semester.pdf          # Project proposal document
│   └── Emmanuel_Olafisoye_Final_Report_Karatu_Second_Semester.pdf      # Full written report
└── README.md
```
---

## Project Documents

| Document | Description |
|---|---|
| [Project Proposal](report/Emmanuel_Olafisoye_Proposal_Document_Karatu_Second_Semester.pdf) | Research questions, objectives, and methodology plan |
| [Final Report](report/Emmanuel_Olafisoye_Final_Report_Karatu_Second_Semester.pdf) | Complete analysis, findings, and recommendations |

---

## Methodology

| Technique | Purpose |
|---|---|
| Two-sample t-test | Confirm statistical significance of year-over-year decline |
| Cohen's d | Measure practical effect size |
| Linear regression | Quantify monthly trend slopes per year |
| Z-score detection | Identify anomalous generation days |
| Rolling averages | Smooth noise and reveal underlying trends |
| Confidence intervals | Bound the true mean generation per year |

---

## Statistical Summary

| Metric | 2023 | 2024 | Change |
|---|---|---|---|
| Mean Daily Generation | 4,018.6 MWh | 3,674.4 MWh | -8.6% |
| Std Deviation | 451.6 MWh | 580.5 MWh | +28.5% |
| Coefficient of Variation | 11.2% | 15.8% | +41% |
| Frequency Violations | 156 days (42.7%) | 179 days (48.9%) | +23 days |
| Statistical Anomalies | 2 days | 11 days | +5.5x |
| t-statistic | — | 8.9469 | — |
| p-value | — | < 0.000001 | — |
| Cohen's d | — | 0.6618 (large) | — |

---

## Tools & Libraries

- **Python**
- **Pandas** - data manipulation
- **NumPy** - numerical computation
- **SciPy** - statistical testing
- **Matplotlib / Seaborn** - visualizations

---

## How to Run

1. Clone the repository
```bash
git clone https://github.com/korie-cyber/nigeria-power-analysis.git
cd nigeria-power-analysis
```

2. Install dependencies
```bash
pip install pandas numpy scipy matplotlib seaborn jupyter
```

3. Open the notebooks
```bash
jupyter notebook
```

Run `Emmanuel_Olafisoye_Data_Cleaning_Notebook_Karatu_2nd_Semester.ipynb` first, then `Emmanuel_Olafisoye_Analysis_Notebook_2nd_Semester_Karatu.ipynb`.

---

## Report

The full written report is available in the `/report` folder. It covers 
the complete methodology, all 9 visualizations, statistical tests, and 
recommendations for policymakers and infrastructure planners.

---

## Author

**Emmanuel Olafisoye**  
AltSchool Africa - Data Science  
Capstone Project | February 2026
