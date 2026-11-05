# Exercise 2. Formula for a 2×2 Matrix

## Problem

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## Solution

**Formula.** If $ad-bc\neq0$, then

$$
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}
$$

**Computation.** $\det A=3\cdot4-2\cdot5=2\neq0$, so

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & -1 \\
-\frac52 & \frac32 \\
\end{pmatrix}
$$

**Verification.**

$$
AA^{-1}=
\begin{pmatrix}
3\cdot2+2\cdot(-\frac52) & 3\cdot(-1)+2\cdot\frac32 \\
5\cdot2+4\cdot(-\frac52) & 5\cdot(-1)+4\cdot\frac32 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$
