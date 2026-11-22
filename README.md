# Google Play Store Apps Data Analysis

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

| Team Member | Primary Role | Key Contributions |
| :--- | :--- | :--- |
| **Raghad Saad Jarman** | Data Understanding & Lead | Topic selection, research question & objective, dataset sourcing, environment setup, loading, and initial data inspection. |
| **Member 2 Name** | Data Engineering & Cleaning | Duplicate & invalid entry removal, numeric formatting cleanup, median imputation, `Install_Tier` transformation, aggregation, and exporting `googleplaystore_cleaned.csv`. |
| **Member 3 Name** | Data Analysis & Visualization | Statistical summaries, creating and interpreting three visualizations, and formulating evidence-based conclusions and limitations. |
| **Member 4 Name** | Documentation & Repository Lead | Notebook structuring, end-to-end reproducibility verification, GitHub repository management, `README.md` documentation, and presentation design. |
