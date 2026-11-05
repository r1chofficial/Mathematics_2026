# Exercise 4. Triangular Matrix

## Problem

Without expanding the determinant, compute

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}.
$$

State the rule for an arbitrary triangular matrix and explain it using this example.

## Solution

**Result.**

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}=2\cdot(-3)\cdot7=-42
$$

**Rule.** The determinant of a triangular matrix, upper or lower, is the product of its diagonal entries.

**Explanation on this example.** Expanding along the first column, only the entry $2$ is nonzero:

$$
\det
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7 \\
\end{pmatrix}=2\cdot\det
\begin{pmatrix}
-3 & 5 \\
0 & 7 \\
\end{pmatrix}=2\cdot(-3)\cdot7=-42
$$

The smaller matrix is again triangular, so the same step repeats until only the diagonal entries remain. The zeros below the diagonal remove all other terms, so the entries above the diagonal, namely $4$, $1$ and $5$, never influence the result.

**Verification.** In Sarrus' rule every product except $2\cdot(-3)\cdot7$ contains at least one of the zeros below the diagonal.
