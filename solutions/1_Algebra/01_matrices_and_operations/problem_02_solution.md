# Exercise 2 – Addition and Scalar Multiplication

## Question

Given the matrices:

\[
A=\begin{pmatrix}1&2\\-1&3\end{pmatrix},
\quad
B=\begin{pmatrix}4&-2\\0&5\end{pmatrix}
\]

Calculate:

1. \(A+B\)
2. \(A-B\)
3. \(3A-2B\)

Explain why matrices must have the same size for addition.

## Solution

**1. Addition**

\[
A+B=
\begin{pmatrix}
1+4&2+(-2)\\
-1+0&3+5
\end{pmatrix}
=
\begin{pmatrix}
5&0\\
-1&8
\end{pmatrix}
\]

**2. Subtraction**

\[
A-B=
\begin{pmatrix}
1-4&2-(-2)\\
-1-0&3-5
\end{pmatrix}
=
\begin{pmatrix}
-3&4\\
-1&-2
\end{pmatrix}
\]

**3. Scalar multiplication**

First:

\[
3A=\begin{pmatrix}3&6\\-3&9\end{pmatrix}
\]

\[
2B=\begin{pmatrix}8&-4\\0&10\end{pmatrix}
\]

Then:

\[
3A-2B=
\begin{pmatrix}
3-8&6-(-4)\\
-3-0&9-10
\end{pmatrix}
=
\begin{pmatrix}
-5&10\\
-3&-1
\end{pmatrix}
\]

**4. Explanation**

Both matrices have size \(2\times2\).

Matrix addition is possible only when both matrices have the same number of rows and columns. This is because we add elements in the same positions.