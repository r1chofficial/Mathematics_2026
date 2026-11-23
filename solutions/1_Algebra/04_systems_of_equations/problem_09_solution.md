# Exercise 9. A System from a Sum Condition

## Problem

Find numbers $x,y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why the solution is unique.

## Solution

**Elimination.** $R_2\leftarrow R_2-2R_1$ removes $x$ from the second equation:

$$
\begin{cases}
x+y=10, \\
3y=12.
\end{cases}
$$

So $y=4$ and $x=10-4=6$.

**Check.** $6+4=10$ and $2\cdot6+5\cdot4=12+20=32$.

**Why the solution is unique.** Each equation describes a line in the plane:

$$
y=10-x,\qquad y=\frac{32}{5}-\frac25x.
$$

The slopes $-1$ and $-\frac25$ are different, so the lines are not parallel and cross in exactly one point, $(6,\ 4)$. Equivalently, the coefficient matrix has determinant $1\cdot5-1\cdot2=3\neq0$.
