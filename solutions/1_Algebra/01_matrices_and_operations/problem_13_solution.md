## Exercise 13. A Recurrence Written in Matrix Form

### Question

Let:
$$
F = \begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence:
$$0, 1, 1, 2, 3, 5, 8, \dots$$
and describe the relationship you observe. Then compute:
$$
F \begin{pmatrix} a \\ b \end{pmatrix}
$$
and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

*Why this exercise:* shows the connection between matrix powers and a simple numerical recurrence.

---

### Solution

#### 1. Computing Powers of $F$ ($F^2$, $F^3$, $F^4$, $F^5$)
* **For $F^2$:**
  $$
  F^2 = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (1)(1)+(1)(1) & (1)(1)+(1)(0) \\ (1)(1)+(0)(1) & (1)(1)+(0)(0) \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
  $$

* **For $F^3$ ($F^2 \cdot F$):**
  $$
  F^3 = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (2)(1)+(1)(1) & (2)(1)+(1)(0) \\ (1)(1)+(1)(1) & (1)(1)+(1)(0) \end{pmatrix} = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
  $$

* **For $F^4$ ($F^3 \cdot F$):**
  $$
  F^4 = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (3)(1)+(2)(1) & (3)(1)+(2)(0) \\ (2)(1)+(1)(1) & (2)(1)+(1)(0) \end{pmatrix} = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
  $$

* **For $F^5$ ($F^4 \cdot F$):**
  $$
  F^5 = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} (5)(1)+(3)(1) & (5)(1)+(3)(0) \\ (3)(1)+(2)(1) & (3)(1)+(2)(0) \end{pmatrix} = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
  $$

#### 2. Relationship with the Fibonacci Sequence
Comparing the entries of these matrices with the Fibonacci sequence ($0, 1, 1, 2, 3, 5, 8, \dots$), we notice that the entries of $F^n$ are consecutive Fibonacci numbers. Specifically, $F^n$ can be expressed as:
$$
F^n = \begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
$$
For instance, $F^5 = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}$, where $8 = F_6$, $5 = F_5$, and $3 = F_4$.

#### 3. Multiplying $F$ by a General Vector $\begin{pmatrix} a \\ b \end{pmatrix}$
Let's compute the product:
$$
F \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} (1)(a) + (1)(b) \\ (1)(a) + (0)(b) \end{pmatrix} = \begin{pmatrix} a + b \\ a \end{pmatrix}
$$

* **Explanation of the Recurrence Step:** 
  If we think of $a$ and $b$ as two consecutive terms in a sequence (where $a$ is the current term and $b$ is the previous term), multiplying by $F$ generates the next term ($a + b$) in the top position, while passing the current term $a$ down to the bottom position to serve as the previous term in the next iteration. This matrix multiplication encapsulates a single step of the Fibonacci recurrence relation.