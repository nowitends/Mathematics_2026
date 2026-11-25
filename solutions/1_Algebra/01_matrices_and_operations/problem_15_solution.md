## Exercise 15 – Associativity of Multiplication and Different Calculation Paths

### Question

Given:

$$
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},
\quad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix},
\quad
C=\begin{pmatrix}2&1\\0&-1\end{pmatrix}
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

### Solution

First, calculate $AB$:

$$
AB=
\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix}
\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}
=
\begin{pmatrix}5&2\\1&4\end{pmatrix}
$$

Then:

$$
(AB)C=
\begin{pmatrix}5&2\\1&4\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
$$

Now calculate $BC$:

$$
BC=
\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
=
\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}
$$

Then:

$$
A(BC)=
\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix}
\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}
=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
$$

### Comparison

Both methods give the same result:

$$
(AB)C=A(BC)=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
$$

For $(AB)C$, there are 20 multiplications and 12 additions.

For $A(BC)$, there are 24 multiplications and 14 additions.

The first method requires fewer operations. This example shows that matrix multiplication is associative, meaning that changing the grouping does not change the final result.