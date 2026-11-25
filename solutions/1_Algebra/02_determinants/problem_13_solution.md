# Exercise 13 - Determinant by Elimination

## Question

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

First, subtract twice the first row from the second row:

$$
R_2 \leftarrow R_2 - 2R_1
$$

This operation does not change the determinant because adding a multiple of one row to another leaves the determinant unchanged.

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix}
$$

Next, subtract the first row from the third row:

$$
R_3 \leftarrow R_3 - R_1
$$

This operation also does not change the determinant.

We get:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
\end{pmatrix}
$$

Now, add twice the second row to the third row:

$$
R_3 \leftarrow R_3 + 2R_2
$$

This operation also leaves the determinant unchanged.

The resulting matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}
$$

Now the matrix is upper triangular, so its determinant is the product of the diagonal entries:

$$
\det(A)=1\cdot1\cdot1
$$

Therefore:

$$
\boxed{\det(A)=1}
$$

Since all three row operations involved adding a multiple of one row to another, none of them changed the determinant.

Thus, the determinant of the original matrix is also 1.

## Conclusion

The determinant is:

$$
\boxed{\det(A)=1}
$$

All three row operations preserve the determinant because adding a multiple of one row to another does not change its value.

By using elimination, we transformed the original matrix into an upper triangular matrix, making the determinant easy to calculate by multiplying its diagonal entries.