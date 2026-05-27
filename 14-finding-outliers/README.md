# Finding Outliers

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## Project focus

This practice notebook reviews exploratory data analysis techniques for detecting and handling outliers in a survey dataset.

## What this notebook covers

- Loading and previewing a dataset with pandas
- Checking the dataset structure with `info()`
- Plotting respondent distribution by industry
- Identifying high compensation outliers using a statistical threshold
- Detecting compensation outliers using the IQR method
- Creating a new DataFrame with only the IQR outliers removed
- Converting age groups into approximate numeric values for correlation analysis
- Visualizing correlations with a heatmap

## Key tools used

- Python
- pandas
- matplotlib
- seaborn

## Important notes

- The original dataset is not overwritten.
- The corrected outlier-removal step removes only IQR outliers from `ConvertedCompYearly`.
- Rows with missing `ConvertedCompYearly` values are kept because missing values are not outliers.
- Age groups are mapped to approximate numeric values, so the correlation analysis should be interpreted carefully.

## Files

- `finding_outliers.ipynb` — cleaned practice notebook
- `requirements.txt` — required Python libraries
