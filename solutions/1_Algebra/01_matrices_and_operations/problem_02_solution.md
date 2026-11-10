## Exercise 2. Addition and Scalar Multiplication

### Question

For the matrices:

$$
A = \begin{pmatrix}
3 & 2 \\
-1 & 3
\end{pmatrix}, \quad
B = \begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix}
$$

Compute:
1. $A + B$
2. $A - B$
3. $3A - 2B$

Explain why matrix addition is possible only for matrices of the same size.

*Why this exercise:* reinforces entry-by-entry operations and the importance of compatible dimensions.

---

### Solution

#### 1. Computing $A + B$
Matrix addition is performed entry by entry. The calculation for each representative entry is as follows:
* Top-left entry: $3 + 4 = 7$
* Top-right entry: $2 + (-2) = 0$
* Bottom-left entry: $-1 + 0 = -1$
* Bottom-right entry: $3 + 5 = 8$

Thus, combining these calculations yields:
$$
A + B = \begin{pmatrix}
3 + 4 & 2 + (-2) \\
-1 + 0 & 3 + 5
\end{pmatrix} = \begin{pmatrix}
7 & 0 \\
-1 & 8
\end{pmatrix}
$$

#### 2. Computing $A - B$
Matrix subtraction is similarly performed entry by entry:
$$
A - B = \begin{pmatrix}
3 - 4 & 2 - (-2) \\
-1 - 0 & 3 - 5
\end{pmatrix} = \begin{pmatrix}
-1 & 4 \\
-1 & -2
\end{pmatrix}
$$

#### 3. Computing $3A - 2B$
First, perform scalar multiplication by multiplying every entry of matrix $A$ by $3$ and every entry of matrix $B$ by $2$:
$$
3A = 3 \begin{pmatrix} 3 & 2 \\ -1 & 3 \end{pmatrix} = \begin{pmatrix} 9 & 6 \\ -3 & 9 \end{pmatrix}
$$
$$
2B = 2 \begin{pmatrix} 4 & -2 \\ 0 & 5 \end{pmatrix} = \begin{pmatrix} 8 & -4 \\ 0 & 10 \end{pmatrix}
$$
Then, subtract the resulting matrices entry by entry:
$$
3A - 2B = \begin{pmatrix}
9 - 8 & 6 - (-4) \\
-3 - 0 & 9 - 10
\end{pmatrix} = \begin{pmatrix}
1 & 10 \\
-3 & -1
\end{pmatrix}
$$

#### 4. Dimension Compatibility in Matrix Addition
Matrix addition and subtraction are defined only for matrices of the **same size** (dimensions). Because these operations are carried out entry by entry, every element in matrix $A$ must have a corresponding, uniquely paired element in matrix $B$. If dimensions do not match, certain entries would lack corresponding partners, making the operation impossible.