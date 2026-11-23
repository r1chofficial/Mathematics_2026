# Exercise 4. Infinitely Many Solutions

## Problem

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

## Solution

**Augmented matrix.**

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

**Elimination.** $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

The second equation is twice the first, so it becomes $0=0$ and adds no information. Only two independent equations remain for three unknowns.

**Solving.** The third row gives $-2y=-2$, so $y=1$. The first row then gives $x+z=1$. The variable $z$ has no pivot, so it is the free variable: $z=t$ and $x=1-t$.

**Parametric form.**

$$
(x,\ y,\ z)=(1-t,\ 1,\ t)=(1,\ 1,\ 0)+t\,(-1,\ 0,\ 1),\qquad t\in\mathbb{R}
$$

Geometrically, the solution set is a line in space.

**Check for t = 2.** The point is $(-1,\ 1,\ 2)$:

$$
\begin{aligned}
-1+1+2 &= 2, \\
2\cdot(-1)+2\cdot1+2\cdot2 &= 4, \\
-1-1+2 &= 0.
\end{aligned}
$$

All three equations hold.
