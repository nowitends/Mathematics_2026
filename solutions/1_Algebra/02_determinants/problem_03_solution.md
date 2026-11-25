# Exercise 3 - Swapping Two Rows

## Question

Given the matrix:

$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

Compute $\det(A)$. Then form a matrix B by swapping the first and second rows of A.

First predict $\det(B)$ using a determinant property, and then verify your prediction by calculation.

## Solution

### 1. Calculation of the determinant of A

Using Sarrus’ rule:

$$
\det(A) = 1 \cdot 3 \cdot 1 + 2 \cdot 1 \cdot 2 + 0 \cdot 0 \cdot 1
$$

$$
= 3 + 4 + 0 = 7
$$

The products of the diagonals in the opposite direction are:

$$
0 \cdot 3 \cdot 2 + 2 \cdot 0 \cdot 1 + 1 \cdot 1 \cdot 1
$$

$$
= 0 + 0 + 1 = 1
$$

Therefore:

$$
\det(A) = 7 - 1 = 6
$$

### 2. Forming matrix B

By swapping the first and second rows of A, we obtain:

$$
B = \begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
$$

### 3. Prediction using a determinant property

When two rows of a matrix are swapped, the determinant changes its sign.

Therefore:

$$
\det(B) = -\det(A)
$$

$$
\det(B) = -6
$$

### 4. Verification by calculation

Using Sarrus’ rule for matrix B:

$$
\det(B) = 0 \cdot 2 \cdot 1 + 3 \cdot 0 \cdot 2 + 1 \cdot 1 \cdot 1
$$

$$
= 0 + 0 + 1 = 1
$$

The products of the diagonals in the opposite direction are:

$$
1 \cdot 2 \cdot 2 + 3 \cdot 1 \cdot 1 + 0 \cdot 0 \cdot 1
$$

$$
= 4 + 3 + 0 = 7
$$

Therefore:

$$
\det(B) = 1 - 7 = -6
$$

## Conclusion

The determinant of matrix A is 6.

After swapping the first and second rows, the determinant changes its sign.

Therefore, the determinant of matrix B is -6.

The calculated result confirms the prediction. This verifies that swapping two rows changes the sign of the determinant.