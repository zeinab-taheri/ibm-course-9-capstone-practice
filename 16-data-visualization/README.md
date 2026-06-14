# Data Visualization Practice

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## Project overview

This practice project focuses on extracting survey data, storing it in a SQLite database, running basic SQL queries, and creating visualizations with pandas and matplotlib.

## Files

- `data_visualization.ipynb` — clean practice notebook
- `requirements.txt` — Python libraries needed to run the notebook

## Skills practiced

- Loading CSV data with pandas
- Creating a SQLite database
- Writing a DataFrame to a SQL table
- Running SQL queries with pandas
- Counting rows and listing tables
- Checking table schema
- Creating histograms, box plots, scatter plots, bubble plots, pie charts, stacked bar charts, line charts, and horizontal bar charts

## Important notes

- The dataset stores `Age`, `TimeSearching`, and `Frustration` as categorical text values, so some visualizations use approximate mappings.
- The `CompTotal` column contains extreme values, so the histogram limits the displayed range for readability.
- The bubble plot is mainly a practice visualization because the selected variables are categorical and do not naturally create a strong numeric bubble plot.
- The age group `30-35` is not available exactly in the dataset, so `25-34 years old` is used as the closest available proxy for the stacked bar chart.

## How to run

1. Install the requirements:

```bash
pip install -r requirements.txt
```

2. Open the notebook:

```bash
jupyter notebook data_visualization.ipynb
```
