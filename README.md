# Capstone_Workplace_Project
Final workplace project repository

# Client Activity Segmentation – Workplace Module

**Author:** Katy Sonnekus  
**Affiliation:** ExploreAI (2024)  
**Module:** QCTO Workplace Learning

---

## Project Overview

This project develops an insights-driven client segmentation model for a banking institution. Traditional segmentation based on age and income is enhanced by incorporating behavioral and engagement metrics such as account usage and digital activity. The goal is to support predictive and prescriptive analytics for hyper-personalization and strategic client growth.

---

## Methods Used

### Data Collection
- Transactional data: volume, account count
- Demographics: age, gender, marital status
- Sampling: proportional by province

### Data Cleaning & Feature Engineering
- Missing value imputation (median/mode)
- Outlier removal (IQR method)
- Feature creation:
  - Age groups
  - Income brackets
  - RFM metrics (Recency, Frequency, Monetary)
  - Digital Engagement Score
  - Product Holding Count

### Exploratory Data Analysis (EDA)
- Summary statistics
- Histograms, box plots, correlation matrices

### Clustering & Modeling
- KMeans, Hierarchical, DBSCAN clustering
- PCA and t-SNE for dimensionality reduction
- Cluster profiling and evaluation
- Random Forest classification for segment prediction

---

## Key Outputs

- Cleaned dataset: 79,226 records × 30 features
- Cluster profiles with behavioral and financial traits
- Visualizations: engagement distribution, cluster scatterplots, confusion matrix
- Exported files for Power BI:
  - `kpi_summary.csv`
  - `cluster_sizes.csv`
  - `classification_report.csv`
  - `confusion_matrix.csv`

---

## Usage Instructions

### Requirements
- Python 3.8+
- Jupyter Notebook
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

### Setup
1. Clone this repository.
2. Place `Customer_DataV3.csv` in the working directory.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
### Reproducibility
- Set random seeds (np.random.seed(42), random_state=42) for consistent results.
- All preprocessing and modeling steps are explicitly coded.
- Outputs (figures, tables, metrics) are saved or displayed inline.
