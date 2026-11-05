# Exercise 1. Definition of the Inverse

## Problem

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## Solution

**Definition.** A matrix $B$ is the inverse of a square matrix $A$ if

$$
AB=BA=I.
$$

**Computation.**

$$
AB=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

$$
BA=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}
$$

**Result.** Both products equal the identity matrix $I$, so $B$ satisfies the definition and $B=A^{-1}$.

**Verification.** $\det A=2-1=1$ and $\det B=2-1=1$, which agrees with $\det A\cdot\det B=\det I=1$.
