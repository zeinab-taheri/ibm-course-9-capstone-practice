# Finding Missing Values with Pandas

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice covers

This notebook practises how to:

- load a CSV dataset
- inspect dataset structure
- identify missing values in all columns
- count missing values in specific columns
- visualise missing values using a heatmap
- find the most frequent value in a categorical column
- practise filling missing values using the mode
- visualise the top Employment categories after imputation

## Dataset

The notebook uses the survey dataset provided in the course lab through a public CSV URL.

## Libraries used

- pandas
- matplotlib
- seaborn

## Key methods used

- `pd.read_csv()`
- `df.info()`
- `df.describe()`
- `df.isnull().sum()`
- `sns.heatmap()`
- `mode()`
- `fillna()`
- `value_counts()`

## Important note

In this dataset, the `Employment` column had zero missing values.  
So the imputation step is mainly a practice/demo step, not a real correction of missing Employment data.

The final chart uses only the top 10 Employment categories because the full column has too many long category names and becomes unreadable.

## What I learned

I learned how to check missing values, count them, visualise missing-value patterns, and practise simple mode-based imputation for categorical data.
