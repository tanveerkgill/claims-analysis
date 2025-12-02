# Healthcare Claims Analysis – May 2024

This project analyzes a sample of prospective hospital claims from **May 2024** at Stony Brook University Hospital.  
The goal of this work is to identify billing patterns, common clinical conditions, and payer trends by linking claim-level, line-level, and diagnosis-level information.

The analysis supports operational needs in:
- Revenue cycle management  
- Coding accuracy and documentation improvement  
- Compliance auditing  
- Payer and reimbursement evaluation  

---

## Data Overview

This project uses **three relational CSV files**:

- **HEADER** – claim-level provider, payer, and service date information  
- **LINE** – procedure-level details (HCPCS/CPT codes, units, charges)  
- **CODE** – diagnosis codes (ICD-10)  

---

## How to Run

1. Clone or download this repository  
2. Place the three CSV files inside the `data/` folder  
3. Open the notebook in Jupyter or Google Colab  
4. Run all cells from top to bottom to reproduce the analysis  

---

## Key Findings 

- The dataset shows clear differences in clinical complexity across providers.  
- **New York Spine and Brain Surgery** submitted the most complex claims, averaging **9.23 diagnosis codes per claim**.  
- **SB Internists** had the second-highest complexity, averaging **3.59 diagnosis codes per claim**.  
- **Medicare** was the dominant payer, leading both in total claim count and total billed charges.  
- The most frequently assigned diagnosis was **J96.01 – Acute respiratory failure with hypoxia**, indicating a high volume of severe respiratory cases.  
- **Inpatient services** represented **59.54%** of all claims, showing a strong focus on hospital-based care.  
- **Doctor’s office visits** made up **34.02%** of claims, reflecting significant outpatient activity as well.  
- The most commonly billed procedure code was **99291**, corresponding to **30–74 minutes of critical care services**.  
- Overall, the findings highlight patterns in billing behavior, case severity, payer distribution, and service utilization across the May 2024 claim sample.


---

## Required Libraries

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
