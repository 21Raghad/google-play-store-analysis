# Google Play Store Apps Data Analysis
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/21Raghad/google-play-store-analysis/blob/main/notebooks/Project_google_Play_Store.ipynb)

## Overview and Research Question
This public repository contains the complete data science workflow for analyzing **Google Play Store Apps** data to examine how app ratings (`Rating`) and installation counts (`Installs`) differ across app categories (`Category`) and pricing types (`Type`: Free vs. Paid).

## Repository Structure
- `data/googleplaystore.csv`: Original raw dataset from Kaggle.
- `data/googleplaystore_cleaned.csv`: Cleaned and prepared dataset after transformation (`Install_Tier`) and aggregation.
- `notebooks/Project_google_Play_Store.ipynb`: Reproducible Google Colab / Jupyter notebook covering data understanding, cleaning, preparation, analysis, three visualizations, interpretations, conclusions, and limitations.

## Dataset Source and Access
- **Dataset:** Google Play Store Apps (`googleplaystore.csv`) from **Kaggle**.
- **Reproducibility:** The notebook checks for a local file first, supports loading from a direct repository raw URL, and falls back to file upload in Google Colab without hard-coded local paths.

## Workflow Summary
1. **Data Understanding:** Inspected dataset shape, column names, data types, missing values, and descriptive statistics.
2. **Data Cleaning and Preparation:** Removed duplicates and invalid entries (`Category == '1.9'`), cleaned numeric symbols (`+`, `,`, `$`), imputed missing `Rating` values using the median, applied transformation (`Install_Tier`) and aggregation (`Category` and `Type`), and saved `googleplaystore_cleaned.csv`.
3. **Analysis and Visualizations:** Summarized install and rating metrics and produced three visualizations (top 10 categories by total installs, rating distribution across Free vs. Paid apps, and app counts across install tiers) with written interpretations, conclusions, and limitations.

## Team Members & Contributions

* **RAGHAD SAAD JARMAN** — *Project Framing & Data Understanding*  
  Defined the research question and objectives, sourced the Kaggle dataset, configured the Google Colab environment, and performed initial structural and missing-value diagnostics.

* **MANAL MOHAMMED** — *Data Cleaning & Preparation*  
  Standardized numeric fields (`Installs`, `Price`, `Rating`), handled duplicates and missing values, engineered the `Install_Tier` feature, aggregated category metrics, and generated the final cleaned dataset.

* **JUDI MAHDI** — *Reproducibility, GitHub & Presentation* 
  Verified end-to-end notebook execution, structured the public GitHub repository, authored project documentation (`README.md`), and aligned presentation slides with course CLOs.

* **MOZON SAEED** — *Statistical Analysis & Visualization* 
  Conducted comparative statistical analysis across categories and pricing types, built three labeled visualizations, and authored interpretations, conclusions, and limitations.
