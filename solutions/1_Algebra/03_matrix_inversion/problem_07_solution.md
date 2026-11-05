# Exercise 7. Inverse of a Product

## Problem

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## Solution

**Left side.**

$$
AB=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix},\qquad \det(AB)=6,\qquad (AB)^{-1}=\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
$$

**Right side.**

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix},\qquad B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}
$$

**Result.** The two matrices are equal, so $(AB)^{-1}=B^{-1}A^{-1}$.

**Meaning of the reversed order.** In $ABx$ the matrix $B$ acts first and $A$ acts second. To undo this, we must first undo the last step, $A$, and only then $B$. It is like socks and shoes: the shoes come off first.

**The wrong order gives something else.**

$$
A^{-1}B^{-1}=
\begin{pmatrix}
\frac12 & -\frac13 \\
0 & \frac13 \\
\end{pmatrix}\neq(AB)^{-1}
$$
