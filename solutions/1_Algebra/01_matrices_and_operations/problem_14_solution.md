# Exercise 14 – Rotation Matrices

## Question

The rotation matrix is:

\[
R(\theta)=\begin{pmatrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{pmatrix}
\]

Calculate \(R(\alpha)R(\beta)\) and show that \(R(\alpha)R(\beta)=R(\alpha+\beta)\) using the angle-sum formulas. Explain the result geometrically.

## Solution

Multiplying the matrices:

\[
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta&
-\cos\alpha\sin\beta-\sin\alpha\cos\beta\\
\sin\alpha\cos\beta+\cos\alpha\sin\beta&
\cos\alpha\cos\beta-\sin\alpha\sin\beta
\end{pmatrix}
\]

Using the angle-sum formulas:

\[
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta
\]

\[
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta
\]

Therefore:

\[
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta)&-\sin(\alpha+\beta)\\
\sin(\alpha+\beta)&\cos(\alpha+\beta)
\end{pmatrix}
\]

\[
R(\alpha)R(\beta)=R(\alpha+\beta)
\]

Geometrically, two rotations performed one after another are equal to one rotation by the sum of their angles.