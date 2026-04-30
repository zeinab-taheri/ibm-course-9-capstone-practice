# Removing Duplicates with Pandas

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice covers

This folder practises basic data-cleaning steps using pandas:

- loading a CSV dataset
- checking for duplicate rows
- removing duplicate rows
- checking missing values
- filling missing values in a categorical column using the mode
- filling missing yearly compensation values using the median

## Dataset

The notebook uses the survey dataset provided in the course lab through a public CSV URL.

## Key pandas methods used

- `pd.read_csv()`
- `df.duplicated()`
- `df.drop_duplicates()`
- `df.isnull().sum()`
- `mode()`
- `median()`
- `fillna()`

## Important note

In the notebook version reviewed, no duplicate rows were found.  
So this practice shows how to check and remove duplicates, but it should not be described as a project where duplicate records were actually removed.

The `ConvertedCompYearly` column had many missing values, so median imputation is only a simple practice method. In real analysis, I would investigate why those salary values are missing before relying on the cleaned result.

## What I learned

I learned how to use pandas to inspect data quality, identify duplicate rows, remove duplicates when needed, and handle simple missing-value issues before further analysis.
