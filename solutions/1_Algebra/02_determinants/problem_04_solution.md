# Exercise 4 - Triangular Matrix

## Question

Given the matrix:

$$
A = \begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
$$

Compute the determinant without expanding it. State the rule for an arbitrary triangular matrix and explain it using this example.

## Solution

### 1. Determinant of the Matrix

The given matrix is an upper triangular matrix because all entries below the main diagonal are zero.

For a triangular matrix, the determinant is equal to the product of its main diagonal entries.

Therefore:

$$
\det(A) = 2 \cdot (-3) \cdot 7
$$

$$
\det(A) = -6 \cdot 7
$$

$$
\boxed{\det(A) = -42}
$$

### 2. General Rule for Triangular Matrices

The determinant of any upper or lower triangular matrix is equal to the product of its main diagonal entries.

For an upper triangular matrix:

$$
A = \begin{pmatrix}
a_{11} & * & * \\
0 & a_{22} & * \\
0 & 0 & a_{33}
\end{pmatrix}
$$

For a lower triangular matrix:

$$
A = \begin{pmatrix}
a_{11} & 0 & 0 \\

* & a_{22} & 0 \\
* & * & a_{33}
    \end{pmatrix}
    $$

In both cases, the determinant is:

$$
\det(A) = a_{11} \cdot a_{22} \cdot a_{33}
$$

In this example, the diagonal entries are 2, -3 and 7. Their product gives -42.

## Conclusion

The determinant of the given upper triangular matrix is -42.

This example confirms that the determinant of a triangular matrix is the product of its main diagonal entries. No determinant expansion is needed.