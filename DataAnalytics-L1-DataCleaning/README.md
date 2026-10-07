Data Cleaning: Cafe Sales Dataset

Overview:
The purpose of this project was to perform data cleansing on dirty data, which is a dataset containing 10,000 rows of data regarding sales at a cafe. Some of the issues which can arise from the data include missing data, poor data, wrong data type, and outliers.

Dataset:
Each record denotes one transaction at the café and includes the following information: Transaction ID, Name of the item, Quantity, Cost per unit, Total cost of the transaction, Mode of payment, and Date of the transaction.

Initial Dataset Problems:
From the initial data analysis, the number of missing values was 6,826 and those that were coded as ERROR and UNKNOWN were 3,256. Numerical variables had inappropriate data types assigned to them while there were invalid and missing values in the transaction date variable. There were no duplicate records but there were outliers in the Total Spent variable.

Data Cleaning Process:
To begin with, I imported the data set and examined the data types, missing values, unique values, and duplicate values. Secondly, I converted the ERROR and UNKNOWN values into missing values. Thirdly, I converted the Quantity, Price Per Unit, and Total Spent columns into numeric data type. The missing values for numeric data type columns were imputed using the median value, while for categorical data type columns the missing values were imputed using mode value. In case of dates, the Transaction Date column was converted into datetime data type and missing values were imputed using the most frequent date.

The Final Dataset:
The new dataset contains 10,000 records with eight variables without any missing or duplicate records. All the numeric variables contain appropriate data type while the date variable is also properly formatted.

Technology used in this project:
The project was created using Python through Jupyter Notebook, and the process of managing and cleaning the data involved Pandas and NumPy.