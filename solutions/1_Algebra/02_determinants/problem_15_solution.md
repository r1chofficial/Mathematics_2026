# Exercise 15. Combining Determinant Properties

## Problem

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

## Solution

**Properties used, in order.**

1. Product rule: the determinant of a product is the product of the determinants.
2. Inverse: $\det(B^{-1})=\frac{1}{\det B}$.
3. Transpose: $\det(A^T)=\det A$.

**Computation.**

$$
\begin{aligned}
\det\left(B^{-1}A^TB\right) &= \det(B^{-1})\cdot\det(A^T)\cdot\det B \\
&= \frac{1}{3}\cdot(-2)\cdot3 \\
&= -2
\end{aligned}
$$

**Why the factors with B cancel.** The matrices $B^{-1}$ and $B$ cannot be moved next to each other, because $A^T$ stands between them and matrix multiplication is not commutative. Their determinants, however, are ordinary numbers and can be reordered, and $\frac{1}{\det B}\cdot\det B=1$. Therefore the result equals $\det A$ for every invertible $B$.

**Verification.** For

$$
A=
\begin{pmatrix}
1 & 3 \\
1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 1 \\
0 & 3 \\
\end{pmatrix}
$$

with $\det A=-2$ and $\det B=3$, direct multiplication gives

$$
B^{-1}A^TB=
\begin{pmatrix}
0 & 2 \\
1 & 2 \\
\end{pmatrix},\qquad \det\left(B^{-1}A^TB\right)=0\cdot2-2\cdot1=-2
$$
