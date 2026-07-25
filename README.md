# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 23/07/2026

# AIM:
To develop a Python program to plot time series data using the House Price dataset and visualize the average house prices over different years.
# ALGORITHM:
1. Import the required libraries such as Pandas and Matplotlib.
2. Read the dataset using the read_csv() function.
3. Display the first few and last few records of the dataset.
4. Check the dataset information using the info() function.
5. Group the data by YearBuilt and calculate the mean of the Price column.
6. Plot the time series graph using Matplotlib.
7. Add the graph title, X-axis label, Y-axis label, and grid.
8. Display the graph.

# PROGRAM:
### Name:  THARUN  D
### Reg.No: 212223240167
```
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("House_Price.csv")
df.head()
```
<img width="750" height="200" alt="image" src="https://github.com/user-attachments/assets/7005be40-e20e-402b-a666-d50e1eee196e" />

```
df.tail()
```
<img width="731" height="185" alt="image" src="https://github.com/user-attachments/assets/490b83ca-d95f-4081-8561-72cfaa80f15f" />


```
df.info()
```
<img width="575" height="339" alt="image" src="https://github.com/user-attachments/assets/5e8a01b5-b7b8-4e27-b8b8-a10946afcc99" />


```
df.groupby("YearBuilt")["Price"].mean().plot(figsize=(10,5))

plt.title("House Price Trend")
plt.xlabel("Year")
plt.ylabel("Price")
plt.grid(True)

plt.show()
```

<img width="818" height="492" alt="image" src="https://github.com/user-attachments/assets/d6a7227c-9885-4e44-a750-b2ef0ea8dadb" />



# RESULT:
Thus we have created the python code for plotting the time series of given data.
