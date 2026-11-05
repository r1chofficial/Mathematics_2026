# Exercise 13. Determinant by Elimination

## Problem

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

| Step | Operation | Effect on the determinant |
|---|---|---|
| 1 | $R_2\leftarrow R_2-2R_1$ | unchanged |
| 2 | $R_3\leftarrow R_3-R_1$ | unchanged |
| 3 | $R_3\leftarrow R_3+2R_2$ | unchanged |

**After steps 1 and 2.**

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}
$$

**After step 3.**

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}
$$

**Result.** The matrix is triangular and no operation changed the determinant, so

$$
\det A=1\cdot1\cdot1=1
$$

**Verification.** Sarrus' rule: $(10+14+0)-(15+0+8)=24-23=1$.
