# Ex02-Outlier

You are given bhp.csv which contains property prices in the city of banglore, India. You need to examine price_per_sqft column and do following,

(1) Remove outliers using IQR 

(2) After removing outliers in step 1, you get a new dataframe.

(3) use zscore of 3 to remove outliers. This is quite similar to IQR and you will get exact same result

(4) for the data set height_weight.csv find the following

    (i) Using IQR detect weight outliers and print them

    (ii) Using IQR, detect height outliers and print them
   
   Program
   import pandas as pd
   
import numpy as np

import seaborn as sns

df=pd.read_csv('superstore.csv') df

df.head() df.info() df.describe() df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)

sns.countplot(x='Postal Code',data=df)

sns.distplot(df["Postal Code"])

sns.histplot(x='Postal Code',data=df)

Output
![image](https://user-images.githubusercontent.com/121303741/229697663-45beb065-7be0-40e5-a85f-493c531c303b.png)
![image](https://user-images.githubusercontent.com/121303741/229697716-1ff314ad-825e-4917-93be-2ac5986fcf12.png)
![image](https://user-images.githubusercontent.com/121303741/229697746-d319a3b5-05f7-40f5-8500-5b7dda533c9e.png)
![image](https://user-images.githubusercontent.com/121303741/229697777-885a3ac7-4095-450d-a4f8-a0b4b1dc965d.png)
![image](https://user-images.githubusercontent.com/121303741/229697813-5d2c136d-3367-4428-8b06-499df06d4735.png)
![image](https://user-images.githubusercontent.com/121303741/229697849-82f9be00-5e76-4e9c-8807-2ada9e2a73d8.png)
![image](https://user-images.githubusercontent.com/121303741/229697877-75166896-6669-45c4-9e77-2533dfc690f4.png)
![image](https://user-images.githubusercontent.com/121303741/229697919-9f8735e9-0b2c-4c04-97fc-db55e56a0a2f.png)
![image](https://user-images.githubusercontent.com/121303741/229697955-16de6bf5-aba1-48c7-bce3-661851923ec7.png)
![image](https://user-images.githubusercontent.com/121303741/229697980-6ffd4380-4554-4705-999b-26fc665f59c2.png)
![image](https://user-images.githubusercontent.com/121303741/229698010-4f32c9c2-49ad-4870-9515-9f4ae944acd0.png)

RESULT
Thus we have read the given data and performed the univariate analysis with different types of
plots.
