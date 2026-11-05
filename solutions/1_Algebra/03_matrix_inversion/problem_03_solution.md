# Exercise 3. When Does the Inverse Not Exist?

## Problem

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## Solution

**Way 1: the determinant.**

$$
\det A=2\cdot2-4\cdot1=0
$$

If an inverse existed, then $AA^{-1}=I$ would give $\det A\cdot\det A^{-1}=\det I=1$. This is impossible when $\det A=0$. In the $2\times2$ formula this shows up as division by zero.

**Way 2: dependent rows.** The first row is twice the second row:

$$
(2,\ 4)=2\cdot(1,\ 2)
$$

Because of this dependence, $A$ sends a nonzero vector to zero:

$$
A
\begin{pmatrix}
2 \\
-1 \\
\end{pmatrix}=
\begin{pmatrix}
2\cdot2+4\cdot(-1) \\
1\cdot2+2\cdot(-1) \\
\end{pmatrix}=
\begin{pmatrix}
0 \\
0 \\
\end{pmatrix}
$$

If $A^{-1}$ existed, multiplying this equation by it would give $(2,\ -1)^T=0$, which is false.

**Connection.** Both arguments describe the same fact: dependent rows are exactly what makes the determinant zero.
