## Exercise 14. A System of Equations and the Determinant

### Question

Consider the system $Ax = b$, where

$$
A = \begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix}
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

---

### Solution

#### 1. Unique Solution Condition (Determinant Test)
A linear system $Ax = b$ with a square matrix $A$ has a unique solution for every vector $b$ if and only if the matrix $A$ is invertible, which is equivalent to saying its determinant is non-zero:

$$
\det(A) \neq 0
$$

Let's compute the determinant of $A$:

$$
\det(A) = (1)(4) - (2)(k) = 4 - 2k
$$

For the system to have a unique solution, we set:

$$
4 - 2k \neq 0 \implies 2k \neq 2 \implies k \neq 2
$$

Thus, the system has **exactly one solution for every $b$** when **$k \neq 2$**.

---

#### 2. The Exceptional Case ($k = 2$)
When $k = 2$, the matrix becomes:

$$
A = \begin{pmatrix}
1 & 2 \\
2 & 4
\end{pmatrix}
$$

In this case, $\det(A) = 0$, meaning the rows are linearly dependent (the second row is twice the first row: $R_2 \to R_2 - 2R_1$). 

Let $b = \begin{pmatrix} b_1 \\ b_2 \end{pmatrix}$ and set up the augmented matrix $\begin{pmatrix} A \mid b \end{pmatrix}$:

$$
\begin{pmatrix}
1 & 2 & \mid & b_1 \\
2 & 4 & \mid & b_2
\end{pmatrix}
$$

Applying the row operation $R_2 \to R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & b_1 \\
0 & 0 & \mid & b_2 - 2b_1
\end{pmatrix}
$$

#### A. Example for Infinitely Many Solutions
For the system to be consistent (and thus have solutions), the last row must yield a true statement ($0 = 0$), meaning:

$$
b_2 - 2b_1 = 0 \implies b_2 = 2b_1
$$

If we choose $b_1 = 1$, then $b_2 = 2$. Thus, choosing the right-hand side vector as:

$$
b = \begin{pmatrix} 1 \\ 2 \end{pmatrix}
$$

gives the system **infinitely many solutions** because the second equation becomes redundant ($0 = 0$).

#### B. Example for No Solution
For the system to have **no solution**, it must be inconsistent, meaning the left-hand side reduces to $0$ while the right-hand side is non-zero ($b_2 - 2b_1 \neq 0$):

$$
b_2 - 2b_1 \neq 0 \implies b_2 \neq 2b_1
$$

If we choose $b_1 = 1$, we can choose $b_2 = 3$ (since $3 \neq 2(1)$). Thus, choosing the right-hand side vector as:

$$
b = \begin{pmatrix} 1 \\ 3 \end{pmatrix}
$$

gives the system **no solution** because the second row yields the contradiction $0 = 1$.

---

### Conclusion
* The system has a unique solution for all $k \neq 2$.
* When $k = 2$, choosing $b = \begin{pmatrix} 1 \\ 2 \end{pmatrix}$ results in **infinitely many solutions**, while choosing $b = \begin{pmatrix} 1 \\ 3 \end{pmatrix}$ results in **no solution**.