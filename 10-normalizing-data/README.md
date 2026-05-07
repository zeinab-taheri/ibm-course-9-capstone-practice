# Normalizing Data Practice

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## Goal

Practice basic data cleaning and normalization using survey compensation data.

## What this notebook does

- Loads a CSV dataset with pandas
- Checks duplicate rows
- Removes duplicate rows if any exist
- Checks missing values in `CodingActivities`
- Fills `CodingActivities` with forward-fill as a practice method
- Prepares `ConvertedCompYearly` for normalization
- Applies Min-Max scaling to yearly compensation
- Applies Z-score normalization to yearly compensation
- Uses histograms to compare the original and normalized distributions

## Dataset

The notebook uses the survey dataset link provided in the course lab.

Main column used:

- `ConvertedCompYearly` — yearly compensation converted into a common format

## Key concepts practiced

### Duplicate checking

`duplicated().sum()` counts repeated rows.  
`drop_duplicates()` removes repeated rows.

### Missing value checking

`isna().sum()` counts empty values in a column.

### Forward-fill practice

`ffill()` fills a missing value using the value from the row above.

This is used here only as a simple practice method.

### Min-Max scaling

Min-Max scaling changes values into a range between 0 and 1.

### Z-score normalization

Z-score normalization shows how far each value is from the average.

## Important limitations

- Forward-fill is only a practice shortcut and may not be suitable for real survey analysis.
- Missing values in `ConvertedCompYearly` must be handled before normalization.
- Salary data can contain extreme outliers.
- Min-Max scaling can be strongly affected by very large outliers.
- This is a learning notebook, not a full professional compensation analysis.

## Files

- `normalizing_data_practice.ipynb` — main practice notebook
- `requirements.txt` — Python libraries used
