# Exercise 1. From a System to a Matrix

## Problem

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

**Matrix form.**

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}
$$

**The three parts.**

- Coefficient matrix $A$: the $3\times3$ matrix of the numbers in front of $x$, $y$, $z$.
- Vector of unknowns $x=(x,\ y,\ z)^T$.
- Right-hand side vector $b=(4,\ 1,\ 7)^T$.

**Rows and equations.** Row $i$ of $A$ contains the coefficients of equation $i$, and entry $i$ of $b$ is its right-hand side. Each column of $A$ belongs to one unknown: the first column to $x$, the second to $y$, the third to $z$. A missing unknown would give a $0$ in its column.

**Verification.** Multiplying out the first row gives

$$
2\cdot x+(-1)\cdot y+1\cdot z=2x-y+z,
$$

which is the left side of the first equation, and the first entry of $b$ is $4$. The other two rows give the second and third equations in the same way.
