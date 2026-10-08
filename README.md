# Week 1 – Data Cleaning and Preliminary Analysis with R

## Project Overview
This project completes the Week 1 task on **Data Cleaning and Preliminary Analysis with R**. The project uses a publicly available World Bank fertility-rate dataset. The dataset contains country-level categorical fields and annual numerical fertility-rate values, including missing observations. The goal is to show a complete beginner-friendly but professional data-cleaning workflow before deeper analysis.

The analysis focuses on the **2000–2011** period. During the initial inspection, the supplied dataset snapshot contained completely empty columns for 2012 and 2013, so those columns were removed instead of being filled with invented values. Missing values in the working year columns were then identified and handled using median imputation. The 2010 fertility rate was used as the main variable for preliminary analysis because it provides a clear example of distribution analysis, outlier detection and normalization.

The project also applies the **IQR method** to detect outliers, uses **min-max normalization** to scale the 2010 fertility rate between 0 and 1, and demonstrates **categorical encoding** using R factors and one-hot encoding. Exploratory analysis includes descriptive statistics, yearly mean trends, country rankings and correlation analysis. Six charts are included to provide visual evidence for the cleaning and analytical steps.

The main finding is that average fertility declines steadily across the working period, from approximately 3.25 births per woman in 2000 to 2.85 in 2011. The 2010 distribution is right-skewed, and four high values are flagged as outliers using the IQR rule.

## Files
- `Week1_Data_Cleaning_Preliminary_Analysis_Report.docx` – final report for portal submission.
- `Week1_Data_Cleaning_Preliminary_Analysis.R` – complete R script.
- `world_bank_fertility.csv` – original working dataset.
- `world_bank_fertility_cleaned.csv` – cleaned and transformed dataset.
- `charts/` – six visualization files.
- `outputs/` – summary tables, missing-value results, outlier results, correlations and encoding output.

## How to run in R / RStudio / VS Code
1. Put all project files in the same folder.
2. Open `Week1_Data_Cleaning_Preliminary_Analysis.R`.
3. Make sure `world_bank_fertility.csv` is in the same folder.
4. Run the script from top to bottom.
5. The script creates an `outputs` folder and saves analysis tables and PNG charts.
6. It also creates/updates `world_bank_fertility_cleaned.csv`.

The script uses **base R**, so no additional R packages are required.

## Data source
World Bank, World Development Indicators: Fertility rate, total (births per woman), indicator `SP.DYN.TFRT.IN`. The dataset snapshot used in this project was distributed through the statsmodels dataset collection.
