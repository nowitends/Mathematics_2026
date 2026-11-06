# Exercise 15 – Associativity of Multiplication and Different Calculation Paths

## Question

Given:

\[
A=\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix},
\quad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix},
\quad
C=\begin{pmatrix}2&1\\0&-1\end{pmatrix}
\]

Calculate \((AB)C\) and \(A(BC)\). Compare the results and the number of intermediate operations. Explain associativity of matrix multiplication.

## Solution

First, calculate AB:

\[
AB=
\begin{pmatrix}
1&2&0\\0&1&1
\end{pmatrix}
\begin{pmatrix}
1&0\\2&1\\-1&3
\end{pmatrix}
=
\begin{pmatrix}5&2\\1&4\end{pmatrix}
\]

Then:

\[
(AB)C=
\begin{pmatrix}5&2\\1&4\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
\]

Now calculate BC:

\[
BC=
\begin{pmatrix}
1&0\\2&1\\-1&3
\end{pmatrix}
\begin{pmatrix}2&1\\0&-1\end{pmatrix}
=
\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}
\]

Then:

\[
A(BC)=
\begin{pmatrix}1&2&0\\0&1&1\end{pmatrix}
\begin{pmatrix}2&1\\4&1\\-2&-4\end{pmatrix}
=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
\]

Both results are equal:

\[
(AB)C=A(BC)=
\begin{pmatrix}10&3\\2&-3\end{pmatrix}
\]

Each calculation path requires two matrix multiplications. The first path needs 20 scalar multiplications, while the second needs 24.

This shows that matrix multiplication is associative. Changing the grouping does not change the final result, but it can change the amount of calculation.