## Exercise 12. Formula for a Matrix Power

### Question

Let:
$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n + 1$.

*Why this exercise:* teaches how to recognize a pattern and formulate a generalization from several computations.

---

### Solution

#### 1. Computing Successive Powers ($A^2$, $A^3$, $A^4$)
* **For $A^2$ ($A \cdot A$):**
  $$
  A^2 = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1)+(1)(0) & (1)(1)+(1)(1) \\ (0)(1)+(1)(0) & (0)(1)+(1)(1) \end{pmatrix} = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}
  $$

* **For $A^3$ ($A^2 \cdot A$):**
  $$
  A^3 = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1)+(2)(0) & (1)(1)+(2)(1) \\ (0)(1)+(1)(0) & (0)(1)+(1)(1) \end{pmatrix} = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}
  $$

* **For $A^4$ ($A^3 \cdot A$):**
  $$
  A^4 = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} (1)(1)+(3)(0) & (1)(1)+(3)(1) \\ (0)(1)+(1)(0) & (0)(1)+(1)(1) \end{pmatrix} = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}
  $$

#### 2. Formulating the Conjecture for $A^n$
Observing the pattern in the top-right entry as the power increases ($A^2$ has $2$, $A^3$ has $3$, $A^4$ has $4$), we can conjecture that for any positive integer $n$:
$$
A^n = \begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

#### 3. Verifying the Induction Step (Multiplying by $A$)
To rigorously justify this, assume the formula holds for some arbitrary integer $n$. Let's multiply our formula for $A^n$ by $A$ to find $A^{n+1}$:
$$
A^{n+1} = A^n \cdot A = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}
$$
Performing the matrix multiplication:
$$
A^{n+1} = \begin{pmatrix}
(1)(1) + (n)(0) & (1)(1) + (n)(1) \\
(0)(1) + (1)(0) & (0)(1) + (1)(1)
\end{pmatrix} = \begin{pmatrix}
1 & 1 + n \\
0 & 1
\end{pmatrix} = \begin{pmatrix}
1 & n + 1 \\
0 & 1
\end{pmatrix}
$$
This precisely matches our conjectured formula with $n$ replaced by $n + 1$, confirming that the pattern holds for all positive integers $n$.