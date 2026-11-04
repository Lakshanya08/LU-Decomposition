# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
1. Import numpy and scipy.linalg.
2. Input the coefficient matrix A (and constants matrix B).
3. Compute the LU decomposition factors using lu() or lu_factor().
4. Print the resulting L and U matrices or solve for X using lu_solve().

## Program:
(i) To find the L and U matrix
 ```
'''Program to find L and U matrix using LU decomposition.
Developed by: LAKSHANYA.N
RegisterNumber: 212224230136
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: LAKSHANYA.N
RegisterNumber: 212224230136
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
```
## Output:
<img width="1375" height="725" alt="image" src="https://github.com/user-attachments/assets/71b0674b-7cb2-49b8-aa51-2e9efa2f8f46" />

<img width="1108" height="606" alt="image" src="https://github.com/user-attachments/assets/f43f572b-f2c3-4583-a971-36b8574ac7c2" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

