# Exercise 8. Row Operations and Their Reversibility

## Problem

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

**Step 1.** $R_2\leftarrow R_2-2R_1$ gives $(2,\ 4,\ 1)-2(1,\ 2,\ -1)=(0,\ 0,\ 3)$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

**Step 2.** $R_3\leftarrow R_3+R_1$ gives $(-1,\ 1,\ 3)+(1,\ 2,\ -1)=(0,\ 3,\ 2)$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2 \\
\end{pmatrix}
$$

**Step 3.** $R_2\leftrightarrow R_3$ gives an upper triangular matrix:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3 \\
\end{pmatrix}
$$

**Reverse operations.**

| Operation | Reverse |
|---|---|
| $R_2\leftarrow R_2-2R_1$ | $R_2\leftarrow R_2+2R_1$ |
| $R_3\leftarrow R_3+R_1$ | $R_3\leftarrow R_3-R_1$ |
| $R_2\leftrightarrow R_3$ | $R_2\leftrightarrow R_3$ (an interchange is its own reverse) |

To return to $A$, the reverse operations are applied in reverse order (step 3 first, step 1 last).

**Verification.** Starting from the final matrix: $R_2\leftrightarrow R_3$, then $R_3\leftarrow R_3-R_1$ gives $(-1,\ 1,\ 3)$, then $R_2\leftarrow R_2+2R_1$ gives $(2,\ 4,\ 1)$. This is the original matrix $A$.
