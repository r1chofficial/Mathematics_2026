# Exercise 14. A System of Equations and the Determinant

## Problem

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

## Solution

**Determinant.**

$$
\det A=1\cdot4-2\cdot k=4-2k
$$

**Exactly one solution.** The system has exactly one solution for every $b$ exactly when $A$ is invertible, that is when $4-2k\neq0$:

$$
k\neq2
$$

In that case the solution is $x=A^{-1}b$.

**The exceptional value k = 2.** The system becomes

$$
\begin{cases}
x_1+2x_2=b_1, \\
2x_1+4x_2=b_2.
\end{cases}
$$

The left side of the second equation is twice the left side of the first.

- **Infinitely many solutions:** $b=(1,\ 2)^T$. The second equation is then twice the first, so only $x_1+2x_2=1$ remains. Its solutions are $x=(1-2s,\ s)^T$ for every real $s$.
- **No solution:** $b=(1,\ 0)^T$. Doubling the first equation gives $2x_1+4x_2=2$, which contradicts $2x_1+4x_2=0$.

**Verification.** For $s=0$ and $s=1$ the vectors $(1,\ 0)^T$ and $(-1,\ 1)^T$ both satisfy $x_1+2x_2=1$ and $2x_1+4x_2=2$.
