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