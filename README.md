# sqlite_database_operations
HHA 504 Week 3 Assignment

## 1. Details on the datasets
  * The data sets utilized inlcuded a dataset from Stony Brook Hospital, proivded     by Professor Williams and a dataset found online from NY Presbyterian Hospital.     The NYP data set was utlized as many other familiar hopsitals were too large

## 2. Account of the exploratory data analysis process
  * Missing values and columns were deleted and all column names were brought to       simple format for both databases.
  * Basic Statistics were conducted for both databases, this included mean, median,   mode, standard deviation, IQR and others. .describe() was used.
  * Data distribution was viewed for both databases using histograms focused on one   column for each. For the StonyBrook Hospital, the column used was gross charge. For Presbyterian hospital, the maximum negotiated charges column was used. 

## 3. Instructions to replicate SQLite database setup
To fully view the code, please use this link: https://github.com/jward6301/sqlite_database_operations/blob/main/sqlite_database_operations.ipynb
  1.   Load in all necessary packages including Import pandas as pd, import sqlite3 and from sqlalchemy import create_engine
  2.   Create your database using the following code -  conn = sqlite3.connect('nameofyourdatabase.db') and c = conn.cursor()
  3.   To manually create the table, start with c.execute(""" and CREATE TABLE desired table name
  4.   Create columns for the table in the same cell
  5.   Confirm that the table was created properly
  6.   Create test or real rows in the table and use the insert into (table name) command
  7.   Create an engine to connect to SQLite db using create_engine
  8.   connect to pandas to look at the table and check all work using the following command pd.read_sql_query("select * from tablename;", conn)
  9.   To load previous csv or json files into the dataframe to input furhter information or replace all of the informatioon using df2.to_sql('stonybrookh_system', conn, if_exists='replace')


       
