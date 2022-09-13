# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
Program Developed By : Mirudhula D

Register number : 212221230060

import pandas as pd
df = pd.read_csv('Data_set.csv')
df.head(10)
df.info()
df.tail()
df.isnull().sum()
df['show_name']=df['show_name'].fillna(df['show_name'].mode()[0])
df['aired_on']=df['aired_on'].fillna(df['aired_on'].mode()[0])
df['original_network']=df['original_network'].fillna(df['original_network'].mode()[0])
df.head()
df['rating']=df['rating'].fillna(df['rating'].mean())
df['current_overall_rank']=df['current_overall_rank'].fillna(df['current_overall_rank'].mean())
df.head()
df['watchers']=df['watchers'].fillna(df['watchers'].median())
df.head()
df.info()
df.isnull().sum()






# OUPUT
# DATASET
![image](https://user-images.githubusercontent.com/94828147/189966383-687e4f5c-20c8-4521-bf78-f0ee41f1f076.png)

# HEAD:
![image](https://user-images.githubusercontent.com/94828147/189966620-a3c3f7e9-1880-4590-b4d5-cee3bfb2c937.png)

# DESCRIBE:
![image](https://user-images.githubusercontent.com/94828147/189966766-a5143ea3-2881-44a6-bf51-66737d439196.png)

# PRE-CLEANING INFORMATION:
![image](https://user-images.githubusercontent.com/94828147/189967166-7cee1cf2-8b61-4cab-a3b4-b80a0e3e4556.png)

# TAIL:
![image](https://user-images.githubusercontent.com/94828147/189967392-71dee6af-1a0c-4f4a-9349-0cbdd3db6ba5.png)
  
# SHAPE
![image](https://user-images.githubusercontent.com/94828147/189967744-d343b4f9-e58f-4ef3-bb2a-1debf9b4f823.png)

# COLUMN:
![image](https://user-images.githubusercontent.com/94828147/189967851-518d14fe-a336-4c76-a129-7e93fb80ed32.png)

# PRE-CLEANING SUM:
![image](https://user-images.githubusercontent.com/94828147/189967980-73a8ae34-be98-410a-b8cf-4472d320663f.png)

# DUPLICATE:
![image](https://user-images.githubusercontent.com/94828147/189968127-4f62dc3a-d6e8-483b-bf62-d179c7a6cea3.png)

# SNS PLOT:
![image](https://user-images.githubusercontent.com/94828147/189968248-e96a3c22-c78c-4932-8054-02a7e5767890.png)

# POST-CLEANING SUM:
![image](https://user-images.githubusercontent.com/94828147/189968371-493b8a14-16f3-4c4a-9a34-7a2bc276311a.png)

# POST CLEANING INFORMATION:
![image](https://user-images.githubusercontent.com/94828147/189968853-29309f2d-9dc5-4a5e-b868-0ea1f8f4bb82.png)



# RESULT:
The given data is read and data cleaning is performed and the cleaned data is saved to a file.


 

