# Matrix-Problem

## Scenario
### Imagine you have a matrix represented asa numpy array, and your task is to find the sum of its diagonal elements using a loop.

## CODE:
```python
import numpy as np

n = int(input("Enter the order of the matrix (n x n): "))

matrix = np.zeros((n, n))

print(f"Enter the values for the {n}x{n} matrix:")
for i in range(n):
for j in range(n):
matrix[i, j] = float(input(f"Enter element at position ({i+1},{j+1}): "))

diagonal_sum = 0
for i in range(n):
diagonal_sum += matrix[i, i]

print("The sum of the diagonal elements is:", diagonal_sum)

OUTPUT:

Enter the order of the matrix (n x n): 2
Enter the values for the 2x2 matrix:
Enter element at position (1,1): 1
Enter element at position (1,2): 45
Enter element at position (2,1): 67
Enter element at position (2,2): 6
The sum of the diagonal elements is: 7.0




