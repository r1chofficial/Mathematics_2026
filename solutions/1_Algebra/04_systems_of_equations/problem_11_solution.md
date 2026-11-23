# Exercise 11. A Parameter in a System of Three Equations

## Problem

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

## Solution

**Elimination.** $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

**Case t ≠ 1.** The next step is to divide by $t-1$, which is allowed only when $t-1\neq0$. Then

$$
y=\frac{1}{t-1},\qquad z=\frac{2}{t-1},\qquad x=1-y-z=\frac{t-4}{t-1}.
$$

There is exactly one solution.

**Case t = 1.** Here division by $t-1$ is impossible, so this value is checked separately. The last two rows become

$$
0=1,\qquad 0=2,
$$

which are contradictions, so there is no solution. Indeed, for $t=1$ all three left sides equal $x+y+z$, which cannot be $1$, $2$ and $3$ at the same time.

**Summary.** Exactly one solution for $t\neq1$, no solution for $t=1$. Infinitely many solutions never occur, because at $t=1$ the right-hand sides contradict each other. This agrees with the determinant of the coefficient matrix, $(t-1)^2$, which is zero only for $t=1$.

**Check for t = 2.** The formulas give $(x,\ y,\ z)=(-2,\ 1,\ 2)$, and $-2+1+2=1$, $-2+2+2=2$, $-2+1+4=3$.
