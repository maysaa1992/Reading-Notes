Reading Questions

Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation?

Pandas is a Python library used for working with data sets. It has functions for analysing, cleaning, exploring, and manipulating data.                                      

Pandas makes it simple to do many of the time consuming, repetitive tasks associated with working with data, including:

Data cleansing
Data fill
Data normalization
Merges and joins
Data visualization
Statistical analysis
Data inspection
Loading and saving data
                               

What are the primary data structures in Pandas, and how do they differ in terms of use cases?                                                                                                       The two main data structures in Pandas are Series for 1-D data and DataFrame for 2-D data. Data in higher dimensions are supported within DataFrame using a concept called hierarchical indexing. For storing axis labels of Series and DataFrame, the data structure used is Index                                                                                                                                                                                                            

Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?                                                                                                                                                                                                  

DataFrame: It is a two-dimensional table-like data structure with labeled rows and columns. DataFrames are suitable for analyzing and manipulating structured data, such as CSV files, SQL tables, or Excel sheets.
Series: It is a one-dimensional labeled array that can hold any data type. Series are useful for representing and working with single-column data or as the columns of a DataFrame. They provide additional functionality compared to regular arrays or lists.




## Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats?
To load a dataset into a DataFrame, Pandas provides functions like read_csv(), read_excel(), read_sql(), etc. Common file formats that can be used include CSV (Comma-Separated Values), Excel, JSON (JavaScript Object Notation), SQL databases, and more. For example, to load a CSV file named "data.csv" into a DataFrame, you can use the following code:
```import pandas as pd
df = pd.read_csv('data.csv')```