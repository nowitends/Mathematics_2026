# Exercise 6 – Transpose

## Question

Given:

\[
A=\begin{pmatrix}1&2&3\\4&5&6\end{pmatrix},
\quad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}
\]

Calculate \(A^T\), \(B^T\) and \(AB\). Verify that \((AB)^T=B^TA^T\).

## Solution

The transpose is obtained by changing rows into columns.

\[
A^T=\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix},
\quad
B^T=\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}
\]

First, calculate AB:

\[
AB=\begin{pmatrix}
1(1)+2(2)+3(-1)&1(0)+2(1)+3(3)\\
4(1)+5(2)+6(-1)&4(0)+5(1)+6(3)
\end{pmatrix}
\]

\[
AB=\begin{pmatrix}2&11\\8&23\end{pmatrix}
\]

Taking the transpose:

\[
(AB)^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}
\]

Now calculate \(B^TA^T\):

\[
B^TA^T=
\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}
\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix}
\]

\[
B^TA^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}
\]

Therefore,

\[
(AB)^T=B^TA^T
\]

The results are equal, so the property is verified.