# Exercise 2. Determinant of a 3×3 Matrix

## Problem

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

## Solution

**Method.** Sarrus' rule: add the three products along the main diagonals and subtract the three products along the anti-diagonals.

$$
\begin{aligned}
\det A &= 1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1 \\
&\quad -\big((-1)\cdot3\cdot2+1\cdot4\cdot1+2\cdot0\cdot5\big) \\
&= (15+16+0)-(-6+4+0) \\
&= 31-(-2)=33
\end{aligned}
$$

**Result.** $\det A=33$.

**Check with a property.** Adding a multiple of one row to another does not change the determinant. The operation $R_3\leftarrow R_3-2R_1$ gives a matrix with two zeros in the first column:

$$
\det
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7 \\
\end{pmatrix}=1\cdot\big(3\cdot7-4\cdot(-3)\big)=21+12=33
$$

Expanding along the first column gives the same value.
