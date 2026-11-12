# Exercise 3. Inconsistent System

## Problem

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

## Solution

**Augmented matrix.**

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

**Elimination.** $R_2\leftarrow R_2-2R_1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

**The contradiction.** The second row now means

$$
0\cdot x+0\cdot y=1,
$$

that is $0=1$. No values of $x$ and $y$ can make this true, so the system is inconsistent and has no solution.

**Interpretation in terms of equations.** Doubling the first equation gives $2x+4y=6$, but the second equation says $2x+4y=7$. The same expression cannot equal both $6$ and $7$.

**Geometric meaning.** Both equations describe lines with slope $-\frac12$:

$$
y=\frac32-\frac12x,\qquad y=\frac72-\frac12x.
$$

The lines are parallel and different, so they have no common point.

**Verification.** The coefficient matrix has determinant $1\cdot4-2\cdot2=0$, so the system cannot have exactly one solution, and the row $0=1$ shows that here it has none.
