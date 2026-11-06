# Python Stats Analyzer

A dependency-free command-line tool that computes descriptive statistics for any column of a tab-separated file. It skips non-numeric and `NaN` values and reports what it skipped.

![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white) ![No dependencies](https://img.shields.io/badge/dependencies-none-brightgreen)

## ✨ Features

* **Descriptive statistics:** count, number of valid values, mean, median, min, max, sample variance and standard deviation.
* **Data validation:** skips non-numeric and `NaN` entries and prints the line number of each skipped value.
* **Clear failures:** prints a helpful message for a missing file or an invalid column index, and exits with code 2 when a column has no numeric data.
* **Pure Python:** implemented with only `sys` and `math`, without NumPy or pandas.

## 🚀 Usage

```bash
python stats_in_python.py <file> <column_index>
```

`column_index` is zero-based. For example:

```bash
python stats_in_python.py data_file.txt 3
```

```
    Column: 3

        Count = 125
        ValidNum = 125
        Average = 57.44
        Maximum = 97.0
        Minimum = 16.0
        Variance = 308.49
        Std Dev = 17.564
        Median = 58.0
```

## 🧪 Sample Data

| File | Purpose |
| :--- | :--- |
| `data_file.txt` | Clean numeric data (125 rows) |
| `data_file2.txt` | The same data with `NaN` values mixed in |
| `data_file3.txt` | A malformed file with text and empty fields, for checking error handling |

## 👤 Author

**Aditya Daware** · [LinkedIn](https://www.linkedin.com/in/aditya-daware) · [GitHub](https://github.com/Adidaware)
