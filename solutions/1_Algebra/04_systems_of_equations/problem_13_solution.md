# Exercise 13. Does Every Equation Add New Information?

## Problem

Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

## Solution

**Augmented matrix.**

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

**Elimination.** $R_3\leftarrow R_3-R_1$, then $R_3\leftarrow R_3+R_2$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

**Solution.** The last row is $0=0$, so the system is consistent, with one free variable. Let $x_3=t$. Then $x_2=8-t$ and $x_1=10-x_2=2+t$:

$$
(x_1,\ x_2,\ x_3)=(2+t,\ 8-t,\ t),\qquad t\in\mathbb{R}
$$

**The third equation is not needed.** Subtracting the second equation from the first gives

$$
(x_1+x_2)-(x_2+x_3)=10-8\quad\Rightarrow\quad x_1-x_3=2,
$$

which is exactly the third equation. It follows from the other two and adds no new information, so the first two equations alone describe the same solution set. This is why elimination produced a zero row.

**Check for t = 0.** The point $(2,\ 8,\ 0)$ gives $2+8=10$, $8+0=8$ and $2-0=2$.
