## Exercise 1. Matrix Size and Entries

### Question

Given the matrices:

$$
A = \begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5
\end{pmatrix}, \quad
B = \begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1
\end{pmatrix}
$$

1. State the sizes of matrices $A$ and $B$.
2. Read off the entries $a_{12}$, $a_{23}$, $b_{21}$, and $b_{32}$ (where $b_{32} = 1$).
3. Write the second row of $A$ and the first column of $B$ as vectors.

*Why this exercise:* builds basic fluency with matrix notation, indices, rows, and columns.

---

### Solution

#### 1. Sizes of Matrices $A$ and $B$
* Matrix $A$ has $2$ rows and $3$ columns, so its size (dimensions) is $2 \times 3$.
* Matrix $B$ has $3$ rows and $2$ columns, so its size (dimensions) is $3 \times 2$.

#### 2. Reading Specific Entries
Using standard row-column index notation ($a_{ij}$ represents the entry in row $i$, column $j$):
* $a_{12} = -1$ (element in the 1st row, 2nd column of $A$)
* $a_{23} = 5$ (element in the 2nd row, 3rd column of $A$)
* $b_{21} = -2$ (element in the 2nd row, 1st column of $B$)
* $b_{32} = 1$ (element in the 3rd row, 2nd column of $B$, as supplied)

#### 3. Rows and Columns as Vectors
* The second row of $A$ expressed as a row vector is $\begin{pmatrix} 0 & 4 & 5 \end{pmatrix}$.
* The first column of $B$ expressed as a column vector is $\begin{pmatrix} 1 \\ -2 \\ 4 \end{pmatrix}$.