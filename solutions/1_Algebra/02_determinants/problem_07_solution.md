# Exercise 7 - Using Properties Instead of Recomputing

## Question

Suppose that for a (3 \times 3) matrix:

$$
\det(A) = -4
$$

Compute:

$$
\det(2A), \quad \det(A^T), \quad \det(A^2), \quad \det(-A)
$$

Justify each answer using the appropriate property.

Solution

### 1. Determinant of (2A)

For an (n \times n) matrix, multiplying the matrix by a scalar (k) multiplies its determinant by (k^n).

Since (A) is a (3 \times 3) matrix:

$$
\det(2A) = 2^3 \det(A)
$$

Substituting the given determinant:

$$
\det(2A) = 8 \cdot (-4)
$$

$$
\boxed{\det(2A) = -32}
$$

### 2. Determinant of the Transpose

The determinant of a matrix is equal to the determinant of its transpose.

Therefore:

$$
\det(A^T) = \det(A)
$$

Since:

$$
\boxed{\det(A^T) = -4}
$$

### 3. Determinant of (A^2)

Using the determinant property for matrix multiplication:

$$
\det(AB) = \det(A) \cdot \det(B)
$$

Since \(A^2\) means \(A \cdot A\):

$$
\det(A^2) = \det(A) \cdot \det(A)
$$

$$
\det(A^2) = (-4) \cdot (-4)
$$

$$
\boxed{\det(A^2) = 16}
$$

### 4. Determinant of (-A)

For an (n \times n) matrix:

$$
\det(kA) = k^n \det(A)
$$

Since (A) is a (3 \times 3) matrix:

$$
\det(-A) = (-1)^3 \det(A)
$$

Substituting:

$$
\det(-A) = (-1) \cdot (-4)
$$

$$
\boxed{\det(-A) = 4}
$$

Conclusion

The results are:

$$
\boxed{
\begin{aligned}
\det(2A) &= -32 \\
\det(A^T) &= -4 \\
\det(A^2) &= 16 \\
\det(-A) &= 4
\end{aligned}
}
$$

Each result was obtained using determinant properties without calculating the determinant from scratch.