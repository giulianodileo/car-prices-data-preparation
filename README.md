# 🚗 Car Price Data Preparation

### Overview
This repository contains a complete preprocessing workflow for a car-price dataset.
The goal is to ensure the data is clean, consistent, and suitable for machine-learning modeling.
All preprocessing steps are implemented in a single, reproducible notebook.

---

### Workflow Summary
The notebook follows a structured approach to data cleaning and preparation:

1. **Duplicate Removal** – eliminate repeated records to prevent data leakage.
2. **Missing Data Treatment** – detect, analyze, and handle missing values through selective imputation.
3. **Outlier Inspection** – visualize distributions to identify unrealistic values before scaling.
4. **Feature Scaling** – normalize numerical features using `RobustScaler` or `StandardScaler` according to their distribution.
5. **Categorical Encoding** – transform text variables into numeric form using:
   - One-Hot Encoding (`aspiration`, `enginelocation`, `enginetype`)
   - Manual Ordinal Encoding (`cylindernumber`)
   - Label Encoding for the target (`price`)
6. **Feature Selection** – apply permutation importance to retain only the most relevant predictors (`curbweight`, `carwidth`).

The notebook concludes with a clean dataset ready for modeling and further analysis.

---

### Repository Structure

car-prices-data-preparation/
│
├── data/
│ ├── raw/ # Original dataset
│ └── processed/ # Cleaned dataset exported from the notebook
│
├── notebooks/
│ └── 01_car_prices_preprocessing.ipynb
│
├── docs/
│ └── dataset_description.md
│
├── requirements.txt
└── README.md


---

### Tools and Libraries
- **Python 3.10+**
- `pandas`, `numpy` – data manipulation
- `matplotlib`, `seaborn` – visualization
- `scikit-learn` – preprocessing, encoding, scaling, modeling
- `statsmodels` – statistical diagnostics

---

### Dataset Notice

The dataset was provided by Le Wagon for educational use.
It is included here solely to demonstrate preprocessing and feature-engineering techniques.
All rights to the original data remain with their respective owners.
