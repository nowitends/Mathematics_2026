# Exercise 5 – Matrix Times Vector

## Question

Given:

\[
A=\begin{pmatrix}2&-1\\1&3\end{pmatrix},
\quad x=\begin{pmatrix}4\\2\end{pmatrix}
\]

Calculate Ax and express it as a linear combination of the columns of A.

## Solution

\[
Ax=\begin{pmatrix}2&-1\\1&3\end{pmatrix}
\begin{pmatrix}4\\2\end{pmatrix}
=\begin{pmatrix}2(4)-2\\4+3(2)\end{pmatrix}
=\begin{pmatrix}6\\10\end{pmatrix}
\]

The columns of A are:

\[
a_1=\begin{pmatrix}2\\1\end{pmatrix},
\quad a_2=\begin{pmatrix}-1\\3\end{pmatrix}
\]

Using the elements of x as coefficients:

\[
Ax=4a_1+2a_2
\]

\[
=4\begin{pmatrix}2\\1\end{pmatrix}
+2\begin{pmatrix}-1\\3\end{pmatrix}
=\begin{pmatrix}6\\10\end{pmatrix}
\]

Both calculations give the same result.