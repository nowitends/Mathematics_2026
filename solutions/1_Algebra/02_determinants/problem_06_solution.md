# Exercise 6 - Parameter and Invertibility

## Question

Given the matrix:

$$
A(t) = \begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
$$

Find all values of (t) for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

## Solution

### 1. Determinant of the Matrix

For a (2 \times 2) matrix, the determinant is calculated using the formula:

$$
\det(A) = ad - bc
$$

For the given matrix:

$$
A(t) = \begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
$$

The determinant is:

$$
\det(A(t)) = t \cdot t - 1 \cdot 2
$$

$$
\det(A(t)) = t^2 - 2
$$

### 2. Condition for Non-Invertibility

A square matrix is not invertible if and only if its determinant is equal to zero.

Therefore:

$$
\det(A(t)) = 0
$$

Substituting the determinant:

$$
t^2 - 2 = 0
$$

$$
t^2 = 2
$$

Taking the square root of both sides:

$$
t = \pm \sqrt{2}
$$

Thus:

$$
\boxed{t = \pm \sqrt{2}}
$$

### 3. Conclusion

The matrix is not invertible when its determinant is zero.

Therefore, the values of (t) for which the matrix is not invertible are:

$$
\boxed{t = -\sqrt{2} \quad \text{or} \quad t = \sqrt{2}}
$$

For all other real values of (t), the matrix is invertible because its determinant is nonzero.