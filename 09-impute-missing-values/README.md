# Impute Missing Values with Pandas

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice covers

This folder practises simple missing-value handling using pandas.

The notebook covers:

- loading a CSV dataset
- checking duplicate rows
- removing duplicates if needed
- checking missing values
- identifying missing values in the `RemoteWork` column
- finding the most common `RemoteWork` value
- filling missing `RemoteWork` values using the mode
- checking compensation-related columns
- reviewing basic distribution information for compensation data

## Dataset

The notebook uses the survey dataset provided in the course lab through a public CSV URL.

## Key pandas methods used

- `pd.read_csv()`
- `df.head()`
- `df.duplicated()`
- `df.drop_duplicates()`
- `df.isnull().sum()`
- `df["column"].value_counts()`
- `df["column"].mode()`
- `df["column"].fillna()`
- `df.describe(include="all")`

## Important note

Mode imputation is a simple practice method. Replacing many missing `RemoteWork` values with the most common answer may distort real analysis.

The compensation columns also show data-quality issues. `CompTotal` contains extreme unrealistic values, so it should not be trusted without further cleaning. `ConvertedCompYearly` is safer for salary analysis, but it still has many missing values.
