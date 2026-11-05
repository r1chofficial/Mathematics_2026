# Exercise 8. Inverse of a Transformation

## Problem

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

## Solution

**Inverse.** For a diagonal matrix, each diagonal entry is replaced by its reciprocal:

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}
$$

**Geometric meaning.** $S$ stretches the horizontal direction by the factor $2$ and compresses the vertical direction by the factor $\frac12$. The inverse does the opposite: it compresses horizontally by $\frac12$ and stretches vertically by $2$, so every point returns to where it started.

**Check on a vector.**

$$
S
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
2 \\
\frac12 \\
\end{pmatrix},\qquad S^{-1}
\begin{pmatrix}
2 \\
\frac12 \\
\end{pmatrix}=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}
$$

**Verification.**

$$
SS^{-1}=
\begin{pmatrix}
2\cdot\frac12 & 0 \\
0 & \frac12\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$
