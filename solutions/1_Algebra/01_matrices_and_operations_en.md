Exercise 1. Matrix Size and Entries

Answers

1. Sizes of matrices A and B:
    * Matrix A: 2 × 3
    * Matrix B: 3 × 2
2. Matrix entries:
    * a₁₂ = -1
    * a₂₃ = 5
    * b₂₁ = -2
3. Second row of A and first column of B:
    * Second row of A: (0, 4, 5)
    * First column of B: (1, -2, 4)ᵀ 
    
    Exercise 2. Addition and Scalar Multiplication
Answers

1. A + B
    A + B = [[5, 0], [-1, 8]]
2. A - B
    Apş - B = [[-3, 4], [-1, -2]]
3. 3A - 2B
    3A - 2B = [[-5, 10], [-3, -1]]
4. Explanation
    Matrix addition and subtraction are possible only for matrices of the same size because corresponding entries must be added or subtracted. Both matrices A and B are 2 × 2 matrices.
    
    Exercise 3. When Can Matrices Be Multiplied?

    Solution

    The sizes of the matrices are:

    * A = 2 × 3
    * B = 3 × 4
    * C = 4 × 2
    * D = 2 × 2

    For matrix multiplication, the number of columns in the first matrix must be equal to the number of rows in the second matrix.

    * AB: Defined. The sizes match (3 = 3), so the result is 2 × 4.
    * BA: Not defined. The sizes do not match (4 ≠ 2).
    * BC: Defined. The sizes match (4 = 4), so the result is 3 × 2.
    * CB: Not defined. The sizes do not match (2 ≠ 3).
    * AC: Not defined. The sizes do not match (3 ≠ 4).
    * CA: Defined. The sizes match (2 = 2), so the result is 4 × 3.
    * AD: Not defined. The sizes do not match (3 ≠ 2).
    * DA: Defined. The sizes match (2 = 2), so the result is 2 × 3.
    
    Exercise 4. Matrix Multiplication and Noncommutativity

    A = [[1, 2], [0, 1]]

    B = [[2, 0], [3, 1]]

    1. AB = [[8, 2], [3, 1]]
    2. BA = [[2, 4], [3, 7]]
    3. AB is not equal to BA.

    The results are different because the order of multiplication matters for matrices.
    
    Exercise 5. Matrix Times Vector

    1. Ax = [6, 10]ᵀ
    2. Ax = 4[2, 1]ᵀ + 2[-1, 3]ᵀ = [6, 10]ᵀ

    Exercise 6. Transpose

    1. Aᵀ = [[1, 4], [2, 5], [3, 6]]
    2. Bᵀ = [[1, 2, -1], [0, 1, 3]]
    3. AB = [[2, 11], [8, 23]]
    4. (AB)ᵀ = [[2, 8], [11, 23]]
        BᵀAᵀ = [[2, 8], [11, 23]]
            Both results are the same, so (AB)ᵀ = BᵀAᵀ.

        Exercise 7. Identity Matrix, Zero Matrix, and Powers

        1. AI = A
        2. IA = A
        3. A + 0 = A
        4. A² = [[4, 4], [0, 4]]
        5. A³ = [[8, 12], [0, 8]]

        The identity matrix keeps A the same when multiplying. Adding zero also keeps A the same. For A² and A³, I multiply A by itself.

            Exercise 8. Row Operations and Their Reversibility

            Step 1: R₂ ← R₂ − 2R₁

            [
            \begin{pmatrix}
            1&2&-1\
            0&0&3\
            -1&1&3
            \end{pmatrix}
            ]

            Reverse operation: (R_2 \leftarrow R_2+2R_1)

            Step 2: R₃ ← R₃ + R₁

            [
            \begin{pmatrix}
            1&2&-1\
            0&0&3\
            0&3&2
            \end{pmatrix}
            ]

            Reverse operation: (R_3 \leftarrow R_3-R_1)

            Step 3: Interchange R₂ and R₃

            [
            \begin{pmatrix}
            1&2&-1\
            0&3&2\
            0&0&3
            \end{pmatrix}
            ]

            Reverse operation: Interchange (R_2) and (R_3) again.

            Conclusion: Each row operation can be reversed by using the opposite operation or swapping the rows again.

          Exercise 9. Composing Transformations

          1. Calculate (Sx):

          [
          Sx=\begin{pmatrix}2\2\end{pmatrix}
          ]

          2. Calculate (R(Sx)):

          [
          RSx=\begin{pmatrix}-2\2\end{pmatrix}
          ]

          3. Calculate (Rx):

          [
          Rx=\begin{pmatrix}-2\1\end{pmatrix}
          ]

          4. Calculate (S(Rx)):

          [
          SRx=\begin{pmatrix}-4\1\end{pmatrix}
          ]

          Explanation:

          The results are different because the order of transformations matters. First scaling and then rotating gives a different result from rotating and then scaling.

            Exercise 10. Columns of a Matrix Product

            1. The columns of B are:

            (b_1=\begin{pmatrix}1\-1\3\end{pmatrix}), (b_2=\begin{pmatrix}2\0\1\end{pmatrix})

            (Ab_1=\begin{pmatrix}-5\2\end{pmatrix})

            (Ab_2=\begin{pmatrix}2\1\end{pmatrix})

            2. Multiplying A and B gives:
            [
            AB=\begin{pmatrix}
            -5 & 2\
            2 & 1
            \end{pmatrix}
            ]

            3. The columns of AB are the same as (Ab_1) and (Ab_2). This is because each column of AB is found by multiplying A by the corresponding column of B.

            Exercise 11. When Do Matrices Commute?

            First, calculate (AB) and (BA).
            [
            AB=\begin{pmatrix}
            a+c&b+d\
            c&d
            \end{pmatrix}
            ]

            [
            BA=\begin{pmatrix}
            a& a+b\
            c&c+d
            \end{pmatrix}
            ]

            For (AB=BA), the corresponding entries must be equal.

            So we get:

            [
            c=0,\qquad d=a
            ]

            and

            [
            b=0
            ]

            Therefore, the conditions are (b=0,\ c=0,\ d=a).

            The general form of B is:

            [
            B=\begin{pmatrix}
            a&0\
            0&a
            \end{pmatrix}
            =aI
            ]

            So B must be a scalar multiple of the identity matrix.

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

          ### Exercise 14. Rotation Matrices

          The matrix for a rotation through an angle $\theta$ is
          $$
          R(\theta) = \begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{pmatrix}.
          $$

          **1. Computing $R(\alpha)R(\beta)$:**

          Let's multiply $R(\alpha)$ and $R(\beta)$:
          $$
          R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha & -\sin\alpha \\ \sin\alpha & \cos\alpha \end{pmatrix} \begin{pmatrix} \cos\beta & -\sin\beta \\ \sin\beta & \cos\beta \end{pmatrix}
          $$

          Multiplying the rows by columns:
          $$
          R(\alpha)R(\beta) = \begin{pmatrix} \cos\alpha\cos\beta - \sin\alpha\sin\beta & -\cos\alpha\sin\beta - \sin\alpha\cos\beta \\ \sin\alpha\cos\beta + \cos\alpha\sin\beta & -\sin\alpha\sin\beta + \cos\alpha\cos\beta \end{pmatrix}
          $$

          **2. Applying angle-sum formulas:**

          Now, we use the trigonometric sum formulas for sine and cosine[span_0](start_span)[span_0](end_span):
          - $\cos(\alpha + \beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$
          - $\sin(\alpha + \beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta$

          Substituting these formulas into our matrix:
          $$
          R(\alpha)R(\beta) = \begin{pmatrix} \cos(\alpha + \beta) & -\sin(\alpha + \beta) \\ \sin(\alpha + \beta) & \cos(\alpha + \beta) \end{pmatrix} = R(\alpha + \beta)
          $$

          This proves that $R(\alpha)R(\beta) = R(\alpha + \beta)$[span_1](start_span)[span_1](end_span).

          **3. Geometric explanation:**

          Geometrically, $R(\beta)$ rotates a vector in the plane by an angle $\beta$, and then $R(\alpha)$ rotates the result further by an angle $\alpha$. 

          Doing these two rotations one after another is exactly equivalent to doing a single combined rotation by the total angle $\alpha + \beta

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