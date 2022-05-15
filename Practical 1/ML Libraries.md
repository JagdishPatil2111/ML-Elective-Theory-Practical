#**Machine Learning Modules for Python**

#1. Numpy

Numpy is a python library for large multi-dimensional array and matrix processing, with the help of a large collection of high-level mathematical functions. It is very useful for fundamental scientific computations in Machine Learning. It is particularly useful for linear algebra, Fourier transform, and random number capabilities.

**Example of Numpy:**

import numpy as np
 
x = np.array([[1, 2], [3, 4]])
y = np.array([[5, 6], [7, 8]])
 
v = np.array([9, 10])
w = np.array([11, 12])
 
print(np.dot(v, w), "\n")
 
print(np.dot(x, v), "\n")
 
print(np.dot(x, y))

Output: 
219 

[29 67] 

[[19 22]
 [43 50]]
 
#2. Pandas
Pandas is a popular Python library for data analysis. It is not directly related to Machine Learning. As we know that the dataset must be prepared before training. In this case, Pandas comes handy as it was developed specifically for data extraction and preparation. It provides high-level data structures and wide variety tools for data analysis. It provides many inbuilt methods for groping, combining and filtering data. 

**Example of Pandas:**

import pandas as pd
 
data = {"country": ["Brazil", "Russia", "India", "China", "South Africa"],
       "capital": ["Brasilia", "Moscow", "New Delhi", "Beijing", "Pretoria"],
       "area": [8.516, 17.10, 3.286, 9.597, 1.221],
       "population": [200.4, 143.5, 1252, 1357, 52.98] }
 
data_table = pd.DataFrame(data)
print(data_table)

Output: 

      country       capital       area        population
 0    Brazil        Brasilia      8.516         200.40
 1    Russia        Moscow        17.100        143.50
 2    India        New Delhi      3.286         1252.00
 3    China         Beijing       9.597         1357.00
 4  South Africa    Pretoria      1.221         52.98
 
**Matplotlib**

Matplotlib is a very popular Python library for data visualization. Like Pandas, it is not directly related to Machine Learning. It particularly comes in handy when a programmer wants to visualize the patterns in the data. It is a 2D plotting library used for creating 2D graphs and plots. A module named pyplot makes it easy for programmers for plotting as it provides features to control line styles, font properties, formatting axes, etc. It provides various kinds of graphs and plots for data visualization, viz., histogram, error charts, bar chats, etc.

import matplotlib.pyplot as plt
import numpy as np
 
x = np.linspace(0, 10, 100)
 
plt.plot(x, x, label ='linear')
 
plt.legend()
 
plt.show()
