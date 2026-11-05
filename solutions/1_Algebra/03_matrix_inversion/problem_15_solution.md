# Exercise 15. Two Methods for Solving the Same System

## Problem

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

**Method 1: the inverse.** This is the same matrix as in Exercise 6, so

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix},\qquad x=A^{-1}b=\frac15
\begin{pmatrix}
3\cdot7-8 \\
-7+2\cdot8 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}
$$

**Method 2: Gaussian elimination.** The system is

$$
\begin{cases}
2x_1+x_2=7, \\
x_1+3x_2=8.
\end{cases}
$$

The operation $R_2\leftarrow 2R_2-R_1$ gives $5x_2=9$, so $x_2=\frac95$. Substituting into the first equation gives $2x_1=7-\frac95=\frac{26}{5}$, so $x_1=\frac{13}{5}$.

**Comparison.** Both methods give the same solution $x=(\frac{13}{5},\ \frac95)^T$.

| Method | Essential steps |
|---|---|
| inverse | determinant, inverse matrix, matrix-vector product |
| elimination | one row operation, one back substitution |

**Which was simpler.** Here elimination was simpler: it needs fewer calculations and no inverse matrix. The inverse is worth computing when the same matrix appears with several right-hand sides, as in Exercises 6 and 15: once $A^{-1}$ is known, each new $b$ needs only one multiplication.

**Verification.** $2\cdot\frac{13}{5}+\frac95=\frac{35}{5}=7$ and $\frac{13}{5}+3\cdot\frac95=\frac{40}{5}=8$.
