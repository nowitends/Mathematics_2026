# Exercise 7 – Inverse of a Product

## Question

Given:

$$
A=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
2&0\\
0&3
\end{pmatrix}
$$

Compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## Solution

### 1. Calculate AB

$$
AB=
\begin{pmatrix}
1&1\\
0&1
\end{pmatrix}
\begin{pmatrix}
2&0\\
0&3
\end{pmatrix}
$$

$$
AB=
\begin{pmatrix}
2&3\\
0&3
\end{pmatrix}
$$

### 2. Calculate the Determinant

$$
\det(AB)=(2)(3)-(3)(0)=6
$$

Since the determinant is not zero, the inverse exists.

### 3. Calculate the Inverse of AB

Using the inverse formula for a $2\times2$ matrix:

$$
(AB)^{-1}
=
\frac{1}{6}
\begin{pmatrix}
3&-3\\
0&2
\end{pmatrix}
$$

$$
(AB)^{-1}
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
$$

### 4. Calculate B⁻¹ and A⁻¹

First, calculate the inverse of B:

$$
B^{-1}=
\begin{pmatrix}
\frac12&0\\
0&\frac13
\end{pmatrix}
$$

Now, calculate the inverse of A:

$$
A^{-1}=
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

### 5. Calculate B⁻¹A⁻¹

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12&0\\
0&\frac13
\end{pmatrix}
\begin{pmatrix}
1&-1\\
0&1
\end{pmatrix}
$$

$$
B^{-1}A^{-1}
=
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
$$

Therefore, both methods give the same result:

$$
\boxed{
(AB)^{-1}=B^{-1}A^{-1}
}
$$

### 6. Verify the Results

Multiply the original product by its calculated inverse:

$$
(AB)(B^{-1}A^{-1})
=
\begin{pmatrix}
2&3\\
0&3
\end{pmatrix}
\begin{pmatrix}
\frac12&-\frac12\\
0&\frac13
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1&0\\
0&1
\end{pmatrix}
=I
$$

The reverse multiplication also gives the identity matrix:

$$
(B^{-1}A^{-1})(AB)=I
$$

This confirms that the calculated matrix is the correct inverse.

### 7. Explanation of the Reversed Order

In matrix multiplication, $AB$ means that B acts first and then A.

To undo these operations, we must first undo A using $A^{-1}$ and then undo B using $B^{-1}$.

Therefore, the order is reversed when calculating the inverse of a product:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

**Conclusion**

Both calculations give the same inverse matrix. The verification shows that their product is the identity matrix. The order is reversed because the inverse operations must undo the original transformations in the opposite order.