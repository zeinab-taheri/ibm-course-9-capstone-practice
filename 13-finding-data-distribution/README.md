# 13 – Finding How The Data Is Distributed

This is my own practice notebook based on what I learned in the IBM Data Analyst Capstone Project on Coursera.

## What this practice is about

This notebook practises checking how data is distributed.

Distribution means understanding how values are spread across a column, which answers are common, which answers are rare, and whether there are visible patterns in the data.

## Main skills practised

- loading a CSV dataset with pandas
- previewing the dataset
- checking column names and data types
- checking missing values
- filling selected missing values
- counting category values with `value_counts()`
- visualising job satisfaction distribution
- using KDE plots and pie charts
- splitting multi-answer programming language columns
- counting programming languages with `Counter`
- comparing languages people have worked with vs want to work with
- visualising remote work distribution
- converting text experience values into numbers
- calculating Pearson correlation
- comparing employment and education with `pd.crosstab()`
- creating stacked bar charts
- exporting a CSV file

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
- `dropna()`
- `fillna()`
- `value_counts()`
- `astype(float)`
- `sns.kdeplot()`
- `plt.pie()`
- `str.split(';')`
- `sum()`
- `pd.DataFrame()`
- `sort_values()`
- `plot(kind='bar')`
- `replace()`
- `pd.to_numeric()`
- `corr(method='pearson')`
- `pd.crosstab()`
- `to_csv()`

## Important notes

This is a practice notebook, not a final professional analysis.

Important limitations from the lab workflow:

- `df_cleaned = df.dropna()` is created, but the later analysis continues mainly with `df`.
- Missing `RemoteWork` values are filled with `Unknown`.
- Missing `JobSat` values are filled with `Not answered`, then later removed before numeric satisfaction analysis.
- The remote work section says region in the instruction, but the code shows overall remote work distribution, not region-based distribution.
- The correlation section changes `df` by removing rows where `JobSat` is `Not answered`.
- Because `df` is changed during the correlation step, later crosstab and export steps use the filtered version of `df`.
- The final CSV saves `df`, not `df_cleaned`.
- Correlation does not prove cause and effect.

## Files in this folder

- `finding_data_distribution_practice.ipynb`
- `requirements.txt`
- `README.md`

## Very short memory line

load data → inspect structure → check missing values → count distributions → visualise JobSat → compare languages → check remote work → calculate correlation → compare education/employment → export CSV
