# Exercise 1-Pandas-and-Numpy

1. Display the first 5 rows = data.head()
2. Display the last 5 rows = data.tail()
3. Check the number of rows and columns = data = 7009 rows x 21 columns
4. Use `info() to inspect the columns and data types.
   <class 'pandas.core.frame.DataFrame'>
RangeIndex: 7009 entries, 0 to 7008
Data columns (total 21 columns):
 #   Column            Non-Null Count  Dtype  
---  ------            --------------  -----  
 0   customerID        7009 non-null   object 
 1   gender            7009 non-null   object 
 2   SeniorCitizen     7009 non-null   int64  
 3   Partner           7009 non-null   object 
 4   Dependents        7009 non-null   object 
 5   tenure            7009 non-null   int64  
 6   PhoneService      7009 non-null   object 
 7   MultipleLines     7009 non-null   object 
 8   InternetService   7009 non-null   object 
 9   OnlineSecurity    7009 non-null   object 
 10  OnlineBackup      7009 non-null   object 
 11  DeviceProtection  7009 non-null   object 
 12  TechSupport       7009 non-null   object 
 13  StreamingTV       7009 non-null   object 
 14  StreamingMovies   7009 non-null   object 
 15  Contract          7009 non-null   object 
 16  PaperlessBilling  7009 non-null   object 
 17  PaymentMethod     7009 non-null   object 
 18  MonthlyCharges    7009 non-null   float64
 19  TotalCharges      7009 non-null   object 
 20  Churn             7009 non-null   object 
dtypes: float64(1), int64(2), object(18)

5. Use `describe() to summarize the numerical columns.

   	SeniorCitizen	tenure	MonthlyCharges
count	7009.000000	7009.000000	7009.000000
mean	0.161935	32.377372	64.746305
std	0.368417	24.556125	30.104056
min	0.000000	0.000000	18.250000
25%	0.000000	9.000000	35.450000
50%	0.000000	29.000000	70.350000
75%	0.000000	55.000000	89.850000
max	1.000000	72.000000	118.750000

   

# Exercise 2
1. Find the unique values in `Contract`.
   df1.nunique()
gender                 2
SeniorCitizen          2
Partner                2
Dependents             2
tenure                73
PhoneService           2
MultipleLines          3
InternetService        3
OnlineSecurity         3
OnlineBackup           3
DeviceProtection       3
TechSupport            3
StreamingTV            3
StreamingMovies        3
Contract               3
PaperlessBilling       2
PaymentMethod          4
MonthlyCharges      1583
TotalCharges        6500
Churn                  2
dtype: int64

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
Products:
1. PhoneService
2. MultipleLines
3. InternetService
4. OnlineSecurity
5. OnlineBackup
6. DeviceProtection
7. TechSupport
8. StreamingTV
9. StreamingMovies

Contracts
1. Month-to-month
2. One year
3. Two year

4. 
