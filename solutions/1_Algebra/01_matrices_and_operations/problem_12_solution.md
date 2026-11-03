### Exercise 12. Formula for a Matrix Power

            **1. Computing the first few powers:**

            First, let's calculate $A^2$:
            $$
            A^2 = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}
            $$

            Next, let's compute $A^3$:
            $$
            A^3 = A^2 A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix}
            $$

            Now, let's compute $A^4$:
            $$
            A^4 = A^3 A = \begin{pmatrix} 1 & 3 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1 & 4 \\ 0 & 1 \end{pmatrix}
            $$

            **2. Formulating a conjecture:**

            Looking at the pattern from $A^1, A^2, A^3,$ and $A^4$, we can conjecture that for any positive integer $n$:
            $$
            A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}
            $$

            **3. Proof / Verification for $n+1$:**

            Assume the formula holds true for $n$, so $A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}$. 

            Now, let's multiply by $A$ to find $A^{n+1}$:
            $$
            A^{n+1} = A^n A = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix} = \begin{pmatrix} 1\cdot 1 + n\cdot 0 & 1\cdot 1 + n\cdot 1 \\ 0\cdot 1 + 1\cdot 0 & 0\cdot 1 + 1\cdot 1 \end{pmatrix} = \begin{pmatrix} 1 & n+1 \\ 0 & 1 \end{pmatrix}
            $$

            This matches the formula for $n+1$, which proves that $A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \end{pmatrix}$ holds for all positive integers $n$.