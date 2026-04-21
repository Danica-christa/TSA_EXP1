# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 20/04/26

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
Name:Danica Christa
RegNo:212223240022
```
```
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("NFLX.csv")
data['Date'] = pd.to_datetime(data['Date'])
data.set_index('Date', inplace=True)
plt.figure(figsize=(10, 6))
plt.plot(data.index, data['Open'], label='Values', color='blue')
plt.title('Open_Value over Date')
plt.xlabel('Date')
plt.ylabel('Open_Value')
plt.grid(True)
plt.legend()
plt.show()
```
# OUTPUT:

<img width="1104" height="685" alt="image" src="https://github.com/user-attachments/assets/5bee826e-7b47-4261-b6b0-f008571f1eb0" />


# RESULT:
Thus we have created the python code for plotting the time series of given data.
