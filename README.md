# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Initialize ( L ) as identity and ( U ) as zero matrices.
2. For each row ( i ), compute ( U[i, j] ) for ( j \geq i ).
3. Compute ( L[j, i] ) for ( j > i ) using the formula for ( L[j, i] ).
4. Return ( L ) and ( U ) such that ( A = L \cdot U ).


## Program:
'''Program to find L and U matrix using LU decomposition.
Developed by: ROHITH J
RegisterNumber: 212224230232
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

'''Program to solve a matrix using LU decomposition.
Developed by: ROHITH J
RegisterNumber: 212224230232
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
piv,lu=lu_factor(A)
result=lu_solve((piv,lu),B)
print(result)

## Output:
![alt text](<Screenshot 2025-05-10 233600.png>)
![alt text](<Screenshot 2025-05-10 233641.png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

