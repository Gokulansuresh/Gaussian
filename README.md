# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. ​Augmented Matrix Setup: Initializes an n \times (n+1) matrix a to store coefficients alongside the constant vector.  
2. Forward Elimination: Converts the coefficient matrix into upper triangular form by subtracting row ratios (ratio = a[j][i] / a[i][i]) from lower rows.  
3. Back Substitution: Solves for unknown variables x sequentially in reverse order, starting from x_{n-1} down to x_0.  
4. ​Output Display: Prints each computed variable X_i rounded to 2 decimal places.

## Program
### ```Program to solve a matrix using Gaussian elimination without partial pivoting.
### Developed by:GOKULAN.S.S 
### RegisterNumber: 26018286
###   import os
### os.environ["OPENBLAS_NUM_THREADS"]="1"
### import numpy as np
### import sys
### n=int(input())

### a = np.zeros((n,n+1))
### x = np.zeros(n)
### for i in range(n):
###     for j in range(n+1):
###       a[i][j] = (input())
### for i in range(n):
###    if a[i][i] == 0.0:
###        sys.exit("divide by zero detected!")
###    for j in range(i+1,n):
###        ratio = a[j][i]/a[i][i]
###        for k in range(n+1):
###            a[j][k] = a[j][k]-ratio * a[i][k]
### x[n-1] = a[n-1][n]/a[n-1][n-1]  
### for i in range(n-2,-1,-1):
###   x[i] = a[i][n]
###     for j in range(i+1,n):
###        x[i] = x[i]-a[i][j] * x[j]
###    x[i]= x[i]/a[i][i]
### for i in range(n):
###     print("X%d = %0.2f"%(i,x[i]),end=' ') ```

## Output:
![gaussian elimination]()
<img width="910" height="856" alt="image" src="https://github.com/user-attachments/assets/b9fca693-f453-4c9a-aaba-e314fa4427b8" />


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

