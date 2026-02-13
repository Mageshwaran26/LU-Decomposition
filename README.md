# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the input matrix (and right-hand side vector for solving equations) from the user.
2. Convert the given input into a NumPy array.
3. Apply LU decomposition to factorize the matrix into Lower triangular matrix (L) and Upper triangular matrix (U).
4. Display the L and U matrices, and if required, solve the system of linear equations using the decomposed matrices.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Mageshwaran T.A
RegisterNumber: 212224230146
'''
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
Developed by: Mageshwaran T.A
RegisterNumber: 212224230146
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
```

## Output:
(i)
<img width="1199" height="461" alt="Screenshot 2026-02-07 082051" src="https://github.com/user-attachments/assets/48288404-f165-4ca0-a604-eb725834bbbc" />
(ii)
<img width="892" height="198" alt="Screenshot 2026-02-07 082113" src="https://github.com/user-attachments/assets/59d3e3a3-60ef-4fc2-958d-a48be7264fc7" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

