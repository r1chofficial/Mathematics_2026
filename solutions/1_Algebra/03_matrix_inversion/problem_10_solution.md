# Exercise 10. Inverse of a Diagonal Matrix

## Problem

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},\qquad E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}.
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

**Rule.** The determinant of a diagonal matrix is the product of its diagonal entries. So a diagonal matrix is invertible exactly when no diagonal entry is zero, and then its inverse is diagonal with the reciprocal entries.

**The matrix D.** $\det D=2\cdot(-3)\cdot5=-30\neq0$, so $D$ is invertible:

$$
D^{-1}=
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}
$$

**The matrix E.** $\det E=2\cdot0\cdot5=0$, so $E$ is not invertible. Its second column is zero, so for example $E(0,\ 1,\ 0)^T=0$, and no matrix can bring this nonzero vector back.

**Verification.**

$$
DD^{-1}=
\begin{pmatrix}
2\cdot\frac12 & 0 & 0 \\
0 & (-3)\cdot(-\frac13) & 0 \\
0 & 0 & 5\cdot\frac15 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}
$$
