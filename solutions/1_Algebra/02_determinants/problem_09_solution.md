# Exercise 9 - Area and the Determinant

## Question

The vectors are:

$$
u = \begin{pmatrix} 3 \\ 1 \end{pmatrix},
\quad
v = \begin{pmatrix} 1 \\ 4 \end{pmatrix}
$$

They span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

### 1. Calculating the Determinant

To calculate the area of the parallelogram, we use the determinant of the matrix formed by the two vectors:

$$
A = \begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}
$$

For a 2 × 2 matrix:

$$
\det(A) = ad - bc
$$

Substituting the values:

$$
\det(A) = 3 \cdot 4 - 1 \cdot 1
$$

$$
\det(A) = 12 - 1 = 11
$$

The area is the absolute value of the determinant:

$$
\text{Area} = |11| = 11
$$

### 2. Reversing the Order of the Vectors

After reversing the vectors, the matrix becomes:

$$
B = \begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}
$$

Its determinant is:

$$
\det(B) = 1 \cdot 1 - 3 \cdot 4
$$

$$
\det(B) = 1 - 12 = -11
$$

The new area is:

$$
\text{Area} = |-11| = 11
$$

### 3. Conclusion

Reversing the order of the vectors changes the sign of the determinant from 11 to -11.

However, the area does not change because it is always the absolute value of the determinant.

Therefore, the area of the parallelogram is 11 square units in both cases.