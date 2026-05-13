# 12 – Exploratory Data Analysis

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice is about

This notebook practises Exploratory Data Analysis, also called EDA.

EDA means looking at data before making conclusions. The goal is to understand missing values, patterns, relationships, and trends using tables and charts.

## Main skills practised

- loading and previewing a dataset
- checking missing values
- calculating missing percentages
- finding mode values
- filling missing values for lab practice
- creating a cleaned dataframe copy
- converting mixed text and numeric experience values
- grouping experience into ranges
- comparing job satisfaction by experience range
- visualising job satisfaction distribution
- visualising remote work distribution
- comparing categories with crosstab
- analysing programming language trends by region
- calculating correlation with `corr()`
- creating scatter plots and bar charts
- simplifying messy charts using top categories
- saving the cleaned dataframe as a CSV file

## Main Python tools used

- `pandas`
- `matplotlib`
- `seaborn`
- `read_csv()`
- `head()`
- `set_option()`
- `isnull().sum()`
- `mean() * 100`
- `mode()`
- `copy()`
- `dropna()`
- `fillna()`
- `def convert_years()`
- `apply()`
- `pd.cut()`
- `groupby()`
- `median()`
- `agg()`
- `sns.countplot()`
- `pd.crosstab()`
- `value_counts()`
- `str.split()`
- `explode()`
- `corr()`
- `plt.scatter()`
- `plot(kind='bar')`
- `to_csv()`

## Important notes

This is a practice notebook, not a final professional analysis.

Important limitations:

- Missing `JobSat` values are filled with the most common value (`8.0`) for the lab cleaning task.
- Because many `JobSat` values are missing, later JobSat analysis uses real JobSat answers from the original dataframe instead of the filled values.
- Missing `RemoteWork` values are filled with the most common value: `Hybrid (some remote, some in-person)`.
- Because missing `RemoteWork` values are filled with Hybrid, the Hybrid category may be inflated.
- Programming language results show trends among survey respondents only, not the whole country population.
- The scatter plot visualises the relationship between experience and satisfaction, but `corr()` calculates the actual correlation value.
- Correlation does not prove cause and effect.
- The education/employment chart uses the top 5 employment types to keep the chart readable.
- The final CSV saves `df_clean`, because that is the cleaned dataframe.

## Files in this folder

- `exploratory_data_analysis_practice.ipynb`
- `requirements.txt`
- `README.md`

## Very short memory line

load data → check missing values → fill for lab → use real JobSat for analysis → group experience → visualise patterns → calculate correlation → compare categories → save `df_clean`
