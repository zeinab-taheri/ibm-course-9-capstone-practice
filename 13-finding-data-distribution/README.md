# 13 – Finding How the Data Is Distributed

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice is about

This notebook practises checking how data is distributed.

Distribution means understanding how values are spread across columns, which values appear most often, and whether there are visible patterns in the data.

## Main skills practised

- loading a CSV dataset with pandas
- examining dataframe structure
- checking missing values
- creating a consistent cleaned dataframe
- analysing category distributions with `value_counts()`
- visualising job satisfaction distribution
- comparing programming languages people have used and want to use
- analysing overall remote work distribution
- converting professional coding experience into numeric values
- calculating Pearson correlation
- comparing employment type and education level with crosstab
- creating a readable stacked bar chart using top employment categories
- exporting the cleaned dataframe as a CSV file

## Main Python tools used

- `pandas`
- `matplotlib`
- `seaborn`
- `Counter`
- `read_csv()`
- `head()`
- `columns`
- `dtypes`
- `info()`
- `isnull().sum()`
- `copy()`
- `fillna()`
- `value_counts()`
- `astype()`
- `sns.kdeplot()`
- `plt.pie()`
- `str.split()`
- `Counter()`
- `pd.DataFrame()`
- `sort_values()`
- `plot(kind='bar')`
- `replace()`
- `pd.to_numeric()`
- `dropna()`
- `corr()`
- `pd.crosstab()`
- `isin()`
- `to_csv()`

## Important correction

The original lab workflow created `df_cleaned = df.dropna()` but then mostly continued using `df`.

In this practice version, the workflow is corrected:

- `df` stays as the original loaded dataset.
- `df_cleaned` is created with `df.copy()`.
- missing `RemoteWork` values are filled in `df_cleaned` with `Unknown`.
- missing `JobSat` values are filled in `df_cleaned` with `Not answered`.
- distribution analysis uses `df_cleaned`.
- correlation uses a separate `corr_df` so the main dataframe is not damaged.
- the education/employment full crosstab keeps all categories.
- the education/employment chart uses only the top 5 employment types so it is readable.
- the final CSV exports `df_cleaned`.

## Important warnings

- `Not answered` and `Unknown` are clear labels for missing values, but they should be interpreted carefully.
- The RemoteWork chart shows overall distribution, not distribution by region.
- Programming language trends are based on survey respondents only.
- The pie chart is included for practice, but it can be harder to read than a bar chart when there are many categories.
- Pearson correlation shows relationship strength, but it does not prove cause and effect.
- Stacked bar charts can become messy when category labels are long or combined.

## Files in this folder

- `README.md`
- `finding_data_distribution_practice.ipynb`
- `requirements.txt`

## Very short memory line

load data → inspect structure → clean consistently → count distributions → visualise JobSat → compare languages → check RemoteWork → calculate correlation safely → compare education/employment → export `df_cleaned`
