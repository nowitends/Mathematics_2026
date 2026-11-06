# Exercise 9 – Composing Transformations

## Question

Given:

\[
S=\begin{pmatrix}2&0\\0&1\end{pmatrix},
\quad
R=\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\quad
x=\begin{pmatrix}1\\2\end{pmatrix}
\]

Calculate \(RSx\) and \(SRx\). Compare the results and explain why the order of transformations matters.

## Solution

First, calculate \(Sx\):

\[
Sx=\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
=\begin{pmatrix}2\\2\end{pmatrix}
\]

Then:

\[
RSx=
\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}2\\2\end{pmatrix}
=\begin{pmatrix}-2\\2\end{pmatrix}
\]

Now calculate \(Rx\):

\[
Rx=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
\begin{pmatrix}1\\2\end{pmatrix}
=\begin{pmatrix}-2\\1\end{pmatrix}
\]

Then:

\[
SRx=
\begin{pmatrix}2&0\\0&1\end{pmatrix}
\begin{pmatrix}-2\\1\end{pmatrix}
=\begin{pmatrix}-4\\1\end{pmatrix}
\]

Therefore:

\[
RSx=\begin{pmatrix}-2\\2\end{pmatrix},
\quad
SRx=\begin{pmatrix}-4\\1\end{pmatrix}
\]

Since the results are different, \(RSx\neq SRx\).

Geometrically, S stretches the x-coordinate, while R rotates the vector 90° counterclockwise. Applying scaling before rotation gives a different result than applying rotation before scaling. Therefore, the order of transformations matters.