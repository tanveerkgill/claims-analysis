# Healthcare Claims Analysis

This project analyzes a sample of prospective **May 2024 hospital claims** from **Stony Brook University Hospital** to understand billing patterns, common clinical conditions, and payer relationships that drive revenue and compliance performance. Using three relational claims files (HEADER, LINE, CODE), the analysis links claim-level, line-level, and diagnosis-level detail to generate actionable insights for the compliance and revenue cycle teams.

The work focuses on:

- Provider billing patterns and claim volume
- Payer mix and contribution to total charges
- Most frequent diagnoses (ICD-10)
- Most frequent procedures (HCPCS/CPT)
- Place of service utilization (e.g., inpatient vs doctor’s office)
- High-complexity claims and diagnosis–procedure combinations

---

## Project Structure

```text
claims-analysis/
│
├── .venv/                     # local Python environment (ignored by Git)
│
├── data/                      # CSV files stored locally (not in repo)
│   ├── STONYBRK_20240531_HEADER.csv
│   ├── STONYBRK_20240531_LINE.csv
│   └── STONYBRK_20240531_CODE.csv
│
├── notebooks/
│   └── claims_analysis.ipynb  # main Google Colab / Jupyter notebook
│
├── requirements.txt
├── .gitignore
└── README.md
