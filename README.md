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
 ![WhatsApp Image 2026-03-13 at 12 05 07 PM](https://github.com/user-attachments/assets/638d162d-be6f-4cf8-be72-c2665b845ec4)
![WhatsApp Image 2026-03-13 at 12 05 10 PM](https://github.com/user-attachments/assets/b5b0d697-5cb7-40ba-bef1-ecfc0d3b1d34)
![WhatsApp Image 2026-03-13 at 12 05 12 PM (1)](https://github.com/user-attachments/assets/7c2e9ef1-d819-46a5-b24f-78474b490ff8)
![WhatsApp Image 2026-03-13 at 12 05 11 PM](https://github.com/user-attachments/assets/541b78ac-9b58-4664-a045-0b4c03182a48)
![WhatsApp Image 2026-03-13 at 12 05 12 PM](https://github.com/user-attachments/assets/985086fc-1f38-477f-b804-d125adcff31e)
![WhatsApp Image 2026-03-13 at 12 05 14 PM (1)](https://github.com/user-attachments/assets/1b917e5c-1d50-4b7f-8adc-62161c476886)
![WhatsApp Image 2026-03-13 at 12 05 14 PM (2)](https://github.com/user-attachments/assets/43d0c98a-8e69-42c9-8e62-2c3c381f3e11)
![WhatsApp Image 2026-03-13 at 12 05 14 PM](https://github.com/user-attachments/assets/ebda81b4-e4e9-4757-b090-19f6e15ce5d4)
