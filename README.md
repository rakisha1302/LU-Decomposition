# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2.Import the necessary libraries(numpy,scipy.linalg)
3.Define the matrix using numpy
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program


## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by:RAKISHA.R
RegisterNumber:212225230223
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:RAKISHA.R
RegisterNumber:212225230223 
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```

## Output:
<img width="1321" height="572" alt="image" src="https://github.com/user-attachments/assets/85225c69-be9d-4ff0-9131-224be3445c17" />

**<img width="1300" height="330" alt="image" src="https://github.com/user-attachments/assets/85d38779-bf3b-4f05-9e2c-8a0943266470" />
**

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

