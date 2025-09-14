# ECE22112_PA3: Python Data Analysis (Panda) 

## 💻 Problem 1
Using knowledge obtained from the experiment and demonstrations:

Load the corresponding .csv file into a data frame using pandas, and display the first five and last five rows of the resulting cars

## 🟢 Background
The steps:

1) Import Python Data Analysis (panda) in the notebook:
  
        import panda as pd

2) Load the corresponding file into a data frame named cars.csv using pd.read_csv:

        df = pd.read_csv('cars.csv')

3) Display the first five rows of the resulting cars using df.head():

        df.head(5)

4) Display the last five rows of the resulting cars using df.tail():

       df. tail(5)

5) Save the file as Surname_Pandas-P1.py

### 📌 Files
All the codes are done in this file. 
         
[Tormes_Pandas-P1.py](https://github.com/MychoTormes/ECE2112_PA3/blob/main/TORMES_Pandas-P1.py)

[Pandas Part 1](https://github.com/MychoTormes/ECE2112_PA3/blob/main/TORMES_Pandas-P1.ipynb)

### 📍 Reference

[Pandas cheat sheet](https://github.com/MychoTormes/ECE2112_PA3/blob/main/Pandas%20Cheat%20Sheet.pdf)

## 💻 Problem 2
Using the dataframe cars in problem 1, extract the following information using subsetting, slicing and indexing operations.

Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7…) of cars and the row that contains the ‘Model’ of ‘Mazda RX4’, find how many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have and determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.

## 🟢 Background
The steps:

1) Import Python Data Analysis (panda) in the notebook:

         import pandas as pd

2) Load the corresponding file into a data frame named cars.csv using pd.read_csv:
   
         pd.read_csv('cars.csv')

3) Display the first five rows into odd-numbered columns using .iloc() and .head():

         c = df.iloc[:,::2]
         xc = c.head(5)

5) Display the row that contains the ‘Model’ of ‘Mazda RX4’ using .iloc():

          c.iloc[[0], [0]]

6) Find the model 'Camaro Z28' and only display 'cyl' by using .loc():

          c.loc[(c['model'] == 'Camaro Z28'), ['cyl']]

7) Find the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ using .loc() and only display 'cyl' and 'gear':

           c.loc[[1,28,18], ['cyl', 'gear']]

### 📌 Files
All the codes are done in the file.

  [Tormes_Pandas-P2.py](https://github.com/MychoTormes/ECE2112_PA3/blob/main/TORMES_Pandas-P2.py)
  [Pandas Part 2]

### 📍 Reference

[Pandas Cheat Sheet](https://github.com/MychoTormes/ECE2112_PA3/blob/main/Pandas%20Cheat%20Sheet.pdf)

### The answers worked for this Programming Assignment are made by Mycho Tormes
