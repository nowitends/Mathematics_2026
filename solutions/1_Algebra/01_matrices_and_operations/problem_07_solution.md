## Exercise 7. Identity Matrix, Zero Matrix, and Powers

### Question

For:
$$
A = \begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
$$

Compute:
$$AI, \quad IA, \quad A + 0, \quad A^2, \quad A^3$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

*Why this exercise:* organizes the roles of neutral elements and reveals regularity in successive powers of a matrix.

---

### Solution

#### 1. Computing $AI$ and $IA$
Here, $I$ is the $2 \times 2$ identity matrix: $I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$.
* Multiplying $A$ by $I$:
  $$
  AI = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = A
  $$
* Multiplying $I$ by $A$:
  $$
  IA = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = A
  $$

#### 2. Computing $A + 0$
Here, $0$ is the $2 \times 2$ zero matrix: $0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$.
$$
A + 0 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} + \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = A
$$

#### 3. Computing Powers $A^2$ and $A^3$
* **For $A^2$ ($A \cdot A$):**
  $$
  A^2 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} (2)(2)+(1)(0) & (2)(1)+(1)(2) \\ (0)(2)+(2)(0) & (0)(1)+(2)(2) \end{pmatrix} = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix}
  $$
* **For $A^3$ ($A^2 \cdot A$):**
  $$
  A^3 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \end{pmatrix} = \begin{pmatrix} (4)(2)+(4)(0) & (4)(1)+(4)(2) \\ (0)(2)+(4)(0) & (0)(1)+(4)(2) \end{pmatrix} = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix}
  $$

#### 4. Explanation of Roles and Successive Powers Pattern
* **Role of $I$ (Identity Matrix):** Acts as the multiplicative neutral element. Multiplying any compatible matrix by $I$ leaves the matrix unchanged ($AI = IA = A$).
* **Role of $0$ (Zero Matrix):** Acts as the additive neutral element. Adding the zero matrix leaves the original matrix unchanged ($A + 0 = A$).
* **Pattern in Successive Powers of $A$:**
  * $A^1 = \begin{pmatrix} 2^1 & 1 \cdot 2^0 \cdot 2? \text{ Let's check entries: } 2 & 1 \\ 0 & 2 \end{pmatrix}$
  * $A^2 = \begin{pmatrix} 4 & 4 \\ 0 & 4 \end{pmatrix} = \begin{pmatrix} 2^2 & 2 \cdot 2 \\ 0 & 2^2 \end{pmatrix}$
  * $A^3 = \begin{pmatrix} 8 & 12 \\ 0 & 8 \end{pmatrix} = \begin{pmatrix} 2^3 & 3 \cdot 2^2 \\ 0 & 2^3 \end{pmatrix}$
  
  In general, for any positive integer $n$, the matrix power follows the pattern:
  $$
  A^n = \begin{pmatrix}
  2^n & n \cdot 2^{n-1} \\
  0 & 2^n
  \end{pmatrix}
  $$