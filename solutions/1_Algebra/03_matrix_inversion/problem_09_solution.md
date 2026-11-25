# Exercise 9 – Matrix Equation

## Question

Given:

$$
A=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix},
\qquad
B=
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

### 1. Decide Where to Apply the Inverse

We are given:

$$
AX=B
$$

Since $A$ is on the left side of $X$, we must multiply both sides by $A^{-1}$ from the left.

$$
A^{-1}(AX)=A^{-1}B
$$

Using the identity property:

$$
IX=A^{-1}B
$$

Therefore:

$$
X=A^{-1}B
$$

### 2. Calculate the Inverse of A

First, calculate the determinant:

$$
\det(A)=(1)(1)-(2)(0)=1
$$

Since the determinant is not zero, $A$ is invertible.

$$
A^{-1}
=
\begin{pmatrix}
1&-2\\
0&1
\end{pmatrix}
$$

### 3. Calculate X

Using $X=A^{-1}B$:

$$
X=
\begin{pmatrix}
1&-2\\
0&1
\end{pmatrix}
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
$$

$$
X=
\begin{pmatrix}
3-4&1-8\\
2&4
\end{pmatrix}
$$

$$
\boxed{
X=
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
}
$$

### 4. Verify the Result by Calculating AX

Substitute the calculated matrix $X$ into the original equation:

$$
AX=
\begin{pmatrix}
1&2\\
0&1
\end{pmatrix}
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
$$

$$
AX=
\begin{pmatrix}
-1+4&-7+8\\
2&4
\end{pmatrix}
$$

$$
AX=
\begin{pmatrix}
3&1\\
2&4
\end{pmatrix}
=B
$$

The result is equal to the given matrix $B$.

**Conclusion**

The solution is:

$$
\boxed{
X=
\begin{pmatrix}
-1&-7\\
2&4
\end{pmatrix}
}
$$

The inverse must be multiplied from the left because $A$ is on the left side of $X$. The verification confirms that $AX=B$.