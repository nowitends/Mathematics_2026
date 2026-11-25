# Exercise 12 - A Parameter Revealed by a Row Operation

## Question

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2 \leftarrow R_2 - 2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

## Solution

First, subtract twice the first row from the second row:

$$
R_2 \leftarrow R_2 - 2R_1
$$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}
$$

This row operation does not change the determinant because adding a multiple of one row to another leaves the determinant unchanged.

Now, expand the determinant along the second row:

$$
\det(A(t)) =
-(t-6)
\begin{vmatrix}
1 & 2 \\
0 & 1
\end{vmatrix}
$$

We get:

$$
\det(A(t)) = -(t-6)(1)
$$

Therefore:

$$
\det(A(t)) = 6-t
$$

A matrix is not invertible when its determinant is zero. Thus:

$$
6-t=0
$$

Solving for $t$ gives:

$$
\boxed{t=6}
$$

When $t=6$, the resulting matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 1
\end{pmatrix}
$$

The second row becomes a zero row.

In the original matrix, the second row is exactly twice the first row:

$$
R_2 = 2R_1
$$

Therefore, the rows are linearly dependent, which means that the determinant is zero and the matrix is not invertible.

## Conclusion

The matrix is not invertible when:

$$
\boxed{t=6}
$$

For this value of $t$, the second row is twice the first row. As a result, the rows are linearly dependent and the determinant is zero.

The row operation $R_2 \leftarrow R_2 - 2R_1$ does not change the determinant and reveals the special relationship between the rows.