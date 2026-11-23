# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Problem

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

## Solution

**Elimination.** $R_2\leftarrow R_2-aR_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
a & a & \mid & 4 \\
\end{pmatrix}\quad\to\quad
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 4-2a \\
\end{pmatrix}
$$

**Case a = 2.** The last row is $0=0$. Only $x+y=2$ remains, so there are infinitely many solutions:

$$
(x,\ y)=(2-s,\ s),\qquad s\in\mathbb{R}
$$

**Case a ≠ 2.** The last row reads $0=4-2a$ with $4-2a\neq0$, which is a contradiction. There is no solution. For example, $a=0$ gives $0=4$.

**Exactly one solution never occurs.** The left side of the second equation is always $a$ times the left side of the first, so elimination always produces a zero row on the left. Equivalently, the coefficient matrix has determinant $1\cdot a-1\cdot a=0$ for every $a$. Geometrically, for $a\neq0$ the equations describe the parallel lines $x+y=2$ and $x+y=\frac4a$, which either coincide or never meet, but never cross in a single point.

**Summary.** Infinitely many solutions for $a=2$, no solution for every other $a$, and exactly one solution for no value of $a$.
