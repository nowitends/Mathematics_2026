# Exercise 4 – Matrix Multiplication and Noncommutativity

## Question

Given:

\[
A=\begin{pmatrix}1&2\\0&1\end{pmatrix},
\quad B=\begin{pmatrix}2&0\\3&1\end{pmatrix}
\]

Calculate AB and BA. Are they equal? Explain your answer.

## Solution

First, calculate AB:

\[
AB=\begin{pmatrix}
1(2)+2(3)&1(0)+2(1)\\
0(2)+1(3)&0(0)+1(1)
\end{pmatrix}
=\begin{pmatrix}8&2\\3&1\end{pmatrix}
\]

Now calculate BA:

\[
BA=\begin{pmatrix}
2(1)+0(0)&2(2)+0(1)\\
3(1)+1(0)&3(2)+1(1)
\end{pmatrix}
=\begin{pmatrix}2&4\\3&7\end{pmatrix}
\]

Since \(AB\neq BA\), matrix multiplication is not commutative. This means changing the order of multiplication changes the result.