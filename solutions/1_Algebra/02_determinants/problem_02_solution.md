#Exercise 2 - Determinant of a 3x3 Matrix

## Question

Given the matrix:

$$
A = \begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
$$

Compute $\det(A)$ using Sarrus’ rule. Then perform one simple check using a chosen property of the determinant.

## Solution

To calculate the determinant of this matrix, I will use Sarrus’ rule.

### 1. Calculation using Sarrus’ rule

First, I calculate the products of the diagonals going from top left to bottom right:

$$
1 \cdot 3 \cdot 5 + 2 \cdot 4 \cdot 2 + (-1) \cdot 0 \cdot 1
$$

$$
= 15 + 16 + 0 = 31
$$

Next, I calculate the products of the diagonals going from top right to bottom left:

$$
(-1) \cdot 3 \cdot 2 + 1 \cdot 4 \cdot 1 + 2 \cdot 0 \cdot 5
$$

$$
= -6 + 4 + 0 = -2
$$

Now, I subtract the second sum from the first sum:

$$
\det(A) = 31 - (-2)
$$

$$
\boxed{\det(A) = 33}
$$

### 2. Check using a determinant property

I will check the result using the row operation property. Adding a multiple of one row to another row does not change the determinant.

I apply the operation:

$$
R_3 \rightarrow R_3 - 2R_1
$$

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}
$$

Now, I expand the determinant along the first column:

$$
\det(A) = 1(3 \cdot 7 - 4 \cdot (-3))
$$

$$
= 21 + 12
$$

$$
= 33
$$

The result is the same as the one obtained using Sarrus’ rule, so the calculation is correct.

## Conclusion

The determinant of matrix A is 33. Both calculations give the same result, so the answer is verified.