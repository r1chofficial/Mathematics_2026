# Exercise 11. Shortening the Calculation with Row Operations

## Problem

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## Solution

**Plan.** Every entry of the first column equals $1$, so subtracting the first row from the other two creates two zeros at once.

**Step 1.** $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}
$$

**Step 2.** $R_3\leftarrow R_3-2R_2$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

**Result.** The matrix is triangular, so

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}=1\cdot1\cdot1=1
$$

**Operations that do not change the determinant.** Adding a multiple of one row to another row. All three operations used here are of this type. By contrast, swapping two rows changes the sign, and multiplying a row by $k$ multiplies the determinant by $k$.

**Verification.** Sarrus' rule: $(18+8+12)-(9+16+12)=38-37=1$.
