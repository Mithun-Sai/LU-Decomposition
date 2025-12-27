# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

(i) To find the L and U matrix:

1.Import required libraries: numpy for array handling and scipy's lu function for decomposition.

2.Read matrix input as a string via input(), evaluate it to create a numpy array A.​

3.Call lu(A) to compute P (permutation), L (lower triangular with 1s on diagonal), and U (upper triangular).

4.Print L followed by U.

(ii) To find the LU Decomposition of a matrix:

1.Import libraries

2.Read and build matrix A

3.Read and build vector/matrix B

4.Compute LU factorization of A

5.Solve the linear system using the LU factors

6.Output the solution

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Mithun Sai P
RegisterNumber: 25008604
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
Developed by: Mithun Sai P
RegisterNumber: 25008604
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A=np.array(eval(input()))
B=np.array(eval(input()))

lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)

print(x)
```

## Output:

<img width="1063" height="584" alt="image" src="https://github.com/user-attachments/assets/900890ac-1e81-4f5b-9e6f-6da2447365a2" />

<img width="939" height="379" alt="image" src="https://github.com/user-attachments/assets/d6edeae3-afe7-4f1e-a3eb-98f9f735b845" />

<img width="1067" height="583" alt="image" src="https://github.com/user-attachments/assets/e439db1f-8afb-4909-a0c6-f8ebba5b70b1" />

<img width="901" height="203" alt="image" src="https://github.com/user-attachments/assets/22d49dd4-5e60-471b-a06f-5e499e8504bb" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

