# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: rohith r
Register number: 212222230121

import numpy as np
import matplotlib.pyplot as py
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num,denom=0,0
for i in range(len(x)):
  num+=(x[i]-x_mean)*(y[i]-y_mean)
  denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-(m*x_mean)
print(m,b) 
y_pred=(m*x)+b
print(y_pred)
py.scatter(x,y,color='blue')
py.plot(x,y_pred,color="#CD5555")
py.show()






```
## Output
![244587754-d8973240-1a41-431f-bd9a-683cc8dfc3e0](https://github.com/Rohithravi333/Univariate-Linear-Regression/assets/119394126/83497680-fdb2-425f-8a1e-5bf3b201e5d0)

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
