# Exercise 3 – When Can Matrices Be Multiplied?

## Question

The matrix sizes are:

\[
A_{2\times3},\quad B_{3\times4},\quad
C_{4\times2},\quad D_{2\times2}
\]

For the following products:

\[
AB,\ BA,\ BC,\ CB,\ AC,\ CA,\ AD,\ DA
\]

Determine whether each product is defined. If it is defined, find the size of the result.

## Solution

For matrix multiplication, the number of columns of the first matrix must be equal to the number of rows of the second matrix.

1. \(AB\): \((2\times3)(3\times4)\) – Defined. Result: \(2\times4\).

2. \(BA\): \((3\times4)(2\times3)\) – Not defined, because \(4\neq2\).

3. \(BC\): \((3\times4)(4\times2)\) – Defined. Result: \(3\times2\).

4. \(CB\): \((4\times2)(3\times4)\) – Not defined, because \(2\neq3\).

5. \(AC\): \((2\times3)(4\times2)\) – Not defined, because \(3\neq4\).

6. \(CA\): \((4\times2)(2\times3)\) – Defined. Result: \(4\times3\).

7. \(AD\): \((2\times3)(2\times2)\) – Not defined, because \(3\neq2\).

8. \(DA\): \((2\times2)(2\times3)\) – Defined. Result: \(2\times3\).

The products \(AB\), \(BC\), \(CA\) and \(DA\) are defined. The other four products are not defined because their inner dimensions are different.