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
 Program for Univariate Linear Regression
 Developed by: Jeevanantham C
 Register Number: 25013725
 import numpy as np
 X=np.array([0,1,2,3,4,5,6,7,8,9])
 Y=np.array([1,3,2,5,7,8,8,9,10,12])
 X_mean=np.mean(X)
 Y_mean=np.mean(Y)
 num=0
 den=0
 for i in range(len(X)):
 num+=(X[i]-X_mean)*(Y[i]-Y_mean)
 den+=(X[i]-X_mean)**2
 m=num/den
 c=Y_mean-m*X_mean
 print(m,c)
  Y_pred=m*X+c
 print(Y_pred)





```
## Output
</br>
<img width="935" height="139" alt="{6DD290D2-BE05-4EF8-A3E2-2EAE57C1EEBD}" src="https://github.com/user-attachments/assets/c6d01b36-61e0-47e0-995d-0a7df4f2f204" />
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
