# Finding Correlations

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## Project overview

This practice project explores relationships between key variables in a developer survey dataset. The focus is on yearly compensation, work experience, job satisfaction, outlier handling, and correlation analysis.

## What this notebook covers

- Loading a survey dataset with pandas
- Plotting the distribution of yearly compensation
- Calculating median compensation for full-time employees
- Comparing compensation distributions by country with box plots
- Removing compensation outliers using the IQR method
- Calculating correlations between selected numeric variables
- Visualizing correlations with a heatmap
- Creating scatter plots to inspect relationships visually

## Key variables used

- `ConvertedCompYearly`: yearly compensation converted to USD
- `WorkExp`: years of work experience
- `JobSatPoints_1`: job satisfaction score
- `Country`: respondent country
- `Employment`: employment status

## Main takeaway

After removing extreme compensation outliers, work experience shows a moderate positive relationship with yearly compensation, while job satisfaction shows little to no clear relationship with compensation.

## Files

- `finding_correlations.ipynb` — clean practice notebook
- `requirements.txt` — Python libraries used

## Libraries

- pandas
- matplotlib
- seaborn
