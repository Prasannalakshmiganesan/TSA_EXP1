### Developed By: Prasannalakshmi G
### Reg No: 212222240075
###  Date: 
# Ex.No: 01A PLOT A TIME SERIES DATA

# AIM:
To Develop a python program to Plot a time series data (Books & their Publication year)
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Using pd.to_datetime we're coverting date/month/year to only year.
4. Plot the data according to need and can be altered yearly.
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

