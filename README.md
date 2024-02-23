# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove 
outliers

# Coding and Output
```
import pandas as pd
df = pd.read_csv("SAMPLEIDS.csv")
(df)
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/298c22ea-2356-44a2-b9ca-6c9ee6c49788)

```
df.describe()
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/b1a256d4-d78b-4b3f-b9d6-bb646a707ff1)
```
df.info()
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/90f9c423-3ebc-458f-ab47-62397130c31f)
```
df.tail()
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/812d6a84-477c-46a3-b831-2b7442c48c5a)
```
df.shape
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/90b27198-bd5d-429f-bbf1-5eaac6c17695)
```
df.isnull().sum()
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/d17fd7c5-670c-4374-9143-fcabd9f1e684)
```
df.fillna(value=10)
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/d79cb2ac-90c9-4508-9c65-c0c92055f3a6)
```
df.fillna(method='ffill')
```
![image](https://github.com/DEEPAK2200233/exno1/assets/118707676/d3b37a20-81a7-4f49-8a18-1b19fa486184)

# Result
Thus,the given data is read,cleansed and the cleaned data is saved into the file.
