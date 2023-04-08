# Ex02-Outlier

You are given bhp.csv which contains property prices in the city of banglore, India. You need to examine price_per_sqft column and do following,

(1) Remove outliers using IQR 

(2) After removing outliers in step 1, you get a new dataframe.

(3) use zscore of 3 to remove outliers. This is quite similar to IQR and you will get exact same result

(4) for the data set height_weight.csv find the following

    (i) Using IQR detect weight outliers and print them

    (ii) Using IQR, detect height outliers and print them

#PROGRAM

Program import pandas as pd

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

#OUTPUT

![image](https://user-images.githubusercontent.com/119476060/230703572-b341947d-2427-42f9-970f-89b732395bd3.png)

![image](https://user-images.githubusercontent.com/119476060/230703575-dfdc0950-3ca6-4e6e-8bde-1f634f405f2a.png)

![image](https://user-images.githubusercontent.com/119476060/230703578-31e9314e-d9f9-4b3a-9df0-6bf8c4ec2fc9.png)

![image](https://user-images.githubusercontent.com/119476060/230703580-59d861f5-6162-4f70-94a5-c6ca29b7a340.png)

![image](https://user-images.githubusercontent.com/119476060/230703585-f164b813-643a-4298-a37e-b407e52fb4a1.png)

![image](https://user-images.githubusercontent.com/119476060/230703591-3751a03b-d407-42b3-8012-137ce3499ef1.png)

![image](https://user-images.githubusercontent.com/119476060/230703597-d31acacf-03c6-4e45-971f-0e3cef9c9752.png)

![image](https://user-images.githubusercontent.com/119476060/230703602-ea78faed-ee2b-45f1-b289-f1abc4b0f42a.png)

![image](https://user-images.githubusercontent.com/119476060/230703607-c0dfaed7-0d61-487a-9a3a-052fc36d8d5e.png)

![image](https://user-images.githubusercontent.com/119476060/230703614-5efbea84-8066-4f81-abf7-acd52195788b.png)

![image](https://user-images.githubusercontent.com/119476060/230703616-8627a248-7563-4f26-90bb-c98f22aac07f.png)

#RESULT

Thus we have read the given data and performed the univariate analysis with different types of plots.








