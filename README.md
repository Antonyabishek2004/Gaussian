# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. First,we want to import numpy,then import sys,assume a variable
2. For gaussian method,we want to make 2nd and 3rd column zero
3. For that we want to make a range according to your output
4. Then print the program with the correct form then the output will display


## Program:
'''Program to solve a matrix using Gaussian elimination without partial pivoting. Developed by: ANTONY ABISHEK K RegisterNumber: 212223240009 ''' import numpy as np import sys n=int(input()) a=np.zeros((n,n+1)) x=np.zeros(n) for i in range(n): for j in range(n+1): a[i][j]=float(input()) for i in range(n): if a[i][j]==0.0: sys.exit('Divide by zero detected!') for i in range(n): for j in range(i+1,n): ratio = a[j][i]/a[i][i] for k in range(n+1): a[j][k] = a[j][k] - ratio * a[i][k] x[n-1]=a[n-1][n]/a[n-1][n-1] for i in range(n-2,-1, -1): x[i]=a[i][n] for j in range(i+1,n): x[i]=x[i]-a[i][j]*x[j] x[i]=x[i]/a[i][i] for i in range(n): print('X%d = %0.2f' % (i,x[i]),end=' ')

## Output:
![image](https://github.com/Antonyabishek2004/Gaussian/assets/138849620/4486b5f8-114b-495c-939b-b9760a6deb77)
![EX NO 6 AI  2](https://github.com/Antonyabishek2004/Gaussian/assets/138849620/69b237cf-62bd-454d-8f72-3efb0b4c9459)




## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

