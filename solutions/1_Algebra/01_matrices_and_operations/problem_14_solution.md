## Exercise 14. Rotation Matrices

### Question

The matrix for a rotation through an angle $\theta$ is:
$$
R(\theta) = \begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that:
$$
R(\alpha)R(\beta) = R(\alpha + \beta)
$$

Explain the result geometrically.

*Why this exercise:* shows the consistency between matrix algebra and the geometry of composing rotations.

---

### Solution

#### 1. Computing the Product $R(\alpha)R(\beta)$
Multiplying the two rotation matrices:
$$
R(\alpha)R(\beta) = \begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}
$$

Calculating each entry using standard matrix multiplication:
* **Top-left entry:** $\cos\alpha\cos\beta - \sin\alpha\sin\beta$
* **Top-right entry:** $-\cos\alpha\sin\beta - \sin\alpha\cos\beta = -(\sin\alpha\cos\beta + \cos\alpha\sin\beta)$
* **Bottom-left entry:** $\sin\alpha\cos\beta + \cos\alpha\sin\beta$
* **Bottom-right entry:** $-\sin\alpha\sin\beta + \cos\alpha\cos\beta = \cos\alpha\cos\beta - \sin\alpha\sin\beta$

#### 2. Applying Trigonometric Angle-Sum Formulas
Using the standard angle-sum identities:
* $\cos(\alpha + \beta) = \cos\alpha\cos\beta - \sin\alpha\sin\beta$
* $\sin(\alpha + \beta) = \sin\alpha\cos\beta + \cos\alpha\sin\beta$

Substituting these into our matrix entries gives:
$$
R(\alpha)R(\beta) = \begin{pmatrix}
\cos(\alpha + \beta) & -\sin(\alpha + \beta) \\
\sin(\alpha + \beta) & \cos(\alpha + \beta)
\end{pmatrix}
$$
This expression is identically equal to $R(\alpha + \beta)$.

#### 3. Geometric Explanation
Geometrically, multiplying two rotation matrices represents the composition (successive application) of two rotations in the plane: first rotating by angle $\beta$ and then by angle $\alpha$. Performing a rotation by $\beta$ followed by a rotation by $\alpha$ is equivalent to performing a single rotation by the sum of the angles, $\alpha + \beta$.