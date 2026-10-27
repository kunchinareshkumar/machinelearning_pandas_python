# 🐼 Pandas — The Complete Guide (Zero to Advanced)

### 📊 Python Data Analysis • Data Cleaning • EDA • AI/ML Testing • QA Engineering

<p align="center">
  <a href="https://github.com/kunchinareshkumar/machinelearning_pandas_python/blob/main/pandasfull.ipynb">
    <img src="https://img.shields.io/badge/📘_Explore-Full_Pandas_Notebook-150458?style=for-the-badge" alt="Explore Pandas Notebook"/>
  </a>
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas" alt="Pandas"/>
  <img src="https://img.shields.io/badge/Level-Zero_to_Advanced-7C3AED?style=for-the-badge" alt="Zero to Advanced"/>
  <img src="https://img.shields.io/badge/Focus-AI%2FML_QA-16A34A?style=for-the-badge" alt="AI ML QA"/>
</p>

---

## 🌟 Welcome to the Pandas Learning Repository!

Learn Python Pandas step by step, from basic Series and DataFrames to advanced data manipulation, data cleaning, exploratory data analysis (EDA), statistical summaries, and real-world data quality validation.

This repository is designed for:

- 🐍 Python beginners
- 🧪 QA Engineers and SDETs
- 🤖 AI/ML Test Engineers
- 📊 Data QA Engineers and Data Analysts
- 🔬 Machine Learning and Data Science learners
- 🚀 Automation Engineers looking to expand into data testing

**Learning approach:** Understand the concept → Write the code → Inspect the output → Validate the result → Apply it to a real-world dataset.

## 🎯 What You Will Learn

| Learning Area | Skills You Will Build |
|---|---|
| 🧱 Pandas Fundamentals | Series, DataFrames, indexes, data types |
| 📂 Data Loading | CSV, Excel, JSON, text files |
| 🔍 Data Inspection | Shape, columns, data types, summaries |
| 🧹 Data Cleaning | Missing values, duplicates, inconsistent data |
| 🎯 Data Selection | Indexing, slicing, filtering, conditional selection |
| 🔄 Data Transformation | Apply, map, replace, type conversion |
| 🔗 Data Combination | Concatenation, merge, join |
| 📊 Data Analysis | GroupBy, aggregation, pivot tables |
| 📅 Time Series | Datetime conversion, resampling, time-based analysis |
| 📈 Visualization | Line, bar, histogram, box, and other plots |
| 🤖 AI/ML Testing | Data validation, feature checks, model input validation |
| ⚡ Advanced Pandas | MultiIndex, performance, vectorization, chunk processing |

---

## 📚 Table of Contents

| # | Topic | Main Concepts |
|---:|---|---|
| 01 | [Introduction to Pandas](#-01-introduction-to-pandas) | Overview and use cases |
| 02 | [Installation and Setup](#-02-installation-and-setup) | Python environment |
| 03 | [Series and DataFrames](#-03-series-and-dataframes) | Core data structures |
| 04 | [Creating DataFrames](#-04-creating-series-and-dataframes) | Lists, dictionaries, arrays |
| 05 | [Reading and Writing Files](#-05-reading-and-writing-files) | CSV, Excel, JSON, TXT |
| 06 | [Inspecting Data](#-06-inspecting-and-understanding-data) | Shape, info, describe |
| 07 | [Selecting and Filtering](#-07-selecting-and-filtering-data) | `loc`, `iloc`, conditions |
| 08 | [Indexing and Sorting](#-08-indexing-and-sorting) | Index, sort, reset |
| 09 | [Data Types](#-09-data-types-and-conversion) | `dtypes`, `astype()` |
| 10 | [Missing Values](#-10-handling-missing-values) | `isna`, `dropna`, `fillna` |
| 11 | [Duplicates and Data Cleaning](#-11-duplicates-and-data-cleaning) | Deduplication, normalization |
| 12 | [Data Transformation](#-12-data-transformation) | `map`, `apply`, `replace` |
| 13 | [String Operations](#-13-string-operations) | Text cleaning and validation |
| 14 | [GroupBy and Aggregation](#-14-groupby-and-aggregation) | Group summaries |
| 15 | [Merge, Join and Concatenate](#-15-merge-join-and-concatenate) | Combining datasets |
| 16 | [Reshaping Data](#-16-reshaping-data) | Pivot, melt, stack |
| 17 | [Date and Time](#-17-date-and-time-operations) | Datetime, resampling |
| 18 | [Statistics and Outliers](#-18-statistics-and-outlier-analysis) | Descriptive statistics, IQR |
| 19 | [Pandas Visualization](#-19-pandas-data-visualization) | Charts and plots |
| 20 | [Advanced Pandas](#-20-advanced-pandas-concepts) | MultiIndex, chunks, optimization |
| 21 | [AI/ML and QA Applications](#-21-pandas-for-aiml-and-qa-testing) | Data quality and validation |
| 22 | [Practice Projects](#-22-practical-projects) | Hands-on exercises |
| 23 | [Interview Preparation](#-23-interview-preparation) | Common interview questions |
| 24 | [Run the Notebook](#-24-how-to-run-the-notebook) | Local setup |
| 25 | [Learning Roadmap](#-25-learning-roadmap) | Recommended sequence |
| 26 | [Official References](#-26-official-references) | Documentation |

---

## 🐼 01. Introduction to Pandas

Pandas is an open-source Python library for working with structured and labeled data. It provides powerful data structures and tools for cleaning, transforming, analyzing, and preparing datasets.

### Why Pandas?

- Read data from files and databases.
- Inspect and understand unfamiliar datasets.
- Identify missing values and duplicate records.
- Filter rows and select columns.
- Combine multiple datasets.
- Perform aggregations and statistical analysis.
- Prepare datasets for machine learning.
- Validate data quality before model training or application processing.

## 🛠️ 02. Installation and Setup

Install the required libraries:

```bash
python3 -m pip install pandas numpy matplotlib openpyxl jupyter
```

Import the libraries:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

print(pd.__version__)
print(np.__version__)
```

Create a simple DataFrame:

```python
df = pd.DataFrame({
    "Name": ["Asha", "Ravi", "John"],
    "Age": [25, 30, 28],
    "Score": [85, 90, 78]
})

print(df)
```

## 🧱 03. Series and DataFrames

Pandas has two fundamental data structures.

| Feature | Series | DataFrame |
|---|---|---|
| Structure | One-dimensional | Two-dimensional |
| Contains | Values with an index | Rows and labeled columns |
| Example | One column of scores | Complete student dataset |
| Creation | `pd.Series()` | `pd.DataFrame()` |

Example:

```python
# Series
scores = pd.Series([85, 90, 78])

# DataFrame
df = pd.DataFrame({
    "Name": ["Asha", "Ravi", "John"],
    "Score": [85, 90, 78]
})

print(scores)
print(df)
```

## 🏗️ 04. Creating Series and DataFrames

Learn to create DataFrames from:

- Lists and nested lists
- Dictionaries
- NumPy arrays
- Series objects
- CSV and Excel files
- JSON records
- Other DataFrames

```python
df = pd.DataFrame({
    "Employee": ["A", "B", "C"],
    "Department": ["QA", "Dev", "Data"],
    "Salary": [50000, 65000, 70000]
})

print(df.head())
```

## 📂 05. Reading and Writing Files

Pandas supports multiple data formats.

| Format | Read | Write |
|---|---|---|
| CSV | `pd.read_csv()` | `df.to_csv()` |
| Excel | `pd.read_excel()` | `df.to_excel()` |
| JSON | `pd.read_json()` | `df.to_json()` |
| Parquet | `pd.read_parquet()` | `df.to_parquet()` |
| SQL | `pd.read_sql()` | `df.to_sql()` |
| Text | `pd.read_csv(sep=...)` | `df.to_csv(sep=...)` |

Examples:

```python
df = pd.read_csv("customers.csv")
print(df.head())
```

Read an Excel file:

```python
df = pd.read_excel("customers.xlsx")
print(df.head())
```

Read a tab-separated text file:

```python
df = pd.read_csv("customers.txt", sep="\t")
print(df.head())
```

Save the cleaned result:

```python
df.to_csv("cleaned_customers.csv", index=False)
```

For Excel files, `openpyxl` is commonly used with `.xlsx` files. Other formats may require additional engines or database drivers.

## 🔍 06. Inspecting and Understanding Data

Inspection should be the first step after loading an unfamiliar dataset.

| Method | Purpose |
|---|---|
| `df.head()` | First five rows by default |
| `df.tail()` | Last five rows by default |
| `df.sample()` | Random sample of rows |
| `df.shape` | Number of rows and columns |
| `df.columns` | Column labels |
| `df.index` | Row index |
| `df.dtypes` | Column data types |
| `df.info()` | Structure and non-null counts |
| `df.describe()` | Descriptive statistics |
| `df.nunique()` | Unique-value counts |
| `df.isna().sum()` | Missing values by column |
| `df.duplicated().sum()` | Number of duplicate rows |

Example:

```python
df = pd.read_csv("customers.csv")

print(df.shape)
print(df.columns)
print(df.dtypes)
print(df.isna().sum())

df.info()
print(df.describe(include="all"))
```

## 🎯 07. Selecting and Filtering Data

### Select columns

```python
print(df["Name"])
print(df[["Name", "Age"]])
```

### Select rows with `loc` and `iloc`

```python
print(df.loc[0, "Name"])  # Label-based selection
print(df.iloc[0, 0])      # Position-based selection
print(df.iloc[:5, :3])    # First 5 rows, first 3 columns
```

### Filter using conditions

```python
adults = df[df["Age"] >= 18]

high_scores = df[df["Score"] >= 80]

print(adults)
print(high_scores)
```

### Combine conditions

```python
result = df[
    (df["Age"] >= 25) &
    (df["Score"] >= 80)
]

print(result)
```

Practice `isin()`, `between()`, `query()`, `where()`, and `mask()`.

## 🔢 08. Indexing and Sorting

Important concepts:

- Setting and resetting indexes
- Sorting by one or more columns
- Sorting index labels
- Selecting rows by index
- Renaming index labels
- Reindexing
- Working with non-unique indexes

```python
sorted_df = df.sort_values(
    by="Score",
    ascending=False
)

print(sorted_df)
```

Reset the index:

```python
df = df.reset_index(drop=True)
```

## 🔄 09. Data Types and Conversion

Correct data types improve data quality and prevent unexpected calculations.

```python
df["Age"] = df["Age"].astype("int64")
```

Convert numeric strings safely:

```python
df["Score"] = pd.to_numeric(
    df["Score"],
    errors="coerce"
)
```

Convert dates:

```python
df["Date"] = pd.to_datetime(
    df["Date"],
    errors="coerce"
)
```

Learn integer, floating-point, string, boolean, categorical, datetime, and nullable Pandas data types.

## 🧹 10. Handling Missing Values

Missing data can affect reporting, statistics, and machine learning.

| Method | Purpose |
|---|---|
| `isna()` / `isnull()` | Detect missing values |
| `notna()` | Identify non-missing values |
| `dropna()` | Remove rows or columns with missing values |
| `fillna()` | Replace missing values |
| `ffill()` | Fill using the previous valid value |
| `bfill()` | Fill using the next valid value |
| `interpolate()` | Estimate missing values between observations |

Example:

```python
df = pd.DataFrame({
    "Name": ["Asha", "Ravi", "John"],
    "Age": [25, np.nan, 30],
    "Score": [85, 90, np.nan]
})

print(df.isna().sum())

df["Age"] = df["Age"].fillna(df["Age"].median())
df["Score"] = df["Score"].fillna(df["Score"].mean())

print(df)
```

**Important:** Choose a missing-value strategy based on business meaning and data characteristics. For ML workflows, calculate imputation values using training data only to avoid data leakage.

## 🧽 11. Duplicates and Data Cleaning

Common operations:

```python
df.duplicated()
df.duplicated().sum()
df.drop_duplicates()
df.drop_duplicates(subset=["Email"])
df.rename(columns={"OldName": "NewName"})
df.replace("Unknown", np.nan)
df.columns = df.columns.str.strip()
```

Typical data-cleaning tasks:

- Standardize column names.
- Remove unwanted whitespace.
- Identify duplicate records.
- Correct inconsistent categories.
- Validate numeric ranges.
- Handle missing or invalid dates.
- Normalize text and categorical values.
- Check uniqueness constraints.
- Preserve original data when traceability is required.

## 🔧 12. Data Transformation

Learn to transform values and derive new columns.

```python
df["Score_Percentage"] = df["Score"] / 100 * 100
```

Apply conditional logic:

```python
df["Result"] = np.where(
    df["Score"] >= 50,
    "Pass",
    "Fail"
)
```

Other methods:

- `map()`
- `apply()`
- `replace()`
- `assign()`
- `where()`
- `mask()`
- `cut()`
- `qcut()`
- `select_dtypes()`

Prefer built-in vectorized operations where practical; they are often clearer and faster than row-by-row Python functions.

## 🔤 13. String Operations

Pandas provides the `.str` accessor for common text-processing tasks.

```python
df["Name"] = df["Name"].str.strip()
df["Name"] = df["Name"].str.lower()
```

Useful operations:

| Operation | Example |
|---|---|
| Lowercase | `df["Name"].str.lower()` |
| Uppercase | `df["Name"].str.upper()` |
| Trim whitespace | `df["Name"].str.strip()` |
| Search text | `df["Name"].str.contains("ash", na=False)` |
| Replace text | `df["Name"].str.replace("old", "new")` |
| Split text | `df["Name"].str.split(" ")` |
| Check prefixes | `df["Name"].str.startswith("A", na=False)` |
| Extract patterns | `df["Email"].str.extract(...)` |

These operations are especially useful for cleaning names, emails, identifiers, log fields, and categorical values.

## 📊 14. GroupBy and Aggregation

GroupBy allows you to summarize data by category.

```python
summary = df.groupby("Department")["Salary"].mean()

print(summary)
```

Multiple aggregations:

```python
summary = df.groupby("Department").agg({
    "Salary": ["mean", "min", "max", "count"]
})

print(summary)
```

Learn:

- `groupby()`
- `agg()`
- `transform()`
- `filter()`
- `value_counts()`
- `crosstab()`
- Grouping by multiple columns
- Handling missing group keys

Applications include defect counts by module, API failures by endpoint, test execution by build, and data quality metrics by source.

## 🔗 15. Merge, Join and Concatenate

Combining datasets is one of the most important Pandas skills.

| Method | Purpose |
|---|---|
| `pd.concat()` | Combine datasets along rows or columns |
| `pd.merge()` | Match records using key columns |
| `df.join()` | Combine DataFrames primarily by index |

### Merge example

```python
customers = pd.DataFrame({
    "CustomerID": [1, 2, 3],
    "Name": ["Asha", "Ravi", "John"]
})

orders = pd.DataFrame({
    "CustomerID": [1, 2, 4],
    "Amount": [500, 700, 300]
})

result = pd.merge(
    customers,
    orders,
    on="CustomerID",
    how="left",
    indicator=True,
    validate="one_to_one"
)

print(result)
```

Learn inner, left, right, and outer joins; suffixes; duplicate-key handling; index joins; and join validation.

**QA tip:** Use merge indicators and key validation to detect missing relationships, unmatched records, and unexpected duplicate keys.

## 🔀 16. Reshaping Data

Reshaping changes the layout of data without necessarily changing its underlying information.

| Method | Purpose |
|---|---|
| `pivot()` | Convert unique row/column combinations into a table |
| `pivot_table()` | Pivot with aggregation |
| `melt()` | Convert wide data to long format |
| `stack()` | Move a column index level into the row index |
| `unstack()` | Move an index level into columns |
| `explode()` | Expand list-like values into rows |
| `crosstab()` | Summarize category combinations |

Example:

```python
df = pd.DataFrame({
    "Name": ["Asha", "Ravi"],
    "Math": [90, 80],
    "Science": [85, 95]
})

long_df = df.melt(
    id_vars="Name",
    var_name="Subject",
    value_name="Score"
)

print(long_df)
```

## 📅 17. Date and Time Operations

Date and time data is common in logs, reports, event tracking, and performance testing.

```python
df["Date"] = pd.to_datetime(
    df["Date"],
    errors="coerce"
)

df["Year"] = df["Date"].dt.year
df["Month"] = df["Date"].dt.month
df["Day"] = df["Date"].dt.day
df["Weekday"] = df["Date"].dt.day_name()
```

Learn:

- `pd.to_datetime()`
- `.dt` accessor
- Date filtering
- Time differences
- Time zones
- Resampling
- Rolling windows
- Frequency conversion
- Time-series aggregation

## 📈 18. Statistics and Outlier Analysis

Pandas supports descriptive statistics and distribution analysis.

```python
print(df["Score"].mean())
print(df["Score"].median())
print(df["Score"].std())
print(df["Score"].quantile([0.25, 0.50, 0.75]))
```

### IQR-based outlier investigation

```python
Q1 = df["Score"].quantile(0.25)
Q3 = df["Score"].quantile(0.75)

IQR = Q3 - Q1

lower_bound = Q1 - 1.5 * IQR
upper_bound = Q3 + 1.5 * IQR

outliers = df[
    (df["Score"] < lower_bound) |
    (df["Score"] > upper_bound)
]

print(outliers)
```

Learn correlation, covariance, percentiles, variance, frequency distributions, and statistical summaries.

An outlier is not automatically an error. Investigate whether it represents an invalid value, a legitimate rare event, or a meaningful change.

## 📉 19. Pandas Data Visualization

Pandas integrates with Matplotlib to provide convenient plotting methods.

| Plot | Example | Use Case |
|---|---|---|
| Line | `df.plot(kind="line")` | Trends |
| Bar | `df.plot(kind="bar")` | Category comparison |
| Horizontal bar | `df.plot(kind="barh")` | Ranking |
| Histogram | `df.plot(kind="hist")` | Distribution |
| Box | `df.plot(kind="box")` | Spread and outliers |
| Scatter | `df.plot(kind="scatter", x="Age", y="Score")` | Relationships |
| Area | `df.plot(kind="area")` | Cumulative trends |
| Pie | `df["Category"].value_counts().plot(kind="pie")` | Category proportions |
| Density | `df["Score"].plot(kind="density")` | Smoothed distribution |

Example:

```python
import matplotlib.pyplot as plt

df.plot(
    x="Month",
    y="Sales",
    kind="bar",
    title="Monthly Sales"
)

plt.tight_layout()
plt.show()
```

Explore the complete visualization guide in your companion repository:

[📊 Matplotlib — Zero to Advanced for AI/ML QA](https://github.com/kunchinareshkumar/datavisualization-matplotlib-aiml-python/blob/main/Matplotlib_Zero_to_Advanced_AI_ML_QA.ipynb)

## 🚀 20. Advanced Pandas Concepts

After mastering the fundamentals, explore:

- MultiIndex and hierarchical indexing
- Advanced merge and join operations
- Window functions and rolling calculations
- Resampling and time-series analysis
- Categorical data optimization
- Nullable data types
- Memory usage analysis
- Vectorization and performance profiling
- Chunk-based CSV processing
- Query optimization with `query()` and `eval()`
- Reading and writing Parquet
- SQL integration
- Working with large datasets
- Data validation and reusable cleaning pipelines

### Process large CSV files in chunks

```python
for chunk in pd.read_csv("large_dataset.csv", chunksize=10000):
    print(chunk.shape)
```

Each chunk can be validated or processed separately. Aggregate results carefully if the final analysis needs statistics across the entire dataset.

## 🤖 21. Pandas for AI/ML and QA Testing

Pandas is useful for validating structured data throughout a software or machine learning lifecycle.

| Testing Area | Example Application |
|---|---|
| Data ingestion | Verify expected rows and columns |
| Data quality | Check nulls, duplicates, and invalid values |
| Data preprocessing | Validate transformations and encodings |
| Feature engineering | Check derived features and data types |
| Training datasets | Validate schema, ranges, and class distribution |
| Model predictions | Compare expected and actual outputs |
| Regression testing | Compare results between application versions |
| Data drift | Compare feature distributions over time |
| API testing | Validate tabular API responses |
| ETL testing | Reconcile source and target records |
| Test reporting | Analyze failures and defect trends |

### Example: Data Quality Validation

```python
import pandas as pd

df = pd.read_csv("customers.csv")

print("Rows and columns:", df.shape)
print("Missing values:\n", df.isna().sum())
print("Duplicate rows:", df.duplicated().sum())

required_columns = {"CustomerID", "Name", "Age"}

missing_columns = required_columns - set(df.columns)

if missing_columns:
    print("FAIL: Missing columns:", missing_columns)
else:
    print("PASS: Required columns exist")
```

### Example: Validate a Numeric Range

```python
valid_age = df["Age"].between(0, 120)

invalid_records = df[~valid_age & df["Age"].notna()]

print("Invalid age records:")
print(invalid_records)
```

### Example: Compare Two DataFrames

```python
expected = pd.DataFrame({
    "ID": [1, 2, 3],
    "Score": [80, 90, 70]
})

actual = pd.DataFrame({
    "ID": [1, 2, 3],
    "Score": [80, 90, 75]
})

comparison = expected.merge(
    actual,
    on="ID",
    how="outer",
    suffixes=("_expected", "_actual"),
    indicator=True,
    validate="one_to_one"
)

comparison["Score_Match"] = (
    comparison["Score_expected"]
    == comparison["Score_actual"]
)

print(comparison)
```

For production-grade comparisons, define key uniqueness, row ordering, missing-value handling, numerical tolerance, and expected schema explicitly.

## 🧪 22. Practical Projects

Use these projects to develop hands-on skills.

| Project | Objective |
|---|---|
| 01. Student Performance Analysis | Analyze marks, averages, and grades |
| 02. Customer Data Cleaning | Clean names, missing values, and duplicates |
| 03. Sales Analysis | Group, aggregate, and visualize sales |
| 04. CSV Data Quality Validator | Validate schemas, types, and value ranges |
| 05. API Response Validator | Compare structured API responses |
| 06. ETL Reconciliation | Match source and target datasets |
| 07. Test Execution Report | Summarize pass/fail results and trends |
| 08. Defect Trend Analysis | Analyze defect counts by module and release |
| 09. ML Dataset EDA | Analyze distributions and class imbalance |
| 10. Data Drift Investigation | Compare reference and current datasets |

## 🎤 23. Interview Preparation

Practice explaining these questions with examples:

1. What is Pandas, and why is it useful?
2. What is the difference between a Series and a DataFrame?
3. What is the difference between `loc` and `iloc`?
4. How do you read CSV and Excel files?
5. How do you find and handle missing values?
6. What is the difference between `dropna()` and `fillna()`?
7. How do you identify and remove duplicate records?
8. What is the difference between `map()`, `apply()`, and vectorized operations?
9. What is the difference between `merge()`, `join()`, and `concat()`?
10. How does `groupby()` work?
11. How do you find outliers using IQR?
12. How do you handle dates and time zones?
13. How do you process large CSV files?
14. How would you validate an ETL pipeline using Pandas?
15. How would you compare model inputs or predictions across versions?
16. How would you investigate data drift?

---

## ▶️ 24. How to Run the Notebook

### Step 1 — Clone the repository

```bash
git clone https://github.com/kunchinareshkumar/machinelearning_pandas_python.git

cd machinelearning_pandas_python
```

### Step 2 — Create a virtual environment

```bash
python3 -m venv .venv

source .venv/bin/activate
```

### Step 3 — Install the dependencies

```bash
python -m pip install --upgrade pip

python -m pip install pandas numpy matplotlib openpyxl jupyter
```

### Step 4 — Launch Jupyter

```bash
python -m jupyter notebook
```

### Step 5 — Open the notebook

[📘 Open pandasfull.ipynb](https://github.com/kunchinareshkumar/machinelearning_pandas_python/blob/main/pandasfull.ipynb)

Run the cells in order and experiment with the examples.

> If your repository uses a different notebook filename, update the notebook link above to match the actual file.

## 🗺️ 25. Learning Roadmap

| Stage | Focus | Goal |
|---|---|---|
| 🟢 Beginner | Series, DataFrames, reading files | Understand Pandas fundamentals |
| 🟡 Intermediate | Filtering, cleaning, missing values | Prepare reliable datasets |
| 🟠 Upper Intermediate | GroupBy, joins, reshaping | Analyze and combine data |
| 🔵 Advanced | Time series, MultiIndex, performance | Handle complex datasets |
| 🟣 Data Analysis | Statistics, EDA, visualization | Discover patterns and anomalies |
| 🔴 QA Applications | Data validation, reconciliation | Build data quality checks |
| ⭐ AI/ML Applications | Feature validation, drift analysis | Support reliable ML pipelines |
| 🚀 Portfolio | Practical projects and documentation | Demonstrate applied skills |

## 📚 26. Official References

- [Pandas Official Documentation](https://pandas.pydata.org/docs/)
- [Pandas Getting Started Tutorials](https://pandas.pydata.org/docs/getting_started/intro_tutorials/)
- [Pandas User Guide](https://pandas.pydata.org/docs/user_guide/index.html)
- [Pandas API Reference](https://pandas.pydata.org/docs/reference/index.html)
- [NumPy Official Documentation](https://numpy.org/doc/)
- [Matplotlib Official Documentation](https://matplotlib.org/stable/)

---

## 👨‍💻 About the Author

**Naresh Kumar**

Learning and sharing practical resources in:

- Python programming
- NumPy and Pandas
- Data analysis and visualization
- QA automation and API testing
- Data quality engineering
- AI/ML testing and model validation

This repository is part of a hands-on learning journey toward applying Python, data analysis, and quality engineering to AI/ML systems.

## 🤝 Contributions and Feedback

Found something useful or have an improvement to suggest?

- ⭐ Star this repository.
- 🍴 Fork it and practice the examples.
- 🐛 Report an issue or correction.
- 🔗 Share it with other Python, QA, and AI/ML learners.

---

<p align="center">

### 🚀 Load • Inspect • Clean • Transform • Analyze • Validate

**Building strong Pandas foundations for Data Science and AI/ML Quality Engineering.**

---

## 🎨 Visual Study Notes & Cheat Sheets

Learn Pandas data visualization through colorful, easy-to-understand visual notes and practical examples.

These study sheets cover the most commonly used Pandas plotting techniques with Matplotlib and Seaborn.

### 📚 Pandas Visualization — Complete Overview

<p align="center">
  <img src="<img width="1024" height="1536" alt="1  Plotting with Pandas Study Cheat Sheet" src="https://github.com/user-attachments/assets/55ae6121-7412-4d5c-b67c-f07d24f1ea37" />
" alt="Complete Pandas plotting cheat sheet" width="800">
</p>

### 1. 📈 Pandas Line Plot

Visualize trends, changes over time, and comparisons between multiple data series.

<p align="center">
  <img src="<img width="1024" height="1536" alt="2  Pandas - Line plot study notes" src="https://github.com/user-attachments/assets/3701cdb0-210d-46cf-b29d-0623701eeef0" />
" alt="Pandas line plot study notes" width="800">
</p>

### 2. 📊 Pandas Bar Plot

Compare categories, product sales, groups, and numerical values.

<p align="center">
  <img src="<img width="1024" height="1536" alt="3  Pandas Bar Plot Notebook Cheat Sheet" src="https://github.com/user-attachments/assets/41d791de-e534-4035-ae8c-244dcd880727" />
" alt="Pandas bar plot study notes" width="800">
</p>

### 3. 🔵 Pandas Scatter Plot

Explore relationships between numerical variables, correlations, clusters, and outliers.

<p align="center">
  <img src="<img width="1024" height="1536" alt="4  Pandas Scatter Plot Study Guide" src="https://github.com/user-attachments/assets/cded25ca-ed4a-47ea-b4d9-d5a08e760497" />
" alt="Pandas scatter plot study notes" width="800">
</p>

### 4. 📦 Pandas Box Plot

Understand distributions, medians, quartiles, interquartile range (IQR), and potential outliers.

<p align="center">
  <img src="<img width="1024" height="1536" alt="5  Pandas Box Plot Study Guide" src="https://github.com/user-attachments/assets/de98fb2d-ade9-4d67-8db8-991d56bfd80c" />
" alt="Pandas box plot study notes" width="800">
</p>

### 5. 🥧 Pandas Pie Plot

Visualize proportions, percentages, and category contributions to a whole.

<p align="center">
  <img src="<img width="1024" height="1536" alt="6  Pandas Pie Plot Study Cheat Sheet" src="https://github.com/user-attachments/assets/4126417b-9d79-4fef-9eb6-2632838547e7" />
" alt="Pandas pie plot study notes" width="800">
</p>

### 6. 🔥 Pandas Heatmap

Explore correlation matrices, numerical patterns, and relationships between variables using Seaborn.

<p align="center">
  <img src="<img width="1024" height="1536" alt="7  Pandas Heatmap Plot Study Infographic" src="https://github.com/user-attachments/assets/2171d21b-25fb-457a-b832-f87368cf6d54" />
" alt="Pandas heatmap study notes" width="800">
</p>

### 7. 🌈 Pandas Area Plot

Visualize magnitude, trends, and cumulative contributions using filled areas.

<p align="center">
  <img src="<img width="1024" height="1536" alt="8  Pandas Area Plot Notebook Cheat Sheet" src="https://github.com/user-attachments/assets/448658f8-045c-43f3-9185-fb6cb552465a" />
" alt="Pandas area plot study notes" width="800">
</p>

---

### 🚀 Practice and Explore

- Review the visual notes for each plot type.
- Practice the examples using your own CSV datasets.
- Customize titles, axis labels, colors, legends, and figure sizes.
- Apply data visualization techniques to exploratory data analysis (EDA).
- Explore how visualization supports data quality analysis and AI/ML testing.

**Keep learning. Keep practicing. Turn data into insights!** 📊



</p>
