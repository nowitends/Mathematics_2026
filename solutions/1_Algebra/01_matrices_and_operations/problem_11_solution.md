## Exercise 11. When Do Matrices Commute?

### Question

Given:
$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}, \quad
B = \begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

Find the conditions on $a, b, c, d$ under which $AB = BA$. Describe the general form of all such matrices $B$.

*Why this exercise:* deepens the idea of noncommutativity by finding the conditions under which commutativity does hold.

---

### Solution

#### 1. Calculating Products $AB$ and $BA$
* **Computing $AB$:**
  $$
  AB = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} a & b \\ c & d \end{pmatrix} = \begin{pmatrix} (1)(a) + (1)(c) & (1)(b) + (1)(d) \\ (0)(a) + (1)(c) & (0)(b) + (1)(d) \end{pmatrix} = \begin{pmatrix} a + c & b + d \\ c & d \end{pmatrix}
  $$

* **Computing $BA$:**
  $$
  BA = \begin{pmatrix} a & b \\ c & d \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (a)(1) + (b)(0) & (a)(1) + (b)(1) \\ (c)(1) + (d)(0) & (c)(1) + (d)(1) \end{pmatrix} = \begin{pmatrix} a & a + b \\ c & c + d \end{pmatrix}
  $$

#### 2. Setting Up Conditions for $AB = BA$
For the two matrices to commute ($AB = BA$), their corresponding entries must be equal:
$$
\begin{pmatrix}
a + c & b + d \\
c & d
\end{pmatrix} = \begin{pmatrix}
a & a + b \\
c & c + d
\end{pmatrix}
$$

This gives us the following system of equations:
1. $a + c = a \implies c = 0$
2. $b + d = a + b \implies d = a$
3. $c = c$ (always true since $c = 0$)
4. $d = c + d \implies 0 = c$ (consistent)

Thus, the required conditions are **$c = 0$** and **$d = a$**, while $a$ and $b$ can be any arbitrary real numbers.

#### 3. General Form of Matrix $B$
Substituting these conditions back into $B$, the general form of all matrices that commute with $A$ is:
$$
B = \begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
$$
where $a$ and $b$ are any real numbers.