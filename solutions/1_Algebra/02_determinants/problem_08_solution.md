# Exercise 8 – Determinant of a Product

## Question

Let $A$ and $B$ be square matrices such that:

$$
\det(A)=3, \qquad \det(B)=-5.
$$

Compute:

$$
\det(AB), \qquad \det(BA), \qquad \det(A^{-1}B).
$$

Explain why the first two results are equal even though usually $AB \neq BA$.

## Solution

### 1. Determinant of AB

Using the determinant product property:

$$
\det(AB)=\det(A)\cdot\det(B)
$$

Substituting the given values:

$$
\det(AB)=3\cdot(-5)
$$

$$
\boxed{\det(AB)=-15}
$$

### 2. Determinant of BA

Similarly:

$$
\det(BA)=\det(B)\cdot\det(A)
$$

Substituting:

$$
\det(BA)=(-5)\cdot3
$$

$$
\boxed{\det(BA)=-15}
$$

### 3. Determinant of A^{-1}B

Since $\det(A)=3\neq0$, the inverse of $A$ exists.

Using the determinant properties:

$$
\det(A^{-1}B)=\det(A^{-1})\cdot\det(B)
$$

And:

$$
\det(A^{-1})=\frac{1}{\det(A)}
$$

Therefore:

$$
\det(A^{-1}B)=\frac{1}{3}\cdot(-5)
$$

$$
\boxed{\det(A^{-1}B)=-\frac{5}{3}}
$$

### 4. Comparison and Explanation

The results are:

$$
\det(AB)=\det(BA)=-15
$$

$$
\det(A^{-1}B)=-\frac{5}{3}
$$

Although matrix multiplication is generally not commutative, the determinant of a product satisfies:

$$
\det(AB)=\det(A)\det(B)
$$

Since multiplication of real numbers is commutative:

$$
\det(A)\det(B)=\det(B)\det(A)
$$

Therefore, $\det(AB)=\det(BA)$, even though $AB$ and $BA$ are not necessarily equal.

**Conclusion:** The determinant of a product depends on the determinants of the individual matrices, not on the order of the factors.