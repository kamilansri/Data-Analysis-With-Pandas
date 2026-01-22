# Mastering Pandas: Data Analysis in Python

This repository documents my journey learning **Pandas**, the premier Python library for data manipulation and analysis. It contains notebooks, scripts, and practice datasets exploring DataFrames, Series, and data cleaning techniques.

---

## 🐼 About Pandas
Pandas is an open-source library built on top of NumPy. It provides high-performance, easy-to-use data structures and data analysis tools for Python. It is the "Excel" of Python, allowing for complex data manipulation without the limitations of spreadsheet software.

---

## 🛠️ Key Concepts Covered

### 1. Data Structures
* **Series:** One-dimensional labeled arrays (like a column in a spreadsheet).
* **DataFrame:** Two-dimensional labeled data structures (like a full spreadsheet table).

### 2. Input/Output (I/O)
* Reading data from various sources: `.read_csv()`, `.read_excel()`, `.read_json()`, `.read_sql()`.
* Exporting cleaned data: `.to_csv()`, `.to_excel()`.

### 3. Data Inspection & Cleaning
* **Inspection:** Using `head()`, `tail()`, `info()`, and `describe()` to understand data.
* **Cleaning:** Handling missing values (`dropna()`, `fillna()`), removing duplicates, and renaming columns.
* **Type Conversion:** Changing data types using `.astype()`.

### 4. Data Manipulation
* **Selection:** Slicing data using `.loc[]` (label-based) and `.iloc[]` (index-based).
* **Filtering:** Conditional selection (e.g., `df[df['Age'] > 25]`).
* **Sorting:** Using `.sort_values()`.

### 5. Aggregation & Grouping
* **Split-Apply-Combine:** Using `.groupby()` to summarize data (mean, sum, count).
* **Pivot Tables:** Creating spreadsheet-style pivot tables.

---

## 💻 Code Examples

### Creating a DataFrame & Basic Inspection
```python
import pandas as pd

# Creating a DataFrame from a dictionary
data = {
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [24, 27, 22, 32],
    'City': ['New York', 'Los Angeles', 'Chicago', 'Houston']
}

df = pd.DataFrame(data)

# View first 5 rows
print(df.head())

# Get statistical summary
print(df.describe())
```
---
## 🔧 Installation

To run the notebooks in this repository, you need to install Pandas. It is also recommended to install `openpyxl` if you plan to work with Excel files.

```bash
# Install Pandas
pip install pandas

# Optional: Install support for Excel files
pip install openpyxl
```
---
## 📚 Resources

Here are some essential links and documentation I used while learning:

* **[Official Pandas Documentation](https://pandas.pydata.org/docs/)** – The comprehensive guide to all functions.
* **[10 Minutes to pandas](https://pandas.pydata.org/docs/user_guide/10min.html)** – The best official quickstart guide.
* **[Pandas Cheat Sheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)** – A handy PDF reference for common commands.
* **[Real Python Pandas Tutorials](https://realpython.com/search?q=pandas)** – In-depth articles and examples.
