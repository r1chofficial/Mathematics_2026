# Exercise 12. Homogeneous System

## Problem

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## Solution

**Elimination.** $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 0 \\
0 & 0 & 0 & \mid & 0 \\
0 & -3 & 3 & \mid & 0 \\
\end{pmatrix}
$$

The second equation is twice the first, so it adds nothing.

**Solving.** The third row gives $-3y+3z=0$, so $y=z$. Let $z=t$. Then $y=t$ and $x=-2y+z=-t$:

$$
(x,\ y,\ z)=t\,(-1,\ 1,\ 1),\qquad t\in\mathbb{R}
$$

The solutions form a line through the origin.

**Check for t = 1.** $-1+2-1=0$, $-2+4-2=0$ and $-1-1+2=0$.

**Why (0, 0, 0) is always a solution.** In a homogeneous system every right-hand side is zero. Putting $x=y=z=0$ turns every left side into a sum of terms with the factor zero, so every equation reads $0=0$. In matrix form, $A\cdot0=0$ for every matrix $A$. A homogeneous system is therefore never inconsistent; the only question is whether zero is the only solution. Here it is not, because one equation is redundant.
