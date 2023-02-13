# Booston_house_dataset-using-pandas-library
booston house dataset analysis with pandas library
import pandas as pd
df= pd.read_csv("/content/drive/MyDrive/train/Boston.csv")
df

#Imputation of missing values.
df.isnull().sum()

#checking the no. of rows and columns
df.shape

#analysis the datatypes of the attributes
df.dtypes

#Descriptive Statistics summary of attributes
df.describe()

#Retrieve columns indexing value
df.iloc[1:10,:]

#Retrieve columns by column names 
df.loc[:,['CRIM','INDUS', 'AGE', 'TAX']]

#Removing the columns having the maximum missing values
df.drop(["Unnamed: 15","Unnamed: 16"], axis= 1,inplace=True)
df
