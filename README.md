# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```

import seaborn as sns
import matplotlib.pyplot as plt

df = sns.load_dataset("iris")
plt.figure(figsize=(8,5))
sns.histplot(df["sepal_length"], kde=True)
plt.title("Distribution of Sepal Length")
plt.show()

<img width="687" height="468" alt="output 1" src="https://github.com/user-attachments/assets/6ec6c1b7-2243-4f0b-853d-d567634e426e" />

sns.jointplot(x="sepal_length", y="sepal_width", data=df, height=6)
plt.show()
...

sns.pairplot(df, hue="species")
plt.show()
...
plt.figure(figsize=(8,6))
sns.heatmap(df.select_dtypes(include='number').corr(), 
            annot=True, cmap="coolwarm")
plt.title("Correlation Heatmap")
plt.show()
...
plt.figure(figsize=(8,5))
sns.boxplot(x="species", y="petal_length", data=df)
plt.title("Boxplot of Petal Length")
plt.show()
...
plt.figure(figsize=(8,5))
sns.violinplot(x="species", y="petal_width", data=df)
plt.title("Violinplot of Petal Width")
plt.show()
...
plt.figure(figsize=(6,4))
sns.countplot(x="species", data=df)
plt.title("Count of Species")
plt.show()
...
plt.figure(figsize=(8,5))
sns.barplot(x="species", y="sepal_length", data=df)
plt.title("Average Sepal Length")
plt.show()

```


# Result:
