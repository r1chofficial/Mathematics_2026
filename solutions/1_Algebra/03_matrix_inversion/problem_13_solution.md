# Exercise 13. Undoing a Composite Transformation

## Problem

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

## Solution

**Way 1: compute T first.**

$$
T=HS=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad \det T=2,\qquad T^{-1}=\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}
$$

**Way 2: inverse of a product.**

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}
$$

Both ways give the same matrix.

**Wrong order.**

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}\neq T^{-1}
$$

**The rule.** $T=HS$ means: first scale with $S$, then shear with $H$. To undo this, we start from the end: first remove the shear with $H^{-1}$, then remove the scaling with $S^{-1}$. As a product this is $S^{-1}H^{-1}$, because the matrix that acts first stands on the right.

**Verification on a vector.** $T(1,\ 1)^T=(3,\ 1)^T$. The correct inverse gives $T^{-1}(3,\ 1)^T=(1,\ 1)^T$, while the wrong order gives $H^{-1}S^{-1}(3,\ 1)^T=(\frac12,\ 1)^T$.
