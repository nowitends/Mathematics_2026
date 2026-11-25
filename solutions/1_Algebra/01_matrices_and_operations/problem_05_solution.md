## Exercise 5. Matrix Times Vector

### Question

Let:
$$
A = \begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}, \quad
x = \begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

*Why this exercise:* shows that multiplying a matrix by a vector can be understood as a linear combination of the matrix columns.

---

### Solution

#### 1. Finding $Ax$
Carrying out the matrix-vector multiplication:
$$
Ax = \begin{pmatrix}
(2)(4) + (-1)(2) \\
(1)(4) + (3)(2)
\end{pmatrix} = \begin{pmatrix}
8 - 2 \\
4 + 6
\end{pmatrix} = \begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

#### 2. Writing $Ax$ as a Linear Combination of Columns
Matrix-vector multiplication can also be viewed as taking a linear combination of the matrix's columns, using the components of vector $x$ as weights.

Let's call the columns of $A$ as $a_1$ and $a_2$:
$$
a_1 = \begin{pmatrix} 2 \\ 1 \end{pmatrix}, \quad a_2 = \begin{pmatrix} -1 \\ 3 \end{pmatrix}
$$

Using the entries of $x = \begin{pmatrix} 4 \\ 2 \end{pmatrix}$ as weights:
$$
Ax = 4a_1 + 2a_2 = 4 \begin{pmatrix} 2 \\ 1 \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \end{pmatrix}
$$

If we compute this:
$$
Ax = \begin{pmatrix} 8 \\ 4 \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \end{pmatrix} = \begin{pmatrix} 8 - 2 \\ 4 + 6 \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \end{pmatrix}
$$
As expected, both methods produce the exact same vector.