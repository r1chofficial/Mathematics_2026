# Exercise 10. Detecting Dependence

## Problem

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

**Observation.** The second row is twice the first row:

$$
(2,\ 4,\ 6)=2\cdot(1,\ 2,\ 3)
$$

**Why the determinant is zero.** The operation $R_2\leftarrow R_2-2R_1$ does not change the determinant and produces a zero row:

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=\det
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5 \\
\end{pmatrix}=0
$$

A determinant with a zero row is zero, because expanding along that row gives only zero terms.

**Dependence.** $2R_1-R_2=0$, so a nontrivial combination of the rows gives the zero row.

**Connection with invertibility.** Because the rows are dependent, the matrix is not invertible. Concretely, it sends a nonzero vector to zero:

$$
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}
\begin{pmatrix}
7 \\
-5 \\
1 \\
\end{pmatrix}=
\begin{pmatrix}
0 \\
0 \\
0 \\
\end{pmatrix}
$$

If an inverse existed, multiplying both sides by it would give $(7,\ -5,\ 1)^T=0$, which is false.
