# Exercise 11 - Shortening the Calculation with Row Operations

## Question

Compute

$$
\det\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## Solution

First, subtract the first row from the second and third rows:

$$
R_2 \leftarrow R_2 - R_1
$$

$$
R_3 \leftarrow R_3 - R_1
$$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}
$$

Next, subtract twice the second row from the third row:

$$
R_3 \leftarrow R_3 - 2R_2
$$

We get:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}
$$

These row operations do not change the determinant because adding a multiple of one row to another leaves the determinant unchanged.

Now the matrix is upper triangular, so its determinant is the product of the diagonal entries:

$$
\det(A) = 1 \cdot 1 \cdot 1 = 1
$$

Therefore:

$$
\boxed{\det(A) = 1}
$$

## Conclusion

The determinant is 1.

Adding a multiple of one row to another does not change the determinant. Using these operations makes the calculation shorter by creating zeros below the diagonal.