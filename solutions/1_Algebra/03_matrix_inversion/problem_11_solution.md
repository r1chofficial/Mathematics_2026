# Exercise 11. Parameter and Invertibility

## Problem

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

## Solution

**Determinant.**

$$
\det A(t)=1\cdot1-t\cdot t=1-t^2
$$

**Invertibility.** The matrix is invertible exactly when $1-t^2\neq0$, that is for $t\neq1$ and $t\neq-1$.

**Inverse.** By the $2\times2$ formula,

$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix},\qquad t\neq\pm1
$$

**At the excluded values.** For $t=\pm1$ the denominator $1-t^2$ is zero, so the formula has no meaning. The rows also become dependent: for $t=1$ both rows are $(1,\ 1)$, and for $t=-1$ the second row $(-1,\ 1)$ is the negative of the first row $(1,\ -1)$.

**Verification.** For $t=2$ the formula gives the factor $\frac{1}{1-4}=-\frac13$, and

$$
A(2)A(2)^{-1}=-\frac13
\begin{pmatrix}
1 & 2 \\
2 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -2 \\
-2 & 1 \\
\end{pmatrix}=-\frac13
\begin{pmatrix}
-3 & 0 \\
0 & -3 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$
