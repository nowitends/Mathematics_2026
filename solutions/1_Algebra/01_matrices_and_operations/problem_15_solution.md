### Exercise 15. Associativity of Multiplication and Different Calculation Paths

          Given
          $$
          A = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix}, \quad 
          B = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix}, \quad 
          C = \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix}.
          $$

          **1. Computing $(AB)C$:**

          First, let's find $AB$:
          $$
          AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix} 
          = \begin{pmatrix} 1(1)+2(2)+0(-1) & 1(0)+2(1)+0(3) \\ 0(1)+1(2)+1(-1) & 0(0)+1(1)+1(3) \end{pmatrix} 
          = \begin{pmatrix} 5 & 2 \\ 1 & 4 \end{pmatrix}
          $$

          Now, multiply $(AB)$ by $C$:
          $$
          (AB)C = \begin{pmatrix} 5 & 2 \\ 1 & 4 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix} 
          = \begin{pmatrix} 5(2)+2(0) & 5(1)+2(-1) \\ 1(2)+4(0) & 1(1)+4(-1) \end{pmatrix} 
          = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}
          $$

          **2. Computing $A(BC)$:**

          First, let's find $BC$:
          $$
          BC = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \end{pmatrix} 
          = \begin{pmatrix} 1(2)+0(0) & 1(1)+0(-1) \\ 2(2)+1(0) & 2(1)+1(-1) \\ -1(2)+3(0) & -1(1)+3(-1) \end{pmatrix} 
          = \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \end{pmatrix}
          $$

          Now, multiply $A$ by $(BC)$:
          $$
          A(BC) = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \end{pmatrix} 
          = \begin{pmatrix} 1(2)+2(4)+0(-2) & 1(1)+2(1)+0(-4) \\ 0(2)+1(4)+1(-2) & 0(1)+1(1)+1(-4) \end{pmatrix} 
          = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}
          $$

          **3. Comparison and Explanation:**

          - **Results:** Both calculation paths give the exact same final matrix: $(AB)C = A(BC) = \begin{pmatrix} 10 & 3 \\ 2 & -3 \end{pmatrix}$.
          - **Operation Count:** 
            - Path 1 $((AB)C)$ computes a $(2 \times 2)$ matrix first, and then multiplies two $(2 \times 2)$ matrices.
              - Path 2 $(A(BC))$ computes a $(3 \times 2)$ matrix first, which involves slightly more intermediate arithmetic operations.
              - **Meaning of Associativity:** Associativity means that when we multiply three matrices together, the grouping (whether we calculate $(AB)$ first or $(BC)$ first) does not change the final result, as long as the order of matrices $(A, B, C)$ remains the same.