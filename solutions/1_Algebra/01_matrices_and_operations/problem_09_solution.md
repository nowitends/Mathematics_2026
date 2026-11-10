## Exercise 9. Composing Transformations

### Question

Let:
$$
S = \begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}, \quad
R = \begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation. For:
$$
x = \begin{pmatrix}
1 \\
2
\end{pmatrix}
$$

Compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

*Why this exercise:* interprets matrix multiplication as composition of transformations.

---

### Solution

#### 1. Computing $RSx$
First, apply the scaling matrix $S$ to vector $x$:
$$
Sx = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 \\ 2 \end{pmatrix} = \begin{pmatrix} (2)(1) + (0)(2) \\ (0)(1) + (1)(2) \end{pmatrix} = \begin{pmatrix} 2 \\ 2 \end{pmatrix}
$$
Next, apply the rotation matrix $R$ to the resulting vector:
$$
RSx = R(Sx) = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 2 \\ 2 \end{pmatrix} = \begin{pmatrix} (0)(2) + (-1)(2) \\ (1)(2) + (0)(2) \end{pmatrix} = \begin{pmatrix} -2 \\ 2 \end{pmatrix}
$$

#### 2. Computing $SRx$
First, apply the rotation matrix $R$ to vector $x$:
$$
Rx = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \begin{pmatrix} 1 \\ 2 \end{pmatrix} = \begin{pmatrix} (0)(1) + (-1)(2) \\ (1)(1) + (0)(2) \end{pmatrix} = \begin{pmatrix} -2 \\ 1 \end{pmatrix}
$$
Next, apply the scaling matrix $S$ to the resulting vector:
$$
SRx = S(Rx) = \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} -2 \\ 1 \end{pmatrix} = \begin{pmatrix} (2)(-2) + (0)(1) \\ (0)(-2) + (1)(1) \end{pmatrix} = \begin{pmatrix} -4 \\ 1 \end{pmatrix}
$$

#### 3. Comparison and Geometric Explanation
Comparing our findings:
$$
RSx = \begin{pmatrix} -2 \\ 2 \end{pmatrix} \neq \begin{pmatrix} -4 \\ 1 \end{pmatrix} = SRx
$$

* **Geometric Meaning:** 
  * In $RSx$, we first stretch the vector horizontally by a factor of 2 (transforming $(1,2)$ into $(2,2)$), and then rotate that stretched vector $90^\circ$ counterclockwise to land at $(-2,2)$.
  * In $SRx$, we first rotate the original vector $90^\circ$ counterclockwise (landing at $(-2,1)$), and then apply the horizontal scaling to stretch its x-coordinate, resulting in $(-4,1)$.

Because the final position of an object depends heavily on the sequence in which geometric transformations are performed, the order matters. This reflects the fundamental noncommutativity of matrix multiplication when viewed as function composition.