# Exercise 8. Two Systems with the Same Coefficient Matrix

## Problem

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
$$

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

**Both systems at once.** Both systems have the same coefficients, with rows $(2,\ 1)$ and $(1,\ -1)$. So I write both right-hand sides next to the coefficient matrix:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 & 1 \\
1 & -1 & \mid & 1 & 4 \\
\end{pmatrix}
$$

**Elimination.** $R_2\leftarrow 2R_2-R_1$:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 & 1 \\
0 & -3 & \mid & -3 & 7 \\
\end{pmatrix}
$$

**First system.** $-3y=-3$ gives $y=1$, and $2x+1=5$ gives $x=2$. Check: $2\cdot2+1=5$ and $2-1=1$.

**Second system.** $-3y=7$ gives $y=-\frac73$, and $2x-\frac73=1$ gives $x=\frac53$. Check: $2\cdot\frac53-\frac73=1$ and $\frac53+\frac73=4$.

**What is the same.** The row operation and the whole left part of the matrix are identical in both cases. Which operations to use depends only on the coefficient matrix, not on the right-hand side; only the numbers in the last column differ. That is why several systems with the same matrix can be solved together, and why for many right-hand sides it pays to do the elimination of the matrix only once.
