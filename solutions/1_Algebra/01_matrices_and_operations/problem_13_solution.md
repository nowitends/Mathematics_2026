### Exercise 13. A Recurrence Written in Matrix Form

          Let
          $$
          F = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix}.
          $$

          **1. Computing powers of $F$:**

          First, let's calculate $F^2$:
          $$
          F^2 = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix}
          $$

          Next, let's compute $F^3$:
          $$
          F^3 = F^2 F = \begin{pmatrix} 2 & 1 \\ 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix}
          $$

          Now, let's compute $F^4$:
          $$
          F^4 = F^3 F = \begin{pmatrix} 3 & 2 \\ 2 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix}
          $$

          Finally, let's compute $F^5$:
          $$
          F^5 = F^4 F = \begin{pmatrix} 5 & 3 \\ 3 & 2 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} = \begin{pmatrix} 8 & 5 \\ 5 & 3 \end{pmatrix}
          $$

          **2. Comparing with the Fibonacci sequence:**

          The given sequence $0, 1, 1, 2, 3, 5, 8, \dots$ is the Fibonacci sequence, where each term is the sum of the two preceding terms.

          Comparing the entries of the matrix powers $F^n$ with the Fibonacci numbers $F_n$ (where $F_0=0, F_1=1, F_2=1, F_3=2, F_4=3, F_5=5, F_6=8, \dots$), we observe that:
          $$
          F^n = \begin{pmatrix} F_{n+1} & F_n \\ F_n & F_{n-1} \end{pmatrix}
          $$

          **3. Computing $F \begin{pmatrix} a \\ b \end{pmatrix}$ and explaining the recurrence step:**

          $$
          F \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} 1 & 1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} a \\ b \end{pmatrix} = \begin{pmatrix} a + b \\ a \end{pmatrix}
          $$

          **Explanation:**
          Multiplying a column vector $\begin{pmatrix} a \\ b \end{pmatrix}$ by $F$ generates a new vector where:
          - The top entry becomes $a + b$, which is the sum of two consecutive terms in the sequence.
          - The bottom entry becomes $a$, which keeps the previous term for the next step.

          This shows how matrix multiplication can naturally perform a recurrence step.