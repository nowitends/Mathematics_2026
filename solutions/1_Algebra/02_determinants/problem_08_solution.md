# Exercise 8 - Determinant of a Product

## Question

Let \(A\) and \(B\) be square matrices of the same size such that:

$$
\det(A) = 3, \qquad \det(B) = -5
$$

Compute \(\det(AB)\), \(\det(BA)\), and, if it exists, \(\det(A^{-1}B)\).

Explain why \(\det(AB)=\det(BA)\), even though the matrices \(AB\) and \(BA\) may be different.


## Solution

### 1. Determinant of \(AB\)

Using the determinant property for matrix multiplication:

$$
\det(AB) = \det(A) \cdot \det(B)
$$

Substituting the given values:

$$
\det(AB) = 3 \cdot (-5)
$$

$$
\boxed{\det(AB) = -15}
$$

### 2. Determinant of \(BA\)

Using the same property:

$$
\det(BA) = \det(B) \cdot \det(A)
$$

Substituting:

$$
\det(BA) = (-5) \cdot 3
$$

$$
\boxed{\det(BA) = -15}
$$

### 3. Determinant of \(A^{-1}B\)

Since:

$$
\det(A) = 3 \neq 0
$$

The matrix \(A\) is invertible.

The determinant of an inverse matrix is:

$$
\det(A^{-1}) = \frac{1}{\det(A)}
$$

Therefore:

$$
\det(A^{-1}) = \frac{1}{3}
$$

Using the determinant property for matrix multiplication:

$$
\det(A^{-1}B) = \det(A^{-1}) \cdot \det(B)
$$

Substituting:

$$
\det(A^{-1}B) = \frac{1}{3} \cdot (-5)
$$

$$
\boxed{\det(A^{-1}B) = -\frac{5}{3}}
$$

### 4. Explanation

Although matrix multiplication is generally not commutative:

$$
AB \neq BA
$$

Their determinants are equal because:

$$
\det(AB) = \det(A)\det(B)
$$

and

$$
\det(BA) = \det(B)\det(A)
$$

Since multiplication of numbers is commutative:

$$
\det(A)\det(B) = \det(B)\det(A)
$$

Therefore:

$$
\det(AB) = \det(BA)
$$

## Conclusion

The results are:

$$
\boxed{\det(AB) = -15}
$$

$$
\boxed{\det(BA) = -15}
$$

$$
\boxed{\det(A^{-1}B) = -\frac{5}{3}}
$$

The determinants of \(AB\) and \(BA\) are equal because the determinant of a product is the product of the individual determinants.

Also, \(A^{-1}\) exists because \(\det(A) \neq 0\).