# Exercise 1-Pandas-and-Numpy

1. Display the first 5 rows = data.head()
2. Display the last 5 rows = data.tail()
3. Check the number of rows and columns = data = 7009 rows x 21 columns
4. Use `info() to inspect the columns and data types.
   <class 'pandas.core.frame.DataFrame'>
RangeIndex: 7009 entries, 0 to 7008
Data columns (total 21 columns):
5. Use `describe() to summarize the numerical columns.

# Exercise 2
1. Find the unique values in `Contract`.
   df1.nunique()

2. Find the unique values in `Internet Service`.
   df1['InternetService'].unique()
   array(['DSL', 'Fiber optic', 'No']
   
3. Find the unique values in `Payment Method`.
   df1['PaymentMethod'].unique()
   array(['Electronic check', 'Mailed check', 'Bank transfer (automatic)',
       'Credit card (automatic)']

4. Find the minimum, maximum, and  average `MonthlyCharges`.
df1['MonthlyCharges'].min()
18.25
  
5. Find the minimum and maximum `tenure`.
df1['tenure'].min()
0

df1['tenure'].max()
72

**Business question:** What types of products and contracts are represented in the customer base, and what does a typical monthly charge look like?
