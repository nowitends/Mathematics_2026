## Exercise 10. Columns of a Matrix Product

### Question

Given:
$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}, \quad
B = \begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
$$

Denote the columns of $B$ by $b_1, b_2$.
1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

*Why this exercise:* extends the interpretation of matrix-vector multiplication to a full product of two matrices instead of simply repeating another $Ax$ exercise.

---

### Solution

#### 1. Computing $Ab_1$ and $Ab_2$
First, let's identify the columns of matrix $B$:
$$
b_1 = \begin{pmatrix} 1 \\ -1 \\ 3 \end{pmatrix}, \quad b_2 = \begin{pmatrix} 2 \\ 0 \\ 1 \end{pmatrix}
$$

* **Computing $Ab_1$:**
  $$
  Ab_1 = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 1 \\ -1 \\ 3 \end{pmatrix} = \begin{pmatrix} (1)(1) + (2)(-1) + (0)(3) \\ (0)(1) + (1)(-1) + (1)(3) \end{pmatrix} = \begin{pmatrix} 1 - 2 + 0 \\ 0 - 1 + 3 \end{pmatrix} = \begin{pmatrix} -1 \\ 2 \end{pmatrix}
  $$

* **Computing $Ab_2$:**
  $$
  Ab_2 = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 2 \\ 0 \\ 1 \end{pmatrix} = \begin{pmatrix} (1)(2) + (2)(0) + (0)(1) \\ (0)(2) + (1)(0) + (1)(1) \end{pmatrix} = \begin{pmatrix} 2 + 0 + 0 \\ 0 + 0 + 1 \end{pmatrix} = \begin{pmatrix} 2 \\ 1 \end{pmatrix}
  $$

#### 2. Computing the Matrix $AB$
Multiplying matrices $A_{2 \times 3}$ and $B_{3 \times 2}$ directly:
$$
AB = \begin{pmatrix}
(1)(1) + (2)(-1) + (0)(3) & (1)(2) + (2)(0) + (0)(1) \\
(0)(1) + (1)(-1) + (1)(3) & (0)(2) + (1)(0) + (1)(1)
\end{pmatrix} = \begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
$$

#### 3. Comparison and Explanation
Comparing the vectors from part 1 with the columns of the product matrix from part 2:
* The first column of $AB$ is $\begin{pmatrix} -1 \\ 2 \end{pmatrix}$, which is exactly $Ab_1$.
* The second column of $AB$ is $\begin{pmatrix} 2 \\ 1 \end{pmatrix}$, which is exactly $Ab_2$.

* **Why this happens:** By definition of matrix multiplication, multiplying a matrix $A$ by a matrix $B = \begin{pmatrix} b_1 & b_2 \end{pmatrix}$ results in a matrix whose columns are formed by multiplying $A$ by each individual column of $B$, yielding $\begin{pmatrix} Ab_1 & Ab_2 \end{pmatrix}$.