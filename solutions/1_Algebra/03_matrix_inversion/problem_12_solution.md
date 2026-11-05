# Exercise 12. Finding Inverses Without Starting from Scratch

## Problem

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## Solution

**Properties used.** For an invertible matrix $A$ and a number $k\neq0$:

$$
(kA)^{-1}=\frac1kA^{-1},\qquad (A^T)^{-1}=(A^{-1})^T,\qquad (A^2)^{-1}=(A^{-1})^2
$$

**Computations.**

$$
(3A)^{-1}=\frac13A^{-1}=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23 \\
\end{pmatrix}
$$

$$
(A^T)^{-1}=(A^{-1})^T=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}
$$

$$
(A^2)^{-1}=(A^{-1})^2=
\begin{pmatrix}
2\cdot2+(-1)\cdot(-3) & 2\cdot(-1)+(-1)\cdot2 \\
(-3)\cdot2+2\cdot(-3) & (-3)\cdot(-1)+2\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}
$$

**Justification.**

- $3A\cdot\frac13A^{-1}=AA^{-1}=I$, because the numbers $3$ and $\frac13$ can be moved freely.
- $A^T(A^{-1})^T=(A^{-1}A)^T=I^T=I$, using $(XY)^T=Y^TX^T$.
- $A^2(A^{-1})^2=AAA^{-1}A^{-1}=AA^{-1}=I$.

**Verification.** Only as a check: since $\det A^{-1}=1$, inverting $A^{-1}$ gives

$$
A=
\begin{pmatrix}
2 & 1 \\
3 & 2 \\
\end{pmatrix},\qquad A^2=
\begin{pmatrix}
7 & 4 \\
12 & 7 \\
\end{pmatrix},\qquad A^2
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$
