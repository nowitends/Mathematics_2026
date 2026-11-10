## Exercise 8. Row Operations and Their Reversibility

### Question

For:
$$A = \begin{pmatrix} 1 & 2 & -1 \\ 2 & 4 & 1 \\ -1 & 1 & 3 \end{pmatrix}$$

Perform, in order:
1. $R_2 \leftarrow R_2 - 2R_1$
2. $R_3 \leftarrow R_3 + R_1$
3. Interchange $R_2$ and $R_3$

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

*Why this exercise:* prepares for elimination by showing that row operations are controlled and reversible transformations of a matrix.

---

### Solution

#### 1. Step-by-Step Matrix Transformations

* **Initial Matrix ($A$):**
  $$A = \begin{pmatrix} 1 & 2 & -1 \\ 2 & 4 & 1 \\ -1 & 1 & 3 \end{pmatrix}$$

* **Step 1 ($R_2 \leftarrow R_2 - 2R_1$):**
  Subtracting $2$ times the first row from the second row:
  $$A_1 = \begin{pmatrix} 1 & 2 & -1 \\ 2 - 2(1) & 4 - 2(2) & 1 - 2(-1) \\ -1 & 1 & 3 \end{pmatrix} = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ -1 & 1 & 3 \end{pmatrix}$$

* **Step 2 ($R_3 \leftarrow R_3 + R_1$):**
  Adding the first row to the third row:
  $$A_2 = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ -1 + 1 & 1 + 2 & 3 + (-1) \end{pmatrix} = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ 0 & 3 & 2 \end{pmatrix}$$

* **Step 3 (Interchange $R_2$ and $R_3$):**
  Swapping the second and third rows:
  $$A_3 = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 3 & 2 \\ 0 & 0 & 3 \end{pmatrix}$$

#### 2. Reversing Operations
Each elementary row operation can be undone by applying its inverse operation:
* **For Step 1 ($R_2 \leftarrow R_2 - 2R_1$):** The reverse operation is adding $2$ times the first row back to the second row, denoted as **$R_2 \leftarrow R_2 + 2R_1$**.
* **For Step 2 ($R_3 \leftarrow R_3 + R_1$):** The reverse operation is subtracting the first row from the third row, denoted as **$R_3 \leftarrow R_3 - R_1$**.
* **For Step 3 (Interchange $R_2$ and $R_3$):** The reverse operation is simply **interchanging $R_2$ and $R_3$ again**.