## Exercise 6. Transpose

### Question

For the matrices:
$$
A = \begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}, \quad
B = \begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
$$

Compute $A^T$, $B^T$, and $AB$. Then verify in this example that:
$$(AB)^T = B^T A^T$$

*Why this exercise:* teaches transposition and an important property that reverses the order of factors.

---

### Solution

#### 1. Computing Transposes $A^T$ and $B^T$
The transpose of a matrix is obtained by swapping its rows and columns.
* For $A$ (size $2 \times 3$), the transpose $A^T$ will be of size $3 \times 2$:
  $$
  A^T = \begin{pmatrix}
  1 & 4 \\
  2 & 5 \\
  3 & 6
  \end{pmatrix}
  $$
* For $B$ (size $3 \times 2$), the transpose $B^T$ will be of size $2 \times 3$:
  $$
  B^T = \begin{pmatrix}
  1 & 2 & -1 \\
  0 & 1 & 3
  \end{pmatrix}
  $$

#### 2. Computing the Product $AB$
Multiplying $A_{2 \times 3}$ and $B_{3 \times 2}$ yields a $2 \times 2$ matrix:
$$
AB = \begin{pmatrix}
(1)(1) + (2)(2) + (3)(-1) & (1)(0) + (2)(1) + (3)(3) \\
(4)(1) + (5)(2) + (6)(-1) & (4)(0) + (5)(1) + (6)(3)
\end{pmatrix}
$$
Simplifying the entries:
* Row 1, Col 1: $1 + 4 - 3 = 2$
* Row 1, Col 2: $0 + 2 + 9 = 11$
* Row 2, Col 1: $4 + 10 - 6 = 8$
* Row 2, Col 2: $0 + 5 + 18 = 23$

Thus:
$$
AB = \begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
$$

#### 3. Verifying $(AB)^T = B^T A^T$
* **Left-hand side, $(AB)^T$:**
  Taking the transpose of $AB$:
  $
  (AB)^T = \begin{pmatrix}
  2 & 8 \\
  11 & 23
  \end{pmatrix}
  $

* **Right-hand side, $B^T A^T$:**
  Multiplying $B^T_{2 \times 3}$ and $A^T_{3 \times 2}$:
  $$
  B^T A^T = \begin{pmatrix}
  (1)(1) + (2)(4) + (-1)(3) & (1)(4) + (2)(5) + (-1)(6) \\
  (0)(1) + (1)(4) + (3)(3) & (0)(4) + (1)(5) + (3)(6)
  \end{pmatrix}
  $$
  Calculating each entry:
  * Row 1, Col 1: $1 + 8 - 3 = 2$
  * Row 1, Col 2: $4 + 10 - 6 = 8$
  * Row 2, Col 1: $0 + 4 + 9 = 13$ $\rightarrow$ *Bekle, küçük bir kontrol yapalım:* $(0)(1) + (1)(2) + (3)(3) = 0 + 2 + 9 = 11$. (Doğrusu 11 olacak).
  * Row 2, Col 2: $0 + 5 + 18 = 23$

  Düzenlenmiş hali:
  $$
  B^T A^T = \begin{pmatrix}
  2 & 8 \\
  11 & 23
  \end{pmatrix}
  $$

Since both sides result in $\begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$, the property $(AB)^T = B^T A^T$ is successfully verified.