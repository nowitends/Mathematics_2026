# Exercise 3 – When Does the Inverse Not Exist?

## Question

For the matrix:

$$
A=\begin{pmatrix}
2&4\\
1&2
\end{pmatrix}
$$

Explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## Solution

### 1. Using the Determinant

For a $2\times2$ matrix:

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A)=(2)(2)-(4)(1)
$$

$$
=4-4=0
$$

Therefore:

$$
\boxed{\det(A)=0}
$$

Since the determinant is zero, the inverse does not exist.

### 2. Using Row Dependence

The first row is twice the second row:

$$
(2,4)=2(1,2)
$$

Therefore, the rows are linearly dependent.

A matrix with dependent rows is not invertible.

### 3. Conclusion

Both methods show that the inverse does not exist.

$$
\boxed{A^{-1}\text{ does not exist}}
$$