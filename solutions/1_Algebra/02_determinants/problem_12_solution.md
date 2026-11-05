# Exercise 12. A Parameter Revealed by a Row Operation

## Problem

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

## Solution

**Row operation.** $R_2\leftarrow R_2-2R_1$ does not change the determinant:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}
$$

**Determinant.** Expanding along the first column:

$$
\det A(t)=1\cdot\det
\begin{pmatrix}
0 & t-6 \\
1 & 1 \\
\end{pmatrix}=0\cdot1-(t-6)\cdot1=6-t
$$

**Result.** $A(t)$ is not invertible exactly for $t=6$.

**What happens to the rows.** For $t=6$ the new second row is the zero row, so the original second row is exactly twice the first:

$$
(2,\ 4,\ 6)=2\cdot(1,\ 2,\ 3)
$$

The rows are dependent, which is why the determinant is zero.

**Verification.** Cofactor expansion of the original matrix along the first row:

$$
1\cdot(4-t)-2\cdot(2-0)+3\cdot(2-0)=4-t-4+6=6-t
$$
