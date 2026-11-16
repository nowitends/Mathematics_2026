# Exercise 6 – Transpose

## Question

Given:

$$
A=\begin{pmatrix}1&2&3\\4&5&6\end{pmatrix},
\quad
B=\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}
$$

Compute \(A^T\), \(B^T\), and \(AB\). Verify that \((AB)^T=B^TA^T\).

## Solution

First, calculate the transposes:

$$
A^T=\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix}
$$

$$
B^T=\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}
$$

Calculate AB:

$$
AB=
\begin{pmatrix}1&2&3\\4&5&6\end{pmatrix}
\begin{pmatrix}1&0\\2&1\\-1&3\end{pmatrix}
=
\begin{pmatrix}2&11\\8&23\end{pmatrix}
$$

Therefore:

$$
(AB)^T=\begin{pmatrix}2&8\\11&23\end{pmatrix}
$$

Now calculate \(B^TA^T\):

$$
B^TA^T=
\begin{pmatrix}1&2&-1\\0&1&3\end{pmatrix}
\begin{pmatrix}1&4\\2&5\\3&6\end{pmatrix}
$$

$$
=\begin{pmatrix}2&8\\11&23\end{pmatrix}
$$

Thus:

$$
\boxed{(AB)^T=B^TA^T}
$$

Both results are equal. The transpose of a product reverses the order of the factors.