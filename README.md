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
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
## Line Plot:
```
import matplotlib.pyplot as plt
x_value =[0,1,2,3,4,5]
y_value = [0,1,4,9,16,25]
plt.plot(x_value,y_value)
plt.show()
```
## Output:
![output 1](https://github.com/user-attachments/assets/8cbc6427-1911-4767-978b-a2bb3a660d75)

## Scatter Plot:
```
import matplotlib.pyplot as plt


x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

y = [2, 4, 5, 7, 6, 8, 9, 11, 12, 12]

plt.scatter(x, y, label="stars", color="green", marker="*", s=30)

plt.xlabel('x axis')


plt.ylabel('y axis')

plt.title('My scatter plot!')

plt.legend()

plt.show()
```
## Output:
![output 2](https://github.com/user-attachments/assets/e8a4b829-22ae-4a7f-b333-a321448f4d2d)

## Pie Chart:
```
import matplotlib.pyplot as plt

activities = ['eat', 'sleep', 'work', 'play']

slices = [3, 7, 8, 6]

colors = ['r', 'y', 'g', 'b']

plt.pie(slices, labels=activities, colors=colors,
        startangle=90, shadow=True, explode=(0, 0, 0.1, 0),
        radius=1.2, autopct='%1.1f%%')


plt.legend()


plt.show()
```
## Output:
![output 3](https://github.com/user-attachments/assets/669dda9f-8b2e-4614-97b2-6719537ee802)

## Area Chart:
```
import matplotlib.pyplot as plt
import numpy as np


x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]


plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.legend(['y1', 'y2'])
plt.show()
```
## Output:
![image](https://github.com/user-attachments/assets/e4052d98-6ded-4d26-9ca0-18955f152a61)

## Bar Chart:
```
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]

names = ['one', 'two', 'three', 'four', 'five']

c1 = ['red', 'green']
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x axis')

plt.ylabel('y axis')

plt.title('My bar chart!')

plt.show()
```
## Output:
![image](https://github.com/user-attachments/assets/a8933616-c0d5-4d12-ac77-5826c5ee90b2)

## Histogram:
```
import matplotlib.pyplot as plt

x = [2, 1, 6, 4, 2, 4, 8, 9, 4, 2, 4, 10, 6, 4, 5, 7, 7, 3, 2, 7, 5, 3, 5, 9, 2, 1]

plt.hist(x, bins=10, color='blue', alpha=0.5)
plt.show()
```
## Output:
![image](https://github.com/user-attachments/assets/8071ebd1-faf0-4f7a-a1f4-85026e67e15c)

## Box Plot:
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
## Output:
![output 7](https://github.com/user-attachments/assets/243a2da2-54b6-43a0-a251-64ce451ea3d2)
![image](https://github.com/user-attachments/assets/1069d9e5-c718-4b36-9f6e-af8cb6f05199)

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
