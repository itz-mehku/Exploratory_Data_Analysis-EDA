# Exploratory_Data_Analysis-EDA
## Mini Project 09: Select any dataset from UCI Dataset Repository and  Perform EDA

**Exploratory Data Analysis (EDA)** is a critical step in data science and analytics. It helps understand the dataset, detect patterns, spot anomalies, test hypotheses, and check assumptions using summary statistics and visualizations.

This Python script performs Exploratory Data Analysis (EDA) on a dataset of used cars. The goal is to understand the structure, detect anomalies, clean the data, and visualize relationships between different features.
## Dataset:
- File Name: used_cars_data.csv

- Description: Contains various details about used cars such as price, year, model, etc.
## Required Libraries:
- pandas

- numpy

- matplotlib

- seaborn
## Perfrom EDA:
### 1. Import Libraries

Libraries like `pandas`, `numpy`, `seaborn`, and `matplotlib` are imported for data handling and visualization.

### 2. Read Dataset

The dataset is read using `pd.read_csv()` and basic structure is explored using `.head()`, `.tail()`, `.shape`, `.columns`, `.dtypes`.

### 3. Summary Statistics

Key statistics are displayed using:

- `df.describe()`

- `df.info()`

- `df.nunique()`

### 4. Drop Irrelevant Columns

Columns not required for analysis like `Fuel_Type` are removed using `df.drop()`.

### 5. Rename Columns

The `Name` column is renamed to `Model` for clarity.

### 6. Handle Duplicates
   
Duplicate rows are identified using `df.duplicated()` and counted.

### 7. Handle Missing Values
   
Missing values are counted with `df.isnull().sum()` and dropped using `df.dropna()`.

### 8. Outlier Detection
   
A boxplot is used to detect outliers in the `Price` column.

### 9. Visualizations

- Histogram: Distribution of `Year`

- Scatter Plot: `Year` vs `Price`

- Line Plot: `Year` vs `Price`

- Heatmap: Correlation matrix of numerical features
