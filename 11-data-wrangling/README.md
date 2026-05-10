# 11 – Data Wrangling

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice is about

This notebook practises basic data wrangling skills.

Data wrangling means cleaning, fixing, transforming, and preparing raw data before analysis.

## Main skills practised

- loading a CSV dataset with pandas
- checking dataset structure
- checking missing values
- standardising messy category names
- encoding categorical variables with one-hot encoding
- filling missing numerical values with the median
- filling missing categorical values with the most frequent value
- applying Min-Max scaling
- applying log transformation
- creating a new experience-level column

## Main Python tools used

- `pandas`
- `numpy`
- `read_csv()`
- `info()`
- `isnull().sum()`
- `describe()`
- `unique()`
- `replace()`
- `get_dummies()`
- `concat()`
- `median()`
- `mode()`
- `fillna()`
- `apply()`
- `np.log1p()`

## Important notes

This is a practice notebook, not a final professional analysis.

Some data-cleaning choices are simple learning shortcuts:

- Missing salary values are filled with the median for practice.
- Missing RemoteWork values are filled with the most common value for practice.
- Salary data may contain extreme outliers, so salary-based transformations should be interpreted carefully.
- The original course-style `inplace=True` approach was avoided because it can cause future pandas issues.
- Missing experience values are handled as `Unknown` so they are not wrongly labelled as `Senior`.

## Files in this folder

- `data_wrangling_practice.ipynb`
- `requirements.txt`
- `README.md`

## Very short memory line

check messy data → standardise category names → encode text columns → fill missing values carefully → scale/log salary → create experience groups → watch out for shortcuts
