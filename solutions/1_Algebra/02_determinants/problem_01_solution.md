# Exercise 1. Determinant of a 2×2 Matrix

## Problem

Compute

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix},\qquad \det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}.
$$

Which matrix is invertible? Justify your answer.

## Solution

**Method.** For a $2\times2$ matrix

$$
\det
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}=ad-bc
$$

**Computation.**

$$
\det
\begin{pmatrix}
3 & -2 \\
5 & 4 \\
\end{pmatrix}=3\cdot4-(-2)\cdot5=12+10=22
$$

$$
\det
\begin{pmatrix}
1 & 7 \\
2 & 14 \\
\end{pmatrix}=1\cdot14-7\cdot2=14-14=0
$$

**Result.** The first matrix is invertible, because its determinant is $22\neq0$. The second matrix is not invertible, because its determinant is $0$.

**Explanation.** A square matrix is invertible exactly when its determinant is nonzero. In the second matrix the second row is twice the first row, so the rows are dependent.

**Verification.** For the first matrix the inverse can be written down explicitly:

$$
\frac{1}{22}
\begin{pmatrix}
4 & 2 \\
-5 & 3 \\
\end{pmatrix}
$$

Multiplying it by the original matrix gives $I$. For example, the upper-left entry is $\frac{3\cdot4+(-2)\cdot(-5)}{22}=\frac{22}{22}=1$.
