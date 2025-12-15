# Boston Marathon Cutoff Prediction & Uncertainty Quantification

**Authors:** Jackson Murray, Kasey Osborne, Zachary Parente, John Pawsat, Abigail Vollrath

---

## Project Overview

This project analyzes Boston Marathon qualifying data to **predict cutoff times**
and **quantify uncertainty** in future acceptance thresholds. Using historical
qualifier distributions and applicant behavior, we model cutoff dynamics for the
**2025 and 2026 Boston Marathons**, emphasizing probabilistic inference and
transparent uncertainty bounds rather than single point estimates.

---

## Repository Contents

### Data Files
- **`Boston_Marathon_2025_Qualifiers.csv`**  
  Cleaned and harmonized qualifying performances for runners eligible for the
  2025 Boston Marathon.

- **`Boston_Marathon_2026_Qualifiers.csv`**  
  Cleaned and harmonized qualifying performances for runners eligible for the
  2026 Boston Marathon, structured consistently with the 2025 dataset.

### Analysis Notebook
- **`Boston_Marathon_Cutoff_Prediction_and_Uncertainty_Quantification.ipynb`**  
  Primary analysis notebook containing:
  - Data cleaning and standardization across years  
  - Exploratory analysis of qualifier and buffer-time distributions by age group  
  - Cutoff time prediction models  
  - Simulation-based uncertainty quantification  
  - Visualizations of projected cutoff distributions and confidence intervals  

---

## Methodology (High-Level)

1. **Data Preparation**  
   Standardized age-group definitions, removed invalid or unknown categories, and
   aligned datasets to ensure year-over-year comparability.

2. **Exploratory Analysis**  
   Examined buffer-time distributions, applicant density near historical cutoffs,
   and structural differences across age groups.

3. **Cutoff Prediction**  
   Modeled expected cutoff times using distributional and simulation-based
   approaches rather than deterministic thresholds.

4. **Uncertainty Quantification**  
   Constructed confidence intervals around predicted cutoffs to reflect
   uncertainty in applicant volume, tail behavior, and year-to-year variation.

---

## Data Sources and Attribution

Raw qualifying data used to construct the 2025 and 2026 Boston Marathon datasets
was originally sourced from a publicly available Kaggle repository compiled by
**Brian Rock**.

The raw Kaggle files are **not included** in this repository. All data cleaning,
harmonization, and feature engineering steps used to generate the final analysis
datasets are fully documented in the accompanying Jupyter notebook. Any errors or
interpretations in this repository are the responsibility of the authors.

---

## How to Run

1. Clone the repository.
2. Create a Python environment with:
   - `pandas`
   - `numpy`
   - `matplotlib`
3. Open and run the notebook:
   ```bash
   Boston_Marathon_Cutoff_Prediction_and_Uncertainty_Quantification.ipynb
