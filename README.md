# IndustrialNetwrok
This folder includes 14 csv files:

1-	location.csv
This file includes the location of 100 water tanks. The headers in this file are x and y, where (x,y) in row i represents the location of tank i.

2-	connection_matrix_inverse_distance.csv
This file represents the connection between the tanks. When there is no pipe between tank j and k, (j,k) value is zero. When there is a pipe between the tanks, (j,k) value is proportional to the inverse length of the pipe; shorter the pipe, larger the connection. 

3-	measurements_1.csv to measurements_12.csv
These files represent tanks time series measurements. The first column in the files represents time. Each tank has three variables:
  1)	Tank Pressurei is the pressure of tank i. This value can be between 0 and 100. 
  2)	Tanki Refill is a binary variable. Tanki Refill=1 when tank i is in the refill mode and Tanki Refill=0 otherwise.
  3)	Tanki Leak is a binary variable. Tanki Leak=1 when tank i is leaking, and Tanki Leak=0 when there is no leak in the tank. 
Therefore, the total number of variables in these files is 301. 

Please cite the follwoing paper when using the dataset.  
Hamed Khorasgani, Arman Hasanzade, Ahmed Farahat, and Chetan Gupta. "Fault Detection and Isolation in Industrial Networks
using Graph Convolutional Neural Networks." IEEE PHM 2019.
