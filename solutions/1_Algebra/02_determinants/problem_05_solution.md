# Exercise 5 - Row Operations

## Question

Given the matrix:

$$
A = \begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

Find $\det(A)$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

### 1. Initial Matrix

The given matrix is:

$$
A = \begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

I will use row operations to transform the matrix into an upper triangular matrix.

Adding a multiple of one row to another row does not change the determinant.

### 2. First Row Operation

Apply the operation:

$$
R_2 \rightarrow R_2 - 2R_1
$$

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
$$

The determinant does not change because adding a multiple of one row to another row leaves the determinant unchanged.

### 3. Second Row Operation

Apply the operation:

$$
R_3 \rightarrow R_3 + R_1
$$

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
$$

The determinant does not change because this is also a row replacement operation.

### 4. Third Row Operation

Apply the operation:

$$
R_3 \rightarrow R_3 + 2R_2
$$

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
$$

The determinant does not change because adding a multiple of one row to another row preserves the determinant.

### 5. Calculating the Determinant

The matrix is now upper triangular.

The determinant of an upper triangular matrix is the product of its main diagonal entries.

Therefore:

$$
\det(A) = 1 \cdot (-3) \cdot (-7)
$$

$$
\boxed{\det(A) = 21}
$$

## Conclusion

The determinant of the given matrix is 21.

All three row operations involved adding a multiple of one row to another row, so the determinant remained unchanged at every step.

The final upper triangular matrix gives the determinant by multiplying its main diagonal entries.