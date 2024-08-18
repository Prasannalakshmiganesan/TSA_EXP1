# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

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
```python
import pandas as pd
import matplotlib.pyplot as plt
data = pd.read_csv("Goodreadsbooks.csv", nrows=25)
data["publication_date"]=pd.to_datetime(data["publication_date"])
plt.plot(data['bookID'], data['publication_date'], label='Time Series Data')
plt.grid(True)
plt.title('Time Series Data Plot')
plt.xlabel('bookID')
plt.ylabel('publication_date')
plt.legend()
plt.show()
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/2b84445d-9be5-47ae-8cc8-c5418b8fc742)

# RESULT:
Thus we have created the Python code for plotting the time series of given data.

