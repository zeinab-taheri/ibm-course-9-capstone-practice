# Normalizing Data Practice

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice notebook covers

- Loading a survey dataset with pandas
- Checking duplicate rows
- Removing duplicate rows
- Checking missing values in `CodingActivities`
- Filling missing `CodingActivities` values using forward-fill
- Identifying compensation-related columns
- Cleaning valid salary values for normalization
- Applying Min-Max normalization to `ConvertedCompYearly`
- Applying Z-score normalization to `ConvertedCompYearly`
- Creating clearer histograms after removing extreme salary outliers only for visualization

## Important note about the charts

The original salary chart can look unreadable because a few very large salary values stretch the x-axis.

To make the distribution easier to read, the notebook removes the extreme top 1% salary values only in the plotting copy of the data.

The original dataset is not changed by this visualization step.

## Key learning

Normalization changes the scale of numerical data so values are easier to compare.

Min-Max normalization converts values into a 0 to 1 range.

Z-score normalization shows how far each value is from the average.

## Files

- `normalizing_data_practice.ipynb` — practice notebook
- `requirements.txt` — Python libraries needed to run the notebook
