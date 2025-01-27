# Pandas Tutorial

![Pandas Logo](https://pandas.pydata.org/static/img/pandas_logo.png)

This tutorial covers **Pandas**, a powerful data analysis and manipulation library in Python. Pandas provides data structures like Series and DataFrame that allow you to manipulate and analyze data efficiently. It is one of the most important tools for data scientists and analysts.

## Table of Contents

- [Introduction to Pandas](#introduction-to-pandas)
- [Series](#series)
- [DataFrames](#dataframes)
- [DataFrame Operations](#dataframe-operations)
- [Handling Missing Data](#handling-missing-data)
- [Data Selection and Filtering](#data-selection-and-filtering)
- [Merging, Joining, and Concatenating DataFrames](#merging-joining-and-concatenating-dataframes)
- [Grouping and Aggregating](#grouping-and-aggregating)
- [Handling Time Series Data](#handling-time-series-data)
- [Visualization](#visualization)

---

## Introduction to Pandas

Pandas is a powerful and flexible Python library for data manipulation. It allows you to manipulate large datasets, filter data, merge different data sources, and much more. Its two primary data structures are:
- **Series**: A one-dimensional array-like object.
- **DataFrame**: A two-dimensional tabular structure with rows and columns.

To install Pandas, you can run:
```bash
pip install pandas
Series

A Series is a one-dimensional labeled array, similar to a list or an array, but with more functionality. You can create a Series from a list, NumPy array, or dictionary.

Example:

import pandas as pd

# Create a Series
s = pd.Series([1, 2, 3, 4, 5])
print(s)


---

DataFrames

A DataFrame is a two-dimensional, size-mutable, and potentially heterogeneous tabular data structure with labeled axes (rows and columns).

Creating a DataFrame

You can create a DataFrame from a variety of data sources:

data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [24, 27, 22],
        'City': ['New York', 'Los Angeles', 'Chicago']}

df = pd.DataFrame(data)
print(df)

Accessing Data in DataFrame

You can access columns and rows in DataFrame using .loc[] and .iloc[].

Example:

# Access a column
print(df['Name'])

# Access a row by index
print(df.iloc[0])


---

DataFrame Operations

Once you have your DataFrame, you can perform various operations like sorting, filtering, adding/removing columns, etc.

Sorting Data

df_sorted = df.sort_values(by='Age')
print(df_sorted)

Adding a Column

df['Salary'] = [50000, 60000, 55000]
print(df)


---

Handling Missing Data

Pandas provides several methods to deal with missing data (NaN). You can fill missing data, drop it, or replace it.

Fill Missing Data

df['Age'] = df['Age'].fillna(df['Age'].mean())

Drop Missing Data

df.dropna(inplace=True)


---

Data Selection and Filtering

You can select data based on conditions using boolean indexing or .loc[] and .iloc[].

Filtering Rows

filtered_df = df[df['Age'] > 25]
print(filtered_df)


---

Merging, Joining, and Concatenating DataFrames

You can combine DataFrames in various ways using merge(), concat(), and join().

Merging DataFrames

df1 = pd.DataFrame({'Key': ['A', 'B', 'C'], 'Value1': [1, 2, 3]})
df2 = pd.DataFrame({'Key': ['A', 'B', 'D'], 'Value2': [4, 5, 6]})

merged_df = pd.merge(df1, df2, on='Key')
print(merged_df)

Concatenating DataFrames

concatenated_df = pd.concat([df1, df2], axis=0)
print(concatenated_df)


---

Grouping and Aggregating

You can group data based on certain criteria and perform aggregate functions like sum, mean, etc.

grouped = df.groupby('City')['Age'].mean()
print(grouped)


---

Handling Time Series Data

Pandas provides powerful tools to work with time series data.

Creating a Time Series

date_rng = pd.date_range(start='2023-01-01', end='2023-01-10', freq='D')
df_time = pd.DataFrame(date_rng, columns=['Date'])
print(df_time)


---

Visualization

Pandas integrates well with matplotlib for creating basic visualizations directly from a DataFrame.

df['Age'].plot(kind='line', title='Age Over Time')

This will generate a line plot of the 'Age' column.


---

Conclusion

This tutorial provided an in-depth overview of how to use Pandas for data manipulation and analysis. It covered essential topics such as Series, DataFrames, handling missing data, grouping data, and more. Pandas is a powerful tool that simplifies the process of working with structured data and is an essential part of the data science ecosystem.

For more information and advanced usage, visit the official Pandas documentation: https://pandas.pydata.org/

Feel free to experiment with the code examples and explore the possibilities of working with Pandas!

### How to Use:
- **Installation**: Make sure you have Pandas installed in your environment using `pip install pandas`.
- **Explore**: Use the code snippets and examples provided to explore the functionality of Pandas.
- **Practice**: Modify the code to fit your data needs and experiment with other methods available in Pandas.

Let me know if you need any further customization or adjustments!

