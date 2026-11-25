# Exercise 14 – A System of Equations and the Determinant

## Question

Consider the system:

$$
Ax=b
$$

where

$$
A=
\begin{pmatrix}
1 & 2\\
k & 4
\end{pmatrix}
$$

For which values of $k$ does the system have exactly one solution for every $b$?

For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

## Solution

### 1. Determine when the system has a unique solution

A square linear system has exactly one solution for every right-hand side $b$ if and only if its coefficient matrix is invertible.

This happens when:

$$
\det(A)\neq 0
$$

Calculate the determinant:

$$
\det(A)=
\begin{vmatrix}
1 & 2\\
k & 4
\end{vmatrix}
$$

$$
\det(A)=1\cdot4-2\cdot k
$$

$$
\det(A)=4-2k
$$

For the matrix to be invertible:

$$
4-2k\neq0
$$

$$
-2k\neq-4
$$

$$
2k\neq4
$$

Therefore:

$$
\boxed{k\neq2}
$$

Thus, the system has exactly one solution for every $b$ when $k\neq2$.

### 2. The exceptional case: k = 2

When $k=2$, the coefficient matrix becomes:

$$
A=
\begin{pmatrix}
1 & 2\\
2 & 4
\end{pmatrix}
$$

The system is:

$$
\begin{cases}
x_1+2x_2=b_1\\
2x_1+4x_2=b_2
\end{cases}
$$

The second equation has a left-hand side that is twice the first equation.

Therefore, the system has either infinitely many solutions or no solution, depending on the right-hand side.

### 3. Example with infinitely many solutions

Choose:

$$
b=
\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

The system becomes:

$$
\begin{cases}
x_1+2x_2=1\\
2x_1+4x_2=2
\end{cases}
$$

The second equation is exactly twice the first equation.

Therefore, both equations represent the same line, and there are infinitely many solutions.

### 4. Example with no solution

Choose:

$$
b=
\begin{pmatrix}
1\\
0
\end{pmatrix}
$$

The system becomes:

$$
\begin{cases}
x_1+2x_2=1\\
2x_1+4x_2=0
\end{cases}
$$

Multiplying the first equation by 2 gives:

$$
2x_1+4x_2=2
$$

However, the second equation requires:

$$
2x_1+4x_2=0
$$

This is a contradiction.

Therefore, the system has no solution.

### Conclusion

The determinant is:

$$
\det(A)=4-2k
$$

- If $k\neq2$, the system has exactly one solution for every $b$.
- If $k=2$ and $b=(1,2)^T$, the system has infinitely many solutions.
- If $k=2$ and $b=(1,0)^T$, the system has no solution.

The determinant determines whether the coefficient matrix is invertible and therefore whether the system has a unique solution for every right-hand side.