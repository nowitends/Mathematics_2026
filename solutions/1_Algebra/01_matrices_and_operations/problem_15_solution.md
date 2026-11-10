## Exercise 15. Associativity of Multiplication and Different Calculation Paths

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
\end{pmatrix}, \quad
C = \begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

*Why this exercise:* reinforces associativity by comparing two mathematically equivalent calculation paths.

---

### Solution

#### 1. Computing $(AB)C$
* **Step 1: Compute $AB$**
  $$
  AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1)+(2)(-1)+(0)(3) & (1)(2)+(2)(0)+(0)(1) \\ (0)(1)+(1)(-1)+(1)(3) & (0)(2)+(1)(0)+(1)(1) \end{pmatrix} = \begin{pmatrix} -1 & 2 \\ 2 & 1 \end{pmatrix}
  $$
* **Step 2: Compute $(AB)C$**
  $$
  (AB)C = \begin{pmatrix} -1 & 2 \\ 2 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} (-1)(2)+(2)(0) & (-1)(1)+(2)(-1) \\ (2)(2)+(1)(0) & (2)(1)+(1)(-1) \end{pmatrix} = \begin{pmatrix} -2 & -3 \\ 4 & 1 \end{pmatrix}
  $$

#### 2. Computing $A(BC)$
* **Step 1: Compute $BC$**
  $$
  BC = \begin{pmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} (1)(2)+(2)(0) & (1)(1)+(2)(-1) \\ (-1)(2)+(0)(0) & (-1)(1)+(0)(-1) \\ (3)(2)+(1)(0) & (3)(1)+(1)(-1) \end{pmatrix} = \begin{pmatrix} 2 & -1 \\ -2 & -1 \\ 6 & 2 \end{pmatrix}
  $$
* **Step 2: Compute $A(BC)$**
  $$
  A(BC) = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 2 & -1 \\ -2 & -1 \\ 6 & 2 \end{pmatrix} = \begin{pmatrix} (1)(2)+(2)(-2)+(0)(6) & (1)(-1)+(2)(-1)+(0)(2) \\ (0)(2)+(1)(-2)+(1)(6) & (0)(-1)+(1)(-1)+(1)(2) \end{pmatrix} = \begin{pmatrix} -2 & -3 \\ 4 & 1 \end{pmatrix}
  $$

#### 3. Comparison and Meaning of Associativity
* **Results Comparison:** Both calculation paths yield the exact same resulting matrix:
  $$
  (AB)C = A(BC) = \begin{pmatrix} -2 & -3 \\ 4 & 1 \end{pmatrix}
  $$
* **Number of Intermediate Operations:** 
  * Path 1 ($(AB)C$) computes a $2 \times 3$ times $3 \times 2$ product first, followed by a $2 \times 2$ times $2 \times 2$ product.
  * Path 2 ($A(BC)$) computes a $3 \times 2$ times $2 \times 2$ product first, followed by a $2 \times 3$ times $3 \times 2$ product. 
  Although the computational workload (number of scalar multiplications and additions) differs depending on which grouping is evaluated first, the final outcome remains identical.
* **Meaning of Associativity:** This property demonstrates the **associativity** of matrix multiplication, meaning that when multiplying three matrices, changing the grouping parentheses does not alter the final product.