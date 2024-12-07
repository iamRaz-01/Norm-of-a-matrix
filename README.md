# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. **Input the Matrix**:  
   - Accept a 2D array from the user using `eval(input())` and convert it into a NumPy array using `np.array()`.

2. **Compute Matrix Norms**:  
   - **1-Norm**: Use `np.linalg.norm(mat, 1)` to calculate the 1-norm (maximum absolute column sum).  
   - **2-Norm**: Use `np.linalg.norm(mat, 2)` to calculate the 2-norm (largest singular value).  
   - **Infinity Norm**: Use `np.linalg.norm(mat, np.inf)` to calculate the infinity norm (maximum absolute row sum).

3. **Format Results**:  
   - Format all norms (1-norm, 2-norm, and infinity norm) to two decimal places using strings or f-strings.

4. **Output Results**:  
   - Print the formatted values of the 1-norm, 2-norm, and infinity norm separately.

5. **End the Program**.  
---

This combined approach will allow you to compute and display the 1-norm, 2-norm, and infinity norm of a matrix. Would you like the implementation code for this?
## Program:
```Python
# Register No: 24002896
# Developed By: Abdul Rasak N 
# 1-Norm of a Matrix

import numpy as np 
mat = np.array (eval(input()))
ans = np.linalg.norm(mat,1)
norm = "{:.2f}".format(ans)
print(norm)

# 2-Norm of a Matrix

import numpy as np
mat = np.array(eval(input()))
ans = np.linalg.norm(mat,2)
print(f'{ans:.2f}')

# Infinity Norm of a Matrix

import numpy as np 
mat = np.array(eval(input()))
res = np.max(np.sum(np.abs(mat),axis = 1 ))
print(f'{res:.2f}')


```
## Output:
### 1-Norm of a Matrix
![image](https://github.com/user-attachments/assets/1814526d-8c33-45ec-b09e-588d4421bed2)


### 2-Norm of a Matrix
![image](https://github.com/user-attachments/assets/23242a62-5ee4-4c64-b759-b47b22410e9c)


### Infinity Norm of a Matrix
![image](https://github.com/user-attachments/assets/f8444d0f-7d31-4644-a5c2-db012369b5c0)

## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
